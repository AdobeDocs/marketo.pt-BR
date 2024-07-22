---
description: Substituição de prioridade para campanhas do acionador - Documentação do Marketo - Documentação do produto
title: Substituição de prioridade para campanhas do acionador
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 1%

---

# Substituição de prioridade para campanhas do acionador {#priority-override-for-trigger-campaigns}

Os administradores podem substituir a prioridade determinada de Marketo Engage para que as Campanhas de acionador definam prioridades que se alinhem melhor aos objetivos de negócios.

>[!NOTE]
>
>Este recurso só está disponível para Campanhas de Gatilho e para usuários que receberam a [ permissão &quot;Editar Prioridade de Campanha de Gatilho&quot;](#grant-priority-override-access).

>[!CAUTION]
>
>É extremamente recomendável usar esse recurso em um conjunto limitado de campanhas críticas para os negócios (25 é o máximo recomendado). Usar o recurso livremente em um conjunto grande pode afetar negativamente a execução geral da campanha.

## Conceder acesso de substituição de prioridade {#grant-priority-override-access}

>[!NOTE]
>
>Somente administradores ou usuários com responsabilidades de administrador devem ter acesso de substituição de prioridade de campanha.

1. Na área [!UICONTROL Administrador], clique em **[!UICONTROL Usuários e funções]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Clique na guia **[!UICONTROL Funções]**, selecione o usuário ao qual deseja conceder acesso e clique em **[!UICONTROL Editar Função]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. Em [!UICONTROL Acessar Atividades de Marketing], selecione **[!UICONTROL Editar Prioridade de Campanha do Gatilho]**. Clique em **[!UICONTROL Salvar]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Substituir prioridade {#override-priority}

1. Localize seu Trigger Campaign. Clique com o botão direito do mouse e selecione **[!UICONTROL Substituir Prioridade de Campanha]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Clique no controle deslizante **[!UICONTROL Substituir prioridade da campanha]** para habilitar. Escolha um novo nível de prioridade e clique em **[!UICONTROL Confirmar]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   O novo nível de prioridade será exibido na guia Schedule.

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Você pode exibir a prioridade padrão da sua campanha na [!UICONTROL Fila de campanha] em [!UICONTROL Atividades de marketing]. Para aumentar a taxa de execução, recomendamos definir a prioridade da campanha para um nível superior ao padrão.
>* A prioridade definida pelo usuário se aplica somente a novas pessoas que se qualificam para a campanha; as pessoas que já estão na fila não serão afetadas.
>* As substituições de prioridade são capturadas em [Trilha de Auditoria](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md){target="_blank"}.
