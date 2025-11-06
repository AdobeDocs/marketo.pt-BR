---
unique-page-id: 2359545
description: Defina os critérios do vencedor do teste A/B - Documentação do Marketo - Documentação do produto
title: Definir os critérios do vencedor do teste A/B
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
feature: Email Programs, A/B Testing
source-git-commit: c80d25aeafe2314fcff1d99359ff146c88acad06
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 21%

---

# Definir os critérios do vencedor do teste A/B {#define-the-a-b-test-winner-criteria}

Ao [adicionar um teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"} ao seu programa de email, você precisará escolher um tipo de teste, [agendar o teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"} e definir os critérios vencedores. Veja como decidir qual email vence.

>[!PREREQUISITES]
>
>[Adicionar um teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target="_blank"}

## Critérios vencedores {#winner-criteria}

1. As opções padrão de **[!UICONTROL Critério de vencedor]** são listadas primeiro.

   ![](assets/define-the-a-b-test-winner-criteria-1.png)

   <table>
   <tr>
   <td><b>[!UICONTROL Abre]</b></td>
   <td>Uma página aberta é registrada quando imagens são baixadas em um email. Mesmo que você não inclua uma imagem, por padrão, o Marketo insere um único pixel de rastreamento em todos os emails do HTML.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Cliques]</b></td>
   <td>Por padrão, os links nos emails têm rastreamento incorporado, permitindo ver quem clicou em qual link, quantos links foram clicados no total etc.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Clicar para Abrir] %</b></td>
   <td>Porcentagem de emails que foram abertos e tiveram um link clicado. Isso mede a relevância e o contexto de um email considerando o número de cliques únicos dividido pelo número de aberturas únicas e multiplicando por 100 para mostrá-lo como uma porcentagem.</td>
   </tr>
   <tr>
   <td><b>[!UICONTROL Pontuação de Envolvimento]</b></td>
   <td>A <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">pontuação de engajamento</a> ajuda a determinar a eficácia do conteúdo.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Se você escolher Pontuação de engajamento, o teste precisará ser executado por pelo menos 24 horas. Saiba mais sobre [como entender a pontuação do engajamento](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

1. Você também pode personalizar seus critérios selecionando **[!UICONTROL Conversão personalizada]** e clicando em **[!UICONTROL Editar]**.

   ![](assets/define-the-a-b-test-winner-criteria-2.png)

   >[!NOTE]
   >
   >A Conversão personalizada permite escolher qualquer evento como uma conversão usando acionadores e filtros.

1. Uma janela é aberta. Encontre o acionador de sua escolha e arraste-o para a tela.

   ![](assets/define-the-a-b-test-winner-criteria-3.png)

1. Defina o acionador.

   ![](assets/define-the-a-b-test-winner-criteria-4.png)

   >[!IMPORTANT]
   >
   >O Marketo permite acionadores/filtros apenas para pessoas que receberam o email deste programa de email, portanto, não há necessidade de adicionar um filtro &quot;E-mail enviado&quot;. Além disso, ao usar um acionador/filtro relacionado ao email, certifique-se de usar &quot;is any&quot; como operador.

1. Feche a nova janela (ou guia) que foi aberta. A Smart List é salva automaticamente.

Agora é hora de decidir como o vencedor é determinado.

## Declarar vencedor {#declare-winner}

1. Escolha uma das duas opções disponíveis.

   ![](assets/define-the-a-b-test-winner-criteria-5.png)

   >[!NOTE]
   >
   >Se você estiver fazendo um teste A/B de **Data/Hora**, poderá escolher somente **[!UICONTROL Manual]**.

   Depois que o teste A/B for concluído, o Marketo poderá enviar automaticamente o email vencedor no horário agendado ou você poderá analisar os resultados e decidir qual email será enviado quando.

1. Automático é o máximo e é a opção padrão. Basta clicar em **[!UICONTROL Avançar]**.

   ![](assets/define-the-a-b-test-winner-criteria-6.png)

   >[!TIP]
   >
   >Escolher **[!UICONTROL Manual]** enviará o teste e aguardará você declarar um vencedor. Você receberá um relatório dos resultados.

Agora vamos [agendar o teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target="_blank"}.
