---
unique-page-id: 10098812
description: Configurar atribuição de receita para campanhas de publicidade digital – documentos do Marketo – Documentação do produto
title: Configurar atribuição de receita para campanhas de publicidade digital
exl-id: 7fb16c5f-7e76-429b-8b01-b5a1dd898158
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Configurar atribuição de receita para campanhas de publicidade digital {#set-up-revenue-attribution-for-digital-advertising-campaigns}

Veja como configurar a atribuição de receita para campanhas e canais de publicidade digitais. Depois de configurá-lo, você pode fazer receita atribuição de primeiro e multi toque para anúncios digitais da mesma forma que em outros programas da Marketo.

>[!IMPORTANT]
>
>Em 31 de julho de 2024, começamos o processo de descontinuação desse recurso. Você não poderá criar novas ativos. A ativos continuará a funcionar até 31 de janeiro de 2025. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Depois de configurar seu primeiro publicidade programa no Marketo, você pode clonar e atualizá-lo para outros canais. Por exemplo, clonar um programa do LinkedIn em um site do Facebook.

Com programas separados, você pode faixa o número de conversões de cada um e ver seus programas no Analisador de Programas, Analisador de Influência de Oportunidades e outros recursos do Marketo Analytics.

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
   >Um sequência de consulta passado pela URL ajuda a Marketo a saber quais campanha publicitária alguém clicou quando se tornou uma pessoa no Marketo.
   >
   >É possível criar uma sequência de consulta metodologia que inclua todas as variáveis que deseja medir. A Marketo usa essas variáveis para adicionar pessoas aos seus diferentes programas.
   >
   >Por exemplo, você pode usar a type_Channel__Asset__Region de Canal. Pode ser semelhante a: SP_FB_NewGuide_US. **Observação**: abreviações economizam espaço.
   >
   >Ou configure-o como Channel_Adsource_AssetName_Region_UniqueIdNumber. Isso pode parecer curtir: Paid_Facebook_NewGuide_NA_123 com Social.

## Criar uma Campaign inteligente para nomes de Novo {#create-a-smart-campaign-for-new-names}

1. Na campanha inteligente, crie uma lista inteligente que contenha dois acionadores e dois filtros, como mostrado.

   ![](assets/image2016-3-23-13-3a59-3a24.png)

   >[!NOTE]
   >
   >O sequência de consulta usado nos dois acionadores e o **filtro Programa que Capturou Nome** é exclusivo para você. As sequências de caracteres do query mostradas aqui são, por exemplo, apenas. Se você clonou o campo, basta substituir esses campos.

1. Criar uma etapa de fluxo para alterar o atributo para **o Programa** de aquisição e definir o Novo Valor para o valor que você definiu para o campanhas sociais pago.

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
1. Criar um novo publicidade.
1. Selecione um landing page do Marketo como destino da Frase de chamariz no campanha.
1. Adicione a sequência de consulta ao URL.

   >[!NOTE]
   >
   >**Exemplo**
   >
   >Veja como adicionar todas as informações configuradas em um URL real. Os itens são separados por um E comercial (&amp;):
   >
   >`www.marketo.com?**source**=Social-Paid&**comment**=Social-Paid_Facebook_NewGuide_NA&**camp**=abc&**kk=**xyz`
   >
   >* **source** é a Pessoa Origem usada como um identificador canal
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
