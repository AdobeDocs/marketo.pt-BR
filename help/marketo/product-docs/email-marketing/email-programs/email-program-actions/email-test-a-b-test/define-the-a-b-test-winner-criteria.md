---
unique-page-id: 2359545
description: Definir o critério do vencedor do teste A/B - Documentos da Marketo - Documentação do produto
title: Definir o critério do vencedor do teste A/B
exl-id: be8a0887-70f4-4667-93a6-d982a16cdfdb
source-git-commit: 67ae4605d541a475b42a5094a5588c469a9d975d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 3%

---

# Definir o critério do vencedor do teste A/B {#define-the-a-b-test-winner-criteria}

When [adição de um teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;} para o seu programa de email, você precisará escolher um tipo de teste, [agendar o teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}, então defina os critérios vencedores. Veja como decidir qual email ganha.

>[!PREREQUISITES]
>
>[Adicionar um teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md){target=&quot;_blank&quot;}

## Critérios vencedores {#winner-criteria}

1. O padrão **Critérios do vencedor** As opções são listadas primeiro.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   <table>
   <tr>
   <td><b>Abre</b></td>
   <td>Uma abertura é registrada quando imagens são baixadas em um email. Mesmo que você não inclua uma imagem, por padrão, o Marketo insere um único pixel de rastreamento em todos os emails do HTML.</td>
   </tr>
   <tr>
   <td><b>Cliques</b></td>
   <td>Por padrão, os links em emails têm rastreamento incorporado, permitindo ver quem clicou em qual link, quantos links totais foram clicados, etc.</td>
   </tr>
   <tr>
   <td><b>Clique para abrir %</b></td>
   <td>Porcentagem de emails que foram abertos e tiveram um link clicado no email. Isso mede a relevância e o contexto de um email, considerando o número de cliques únicos dividido pelo número de aberturas exclusivas e, em seguida, multiplicando por 100 para exibi-lo como uma porcentagem.</td>
   </tr>
   <tr>
   <td><b>Pontuação de envolvimento</b></td>
   <td>O <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.html" target="_blank">pontuação de engajamento</a> O ajuda a determinar a eficácia do conteúdo.</td>
   </tr>
   </table>

   >[!TIP]
   >
   >Se você escolher Pontuação de engajamento , o teste precisará ser executado por pelo menos 24 horas. Saiba mais sobre [noções básicas sobre a pontuação de engajamento](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target=&quot;_blank&quot;}.

1. Você também pode personalizar seus critérios selecionando Conversão personalizada e clicando em Editar.

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >A Conversão personalizada permite selecionar qualquer evento como conversão usando acionadores e filtros.

1. Uma janela aparecerá. Encontre o acionador de sua escolha e arraste-o para a tela.

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. Defina o acionador.

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!IMPORTANT]
   >
   >O Marketo permite somente acionadores/filtros para pessoas que receberam o email deste programa de email; portanto, não há necessidade de adicionar um filtro &quot;Foi enviado por email&quot;. Além disso, ao usar um acionador/filtro relacionado a email, certifique-se de usar &quot;é qualquer&quot; como operador.

1. Clique em **Fechar**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Ótimo! Agora é hora de decidir como o vencedor é determinado.

## Declarar vencedor {#declare-winner}

1. Escolha uma das duas opções disponíveis.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Se você estiver fazendo uma **Data/Hora** Teste A/B, você só pode escolher **Manual**.

   Quando o teste A/B terminar, o Marketo poderá enviar automaticamente o email vencedor no horário agendado, ou você poderá revisar os resultados e decidir qual email sai quando.

1. Automatic é incrível e é a opção padrão. Basta clicar em **Próximo**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Escolha **Manual** O enviará o teste e aguardará que você declare um vencedor. Você receberá um relatório dos resultados.

Perfeita! Agora vamos [agendar o teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md){target=&quot;_blank&quot;}.
