---
unique-page-id: 10098812
description: Configurar atribuição de receita para campanhas de publicidade digital - Documentos do Marketo - Documentação do produto
title: Configurar atribuição de receita para campanhas de publicidade digital
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---

# Configurar atribuição de receita para campanhas de publicidade digital {#set-up-revenue-attribution-for-digital-advertising-campaigns}

Veja como configurar a atribuição de receita para canais e campanhas de publicidade digital. Depois de configurá-lo, você pode fazer atribuição de receita de primeiro e multitoque para anúncios digitais da mesma forma que em outros programas Marketo.

Após configurar seu primeiro programa de publicidade no Marketo, é possível cloná-lo e atualizá-lo para outros canais. Por exemplo, clonar um programa do LinkedIn para um Facebook.

Com programas separados, você pode acompanhar o número de conversões de cada um e ver seus programas no Analisador de programas, no Analisador de influência de oportunidades e em outros recursos do Marketo Analytics.

>[!PREREQUISITES]
>
>* Configure uma tag de canal com valores de status e sucesso de programa (por exemplo, Digital Advertising ou Social Paid e PPC)
>* Criar ou editar um formulário para passar uma sequência de consulta com a pessoa
>* Certifique-se de ter acesso a alguns recursos do Revenue Cycle Analytics para criar relatórios sobre seus canais e campanhas de anúncios


## Criar um programa padrão {#create-a-default-program}

Ao contrário de alguns programas (como email) que podem ser executados periodicamente por um período específico, os programas padrão estão sempre ativados.

1. Ir para **Atividades de marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Clique em **Novo** e selecione **Novo programa**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Se você já tiver um programa em vigor, poderá [clonar](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Sempre que clonar um programa, certifique-se de substituir os nomes dos campos da sequência de consulta das listas inteligentes.

1. Coloque o novo programa em uma pasta de campanha específica, depois que o programa inicial for definido.

   >[!NOTE]
   >
   >**Exemplo**
   >
   >Uma sequência de consulta transmitida pelo URL ajuda a Marketo a saber em qual campanha publicitária alguém clicou quando se tornou uma pessoa no Marketo.
   >
   >Você pode criar uma metodologia de sequência de consulta que inclua todas as variáveis que deseja medir. O Marketo usa essas variáveis para adicionar pessoas a seus diferentes programas.
   >
   >Por exemplo, você pode usar Channel type_Channel_Asset__Region. Isso pode parecer: SP_FB_NewGuide_US. **Observação**: abreviações economizam espaço.
   >
   >Ou configure-a como Channel_Adsource_AssetName_Region_UniqueIdNumber. Isso pode parecer: Social-Paid_Facebook_NewGuide_NA_123.

## Criar uma campanha inteligente para novos nomes {#create-a-smart-campaign-for-new-names}

1. Na campanha inteligente, crie uma lista inteligente que contenha dois acionadores e dois filtros, como mostrado.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >A string de consulta usada nos dois acionadores e a variável **Programa que capturou o nome** O filtro é exclusivo para você. As cadeias de caracteres de consulta mostradas aqui são, por exemplo, apenas. Se você tiver clonado o campo, basta substituir esses campos.

1. Crie uma etapa de fluxo para alterar o atributo para **Programa de aquisição** e defina o Novo valor como o valor definido para campanhas sociais pagas.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Programe e ative a campanha.

## Criar uma campanha inteligente para o status/sucesso do programa {#create-a-smart-campaign-for-status-program-success}

Você precisa de uma segunda campanha inteligente para alterar o status das pessoas, para que elas possam alcançar o sucesso do programa e ser incluídas nos cálculos de atribuição de receita.

1. No **Preenche Formulário** , insira o nome do programa na sequência de caracteres de consulta. Se você estiver clonando o programa, basta substituir o nome da sequência de consulta antiga pelo novo.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Crie etapas de fluxo para alterar o status para um associado ao sucesso do programa.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >O exemplo acima mostra **Convertido**, mas depende do status/dos valores de sucesso.

1. Programe e ative a campanha.

## Crie seu anúncio {#create-your-ad}

Depois de configurar o programa e as campanhas, crie o novo anúncio.

1. Ir para o canal; Por exemplo, LinkedIn ou Facebook.
1. Crie uma nova publicidade.
1. Selecione uma página de aterrissagem do Marketo como destino para a Ação de chamada na campanha.
1. Adicione a string de consulta ao URL.

   >[!NOTE]
   >
   >**Exemplo**
   >
   >Veja como adicionar todas as informações configuradas em um URL real. Os itens são separados por um E comercial (&amp;):
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** é a fonte de pessoa usada como um identificador de canal
   >* **comentário** é o identificador exclusivo criado para cada programa
   >* **acampamento** é a campanha no Facebook, LinkedIn ou Google
   >* **kk** é a palavra-chave ou o nome do ativo que você deseja capturar

   >
   >**Esses quatro termos devem estar em minúsculas e não pode haver espaços no URL para que essas informações sejam capturadas.**

## Práticas recomendadas {#best-practices}

Use uma única tag de canal para representar toda a Publicidade digital ou use várias tags de canal se desejar comparações mais granulares com seus outros canais de marketing (por exemplo, Social-Paid, Pesquisa-Paga, Exibição, Redirecionamento).

Em seguida, configure programas diferentes para cada exibição de relatório necessária. Use uma ID comum como parâmetro no URL (BC, por exemplo) na sequência de consulta, se você tiver 10 regiões iniciando uma &quot;Campanha grande&quot; juntas e quiser visualizar os resultados em todas as regiões.

Se quiser relatar cada região e os resultados coletivos da Grande Campanha, crie 11 programas, um para cada região e um para a Grande Campanha. Cada programa faz referência apenas aos caracteres relevantes da sequência de consulta (como BC).

Há uma sobreposição intencional na contagem de pessoas entre o Big Campaign e os programas da região, então você não gostaria de relatar a contagem total de pessoas em todos os 11 programas, como algumas pessoas estão tanto no Big Campaign quanto em um dos programas da região.
