---
unique-page-id: 10098812
description: Configurar atribuição de receita para campanhas do Digital Advertising - Documentação do Marketo - Documentação do produto
title: Configurar atribuição de receita para campanhas do Digital Advertising
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Configurar atribuição de receita para campanhas do Digital Advertising {#set-up-revenue-attribution-for-digital-advertising-campaigns}

Veja como configurar a atribuição de receita para campanhas e canais de publicidade digitais. Depois de configurá-lo, você pode fazer a atribuição de receita de primeiro e de multitoque para anúncios digitais da mesma forma que em outros programas da Marketo.

Depois de configurar seu primeiro programa de publicidade no Marketo, você pode cloná-lo e atualizá-lo para outros canais. Por exemplo, clone um programa LinkedIn em um Facebook.

Com programas separados, você pode rastrear o número de conversões de cada um e ver seus programas no Analisador de programas, no Analisador de influência de oportunidades e em outros recursos do Marketo Analytics.

>[!PREREQUISITES]
>
>* Configurar uma tag de canal com valores de status e sucesso do programa (por exemplo, Advertising digital ou Social Paid e PPC)
>* Criar ou editar um formulário para passar uma sequência de consulta com a pessoa
>* Certifique-se de ter acesso a alguns recursos do Revenue Cycle Analytics para criar relatórios sobre seus canais e campanhas de publicidade

## Criar um programa padrão {#create-a-default-program}

Ao contrário de alguns programas (como email) que podem ser executados periodicamente por um período específico, os programas padrão estão sempre ativos.

1. Vá para **Atividades de marketing**.

   ![](assets/login-marketing-activities-5.png)

1. Clique em **Novo** e selecione **Novo programa**.

   ![](assets/image2016-3-14-15-52-0.png)

1. Se você já tiver um programa em vigor, poderá [cloná-lo](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-a-program.md).

   >[!TIP]
   >
   >Sempre que você clonar um programa, substitua os nomes nos campos de sequência de consulta das smart lists.

1. Coloque o novo programa em uma pasta de campanha específica, após a definição do programa inicial.

   >[!NOTE]
   >
   >**Exemplo**
   >
   >Uma sequência de consulta transmitida pelo URL ajuda a Marketo a saber em qual campanha de publicidade alguém clicou quando se tornou uma pessoa no Marketo.
   >
   >Você pode criar uma metodologia de sequência de consulta que inclua todas as variáveis que deseja medir. O Marketo usa essas variáveis para adicionar pessoas aos seus diferentes programas.
   >
   >Por exemplo, você pode usar Canal type_Channel_Asset_Region. Pode ser semelhante a: SP_FB_NewGuide_US. **Observação**: abreviações economizam espaço.
   >
   >Ou configure-o como Channel_Adsource_AssetName_Region_UniqueIdNumber. Pode ser semelhante a: Social-Paid_Facebook_NewGuide_NA_123.

## Criar uma campanha inteligente para novos nomes {#create-a-smart-campaign-for-new-names}

1. Na campanha inteligente, crie uma lista inteligente que contenha dois acionadores e dois filtros, conforme mostrado.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >A cadeia de caracteres de consulta usada nos dois disparadores e no filtro **Nome do Programa que Capturou** é exclusiva para você. As cadeias de caracteres de consulta mostradas aqui são somente para fins de exemplo. Se você clonou o campo, basta substituir esses campos.

1. Crie uma etapa de fluxo para alterar o atributo para **Programa de aquisição** e defina o Novo valor para o valor definido para campanhas sociais pagas.

   ![](assets/image2016-3-14-14-3a58-3a6.png)

1. Agende e ative a campanha.

## Criar uma campanha inteligente para obter status/sucesso do programa {#create-a-smart-campaign-for-status-program-success}

Você precisa de uma segunda campanha inteligente para alterar o status das pessoas, para que elas possam alcançar o sucesso do programa e serem incluídas nos cálculos de atribuição de receita.

1. No acionador **Preencher Formulário**, digite o nome do programa na cadeia de caracteres de consulta. Se estiver clonando o programa, basta substituir o nome da sequência de consulta antiga pelo novo.

   ![](assets/image2016-3-23-14-3a7-3a20.png)

1. Crie etapas de fluxo para alterar o status para um associado ao sucesso do programa.

   ![](assets/image2016-3-14-15-3a9-3a29.png)

   >[!NOTE]
   >
   >O exemplo acima mostra **Convertido**, mas isso depende de seus valores de status/sucesso.

1. Agende e ative a campanha.

## Crie seu anúncio {#create-your-ad}

Depois de configurar o programa e as campanhas, crie o novo anúncio.

1. Vá para o canal; por exemplo, LinkedIn ou Facebook.
1. Crie um novo anúncio.
1. Selecione uma landing page do Marketo como destino da Chamada para ação na campanha.
1. Adicione a cadeia de caracteres de consulta ao URL.

   >[!NOTE]
   >
   >**Exemplo**
   >
   >Veja como adicionar todas as informações configuradas em um URL real. Os itens são separados por um E comercial (&amp;):
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **origem** é a Pessoa Source usada como um identificador de canal
   >* **comentário** é o identificador exclusivo criado para cada programa
   >* **camp** é a campanha no Facebook, LinkedIn ou Google
   >* **kk** é a palavra-chave ou o nome do ativo que você deseja capturar
   >
   >**Todos esses quatro termos devem estar em minúsculas e não pode haver nenhum espaço na URL para que essas informações sejam capturadas.**

## Práticas recomendadas {#best-practices}

Use uma única tag de canal para representar toda a Advertising digital ou use várias tags de canal se desejar comparações mais granulares com outros canais de marketing (por exemplo, Social-Pago, Pesquisa-Paga, Exibição, Redirecionamento).

Em seguida, configure programas diferentes para cada exibição de relatório necessária. Use uma ID comum como parâmetro no URL (BC, por exemplo) na string de consulta se você tiver 10 regiões iniciando uma &quot;Campanha grande&quot; juntas e quiser ver os resultados nas regiões.

Se quiser relatar cada região e os resultados coletivos da Campanha Grande, crie 11 programas, um para cada região e um para a Campanha Grande. Cada programa faz referência apenas aos caracteres relevantes da sequência de consulta (como BC).

Há uma sobreposição intencional na contagem de pessoas entre o Big Campaign e os programas da região, portanto, você não gostaria de relatar a contagem total de pessoas em todos os 11 programas, pois algumas pessoas estão tanto no Big Campaign quanto em um dos programas da região.
