---
unique-page-id: 2359545
description: Defina o critério do vencedor do teste A/B - Documentos do marketing - Documentação do produto
title: Definir o critério do vencedor do teste A/B
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 0%

---


# Defina o Critério do vencedor do teste A/B {#define-the-a-b-test-winner-criteria}

Quando [adicionar um teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md) ao seu programa de correio eletrônico, terá de selecionar um tipo de teste, [agendar o teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md) e definir os critérios vencedores. Aqui está como decidir qual e-mail vence.

>[!PREREQUISITES]
>
>[Adicionar um teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/add-an-a-b-test.md)

## Critérios de vencedor {#winner-criteria}

1. As opções padrão **Critérios do Vencedor** são listadas primeiro.

   ![](assets/image2014-9-12-15-3a51-3a3.png)

   | **Abre** | Uma opção aberta é registrada quando as imagens são baixadas em um email. Mesmo se você não incluir uma imagem, por padrão, o Marketo insere um único pixel de rastreamento em todos os emails HTML. |
   |---|---|
   | **Cliques** | Por padrão, os links em emails têm rastreamento incorporado, permitindo que você veja quem clicou em qual link, quantos links totais foram clicados etc. |
   | **Clique para Abrir %** | Porcentagem de emails que foram abertos e tiveram um link clicado no email. Isso mede a relevância e o contexto de um email, considerando o número de cliques únicos dividido pelo número de aberturas exclusivas e, em seguida, multiplicando por 100 para exibi-lo como uma porcentagem. |
   | **Pontuação de envolvimento** | A [pontuação de envolvimento](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md) ajuda a determinar a eficácia do seu conteúdo. |

   >[!TIP]
   >
   >Se você escolher Pontuação de envolvimento, o teste precisará ser executado por pelo menos 24 horas. Saiba mais sobre [como entender a pontuação de envolvimento](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md).

1. Você também pode personalizar seus critérios selecionando Conversão personalizada e clicando em Editar.

   ![](assets/image2014-9-12-15-3a51-3a53.png)

   >[!NOTE]
   >
   >A Conversão personalizada permite que você escolha qualquer evento como conversão usando filtros e acionadores.

1. Uma janela aparecerá. Encontre o acionador de sua escolha e arraste-o para a tela.

   ![](assets/image2014-9-12-15-3a52-3a18.png)

1. Defina o acionador.

   ![](assets/image2014-9-12-15-3a53-3a11.png)

   >[!NOTE]
   >
   >O Marketo só permitirá acionadores para pessoas que receberam o email deste programa de email. Não é necessário adicionar um filtro &quot;Foi Enviado por email&quot;.

1. Clique em **Fechar**.

   ![](assets/image2014-9-12-15-3a53-3a36.png)

   Ótimo! Agora é hora de decidir como o vencedor é determinado.

## Declarar vencedor {#declare-winner}

1. Escolha uma das duas opções disponíveis.

   ![](assets/image2014-9-12-15-3a53-3a44.png)

   >[!NOTE]
   >
   >Se estiver fazendo um teste A/B **Date/Time**, você só poderá escolher **Manual**.

   Quando o teste A/B terminar, o Marketo poderá enviar automaticamente o email vencedor no horário agendado, ou você poderá revisar os resultados e decidir qual email será enviado quando.

1. Automático é incrível e é a opção padrão. Basta clicar em **Next**.

   ![](assets/image2014-9-12-15-3a54-3a35.png)

   >[!TIP]
   >
   >Escolher **Manual** enviará o teste e aguardará que você declare um vencedor. Você receberá um relatório dos resultados.

Perfeito! Agora vamos [agendar o teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/schedule-the-a-b-test.md).
