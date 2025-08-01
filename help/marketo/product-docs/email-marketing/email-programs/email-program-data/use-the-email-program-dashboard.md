---
unique-page-id: 2359476
description: Use o painel do programa de email - Documentação do Marketo - Documentação do produto
title: Usar o painel do programa de email
exl-id: 47c1925a-144b-4277-a08d-1af660ed3d50
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Usar o painel do programa de email {#use-the-email-program-dashboard}

Confira o desempenho de seus programas de email com essa exibição de painel.

>[!CAUTION]
>
>Para obter relatórios precisos, evite _reutilizar_ um email de um programa de email referenciando-o em uma Campanha Inteligente ou movendo o ativo do programa de email iniciado para um novo. Isso agregará todos os dados em cada painel de relatórios anexado a esse email. Se você precisar reutilizar um email, [clone-o](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/clone-an-asset-in-a-program.md){target="_blank"}, pois ele copia o email, mas cria um novo com uma nova ID.

>[!NOTE]
>
>Se o seu programa tiver um teste A/B, confira o [Painel do Programa de Email - Exibição de Teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}.

![](assets/image2014-9-12-14-3a12-3a56.png)

>[!NOTE]
>
>Todos os dados nessa visualização são agregados (incluem o teste A/B, bem como o envio final de email).

## Enviar por e-mail {#email-send}

Aqui você pode ver quantos emails foram enviados, devolvidos e entregues.

![](assets/image2014-9-12-14-3a13-3a3.png)

>[!NOTE]
>
>Devido aos padrões de capacidade de entrega de email que estão fora do controle da Marketo, as estatísticas Devolvidas e Devolvidas são aproximadas, não exatas.

## Aberturas/Cliques {#opens-clicks}

Este gráfico mostra o número de emails abertos/clicados durante períodos específicos após a execução do programa de email.

![](assets/image2014-9-12-14-3a13-3a7.png)

>[!TIP]
>
>Observe como o número de aberturas/cliques diminui com o passar do tempo.

## Resumo - Participação {#summary-engagement}

Isto mostra a você a [pontuação geral do engajamento](/help/marketo/product-docs/email-marketing/drip-nurturing/reports-and-notifications/understanding-the-engagement-score.md){target="_blank"}.

![](assets/image2014-9-12-14-3a13-3a11.png)

## Resumo - Restante {#summary-rest}

O restante dos dados exibirá Opens, Clicks, Click/Open Ratio e Unsubscribes.

![](assets/image2014-9-12-14-3a13-3a15.png)

>[!TIP]
>
>A taxa de **Cancelamento de inscrição** no exemplo acima era tão pequena que o Marketo ampliou para dar a você uma melhor aparência. O segundo número dentro da barra é apenas adicionado para escala.

>[!NOTE]
>
>**Definição**
>
>**[!UICONTROL Aberturas]** são contadas quando o destinatário do email baixa as imagens do email, o que inclui um pixel de rastreamento inserido pela Marketo. Se o recipient visualizar o email, mas optar por não baixar as imagens, isso não contará como uma abertura. Se as imagens forem carregadas no painel de visualização do recipient, isso geralmente contará como uma abertura, mas variará com base no cliente de email.
>
>**[!UICONTROL Clicar para Abrir]** mede a porcentagem de emails que foram abertos e tiveram um link clicado no email. Pegamos o número de cliques únicos dividido pelo número de aberturas únicas e, em seguida, multiplicamos por 100 para mostrá-lo como uma porcentagem.

## Atualizar painel {#refresh-dashboard}

Para ver os dados mais atualizados, basta clicar no ícone de atualização no painel.

![](assets/refreshicon.png)

>[!MORELIKETHIS]
>
>[Usar o Painel do Programa de Email - Modo de Exibição de Teste A/B](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/use-the-email-program-dashboard-a-b-test-view.md){target="_blank"}
