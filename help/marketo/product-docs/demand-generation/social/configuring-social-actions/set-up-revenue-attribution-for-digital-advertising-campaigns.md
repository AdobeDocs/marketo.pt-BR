---
unique-page-id: 10098812
description: Configurar atribuição de receita para Campanhas de publicidade digital - Documentos do marketing - Documentação do produto
title: Configurar atribuição de receita para Campanhas de publicidade digital
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 0%

---


# Configurar atribuição de receita para Campanhas de publicidade digital {#set-up-revenue-attribution-for-digital-advertising-campaigns}

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Veja como configurar a atribuição de receita para canais e campanhas de publicidade digital. Depois de configurá-lo, você pode fazer a atribuição de receita de primeiro toque e multitoque para anúncios digitais da mesma forma que em outros programas de marketing.

Depois de configurar seu primeiro programa de anúncio no Marketo, você pode cloná-lo e atualizá-lo para outros canais. Por exemplo, clone um programa do LinkedIn para um do Facebook.

Com programas separados, você pode rastrear o número de conversões de cada um e ver seus programas no Programa Analyzer, no Opportunity Influence Analyzer e em outros recursos do Marketing Cloud Analytics.

>[!NOTE]
>
>**Pré-requisitos**
>
>* Configure uma tag de canal com valores de status e sucesso de programa (por exemplo, Anúncio digital ou Publicidade social paga e PPC)
>* Criar ou editar um formulário para passar uma sequência de query com a pessoa
>* Verifique se você tem acesso a alguns recursos do Revenue Cycle Analytics para relatar sobre seus canais e campanhas de anúncios

>



## Criar um Programa padrão {#create-a-default-program}

Ao contrário de alguns programas (como e-mail) que podem ser executados periodicamente por um período específico, os programas padrão estão sempre ativados.

1. Vá para **Marketing Atividade**.

   ![](assets/login-marketing-activities-5.png)

1. Clique em **Novo** e selecione **Novo Programa**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Se você já tiver um programa no lugar, você pode [cloná-lo](../../../../product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Sempre que clonar um programa, substitua os nomes nos campos da sequência de query das listas inteligentes.

1. Coloque o novo programa em uma pasta de campanha específica, depois que o programa inicial for definido.

   >[!NOTE]
   >
   >**Exemplo**
   >
   >
   >Uma sequência de caracteres de query transmitida pelo URL ajuda o Marketo a saber em qual campanha de anúncio alguém clicou quando se tornou uma pessoa no Marketo.
   >
   >
   >Você pode criar uma metodologia de sequência de query que inclua todas as variáveis que deseja medir. O Marketo usa essas variáveis para adicionar pessoas a seus diferentes programas.
   >
   >
   >Por exemplo, você pode usar o tipo de Canal type_Canal__Asset__Region. Isso pode parecer: SP_FB_NewGuide_US. **Observação**: abreviações economizam espaço.
   >
   >
   >Ou configure-o como Canal_Adsource_AssetName_Region_UniqueIdNumber. Isso pode parecer: Social-Paid_Facebook_NewGuide_NA_123.

## Criar uma Campanha inteligente para novos nomes {#create-a-smart-campaign-for-new-names}

1. Na campanha inteligente, crie uma lista inteligente que contenha dois acionadores e dois filtros, como mostrado.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >A string de query usada nos dois acionadores e o filtro **Programa que captou o nome** é exclusivo para você. As strings de query mostradas aqui são apenas por exemplo. Se você clonou o campo, basta substituir esses campos.

1. Crie uma etapa de fluxo para alterar o atributo para Programa **de** aquisição e defina o Novo valor como o valor definido para campanhas sociais pagas.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Agende e ativa a campanha.

## Criar uma Campanha inteligente para o status/Programa bem-sucedido {#create-a-smart-campaign-for-status-program-success}

Você precisa de uma segunda campanha inteligente para alterar o status das pessoas, de modo que elas possam alcançar o sucesso do Programa e sejam incluídas nos cálculos de atribuição de receita.

1. No acionador **Preencher formulário** , insira o nome do programa na string do query. Se você estiver clonando o programa, substitua o nome da sequência de query antigo pelo novo.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Crie etapas de fluxo para alterar o status para um status associado ao sucesso do programa.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >O exemplo acima mostra **Converted, **mas isso depende de seus valores de status/sucesso.

1. Agende e ativa a campanha.

## Crie seu anúncio {#create-your-ad}

Depois de configurar o programa e o campanha, crie o novo anúncio.

1. Ir para o canal; Por exemplo, LinkedIn ou Facebook.
1. Crie um novo anúncio.
1. Selecione uma landing page de marketing como destino para a Ação de chamada na campanha.
1. Adicione a string de query ao URL.

   >[!NOTE]
   >
   >**Exemplo**
   >
   >
   >Veja como você pode adicionar todas as informações configuradas em um URL real. Os itens são separados por um E comercial (&amp;):
   >
   >
   >[www.marketo.com?**source**=Social-Paid&amp;**comment**=Social-Paid_Facebook_NewGuide_NA&amp;**camp**=abc&amp;**kk=**xyz](http://www.marketo.com?source=Social-Paid&amp;comment=Social-Paid_Facebook_NewGUide_NA&amp;camp=abc&amp;kk+xyz)
   >
   >    
   >    
   >    * **fonte** é a Fonte da Pessoa usada como um identificador de canal
   >    * **comment** é o identificador exclusivo criado para cada programa
   >    * **camp** é a campanha no Facebook, LinkedIn ou Google
   >    * **kk** é a palavra-chave ou o nome do ativo que você deseja capturar

   >    
   >    
   >**Esses quatro termos devem estar em minúsculas e não podem haver espaços no URL para que essas informações sejam capturadas.**

## Práticas recomendadas {#best-practices}

Use uma única tag de canal para representar toda a publicidade digital ou use várias tags de canal se desejar comparações mais granulares com seus outros canais de marketing (por exemplo, Social-Paid, Search-Paid, Exibir, Redirecionamento).

Em seguida, configure programas diferentes para cada visualização de relatórios necessária. Use uma ID comum como parâmetro no URL (BC, por exemplo) na sequência de query se você tiver 10 regiões iniciando uma &quot;Campanha grande&quot; juntas e quiser ser capaz de visualização dos resultados entre as regiões.

Se você quiser relatar cada região e os resultados coletivos da Grande Campanha, crie 11 programas, um para cada região e outro para a Grande Campanha. Cada programa faz referência apenas aos caracteres relevantes da string do query (como BC).

Há sobreposição intencional na contagem de pessoas entre a Grande Campanha e os programas da região, então você não gostaria de relatar a contagem total de pessoas em todos os 11 programas, como algumas pessoas estão tanto na Grande Campanha quanto em um dos programas da região.
