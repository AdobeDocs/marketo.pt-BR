---
description: Filtrar atividade de bot de email - Documentos do Marketo - Documentação do produto
title: Filtrar atividade de bot de email
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: a64c499f6972e94adfecbe164d86f7db1b1447aa
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Filtrar atividade de bot de email {#filtering-email-bot-activity}

Às vezes, a atividade de bot de email pode aumentar erroneamente seus dados de aberturas e cliques de email. Veja como consertar isso.

>[!NOTE]
>
>Usar o [Lista internacional de spiders e bots da IAB/ABC](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/), toda a atividade de abertura/clique com um IP ou agente do usuário que corresponde a qualquer item dessa lista será identificada como atividade de bot e não será registrada no Marketo.

1. Clique em **Administrador**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Clique em **Email**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Clique no botão **Atividade de bot** guia .

   ![](assets/filtering-email-bot-activity-3.png)

1. Clique no controle deslizante para ativar **Filtrar atividade de bot**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Você pode escolher separadamente se deseja ou não ter a atividade de bot registrada. Se você optar por não fazer isso, poderá observar uma queda na abertura e no clique do email, pois números falsos são filtrados.

**ETAPA OPCIONAL**: Para desativar o recurso, basta desmarcar o controle deslizante. Se você desativar, os dados de &quot;Atividade do robô nos últimos 90 dias&quot; funcionarão **not** redefinir.

>[!TIP]
>
>Aproveite os dados da atividade de bot nas Smart Lists por meio do booleano &quot;Is Bot Activity&quot; (sim/não) ou nas restrições aplicáveis de filtro/acionador.
