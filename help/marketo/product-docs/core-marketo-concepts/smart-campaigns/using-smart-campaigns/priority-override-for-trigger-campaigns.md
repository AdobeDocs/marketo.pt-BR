---
description: Substituição de prioridade para campanhas do acionador - Documentação do Marketo - Documentação do produto
title: Substituição de prioridade para campanhas do acionador
exl-id: cf9b4d27-0e4c-40cf-accd-4f4a102160cc
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 8%

---

# Substituição de prioridade para campanhas do acionador {#priority-override-for-trigger-campaigns}

Os administradores podem substituir a prioridade determinada pelo Marketo para acionar campanhas definindo prioridades que melhor se alinhem com os objetivos do negócio.

>[!NOTE]
>
>Esse recurso só está disponível para campanhas de acionador e para usuários que receberam a permissão [Permissão &quot;Editar Prioridade de Campanha do Acionador&quot;](#grant-priority-override-access).

>[!CAUTION]
>
>É extremamente recomendável usar esse recurso em um conjunto limitado de campanhas críticas para os negócios (25 é o máximo recomendado). Usar o recurso livremente em um conjunto grande pode afetar negativamente a execução geral da campanha.

## Conceder acesso de substituição de prioridade {#grant-priority-override-access}

>[!NOTE]
>
>Somente administradores ou usuários com responsabilidades de administrador devem ter acesso de substituição de prioridade de campanha.

1. No [!UICONTROL Admin] clique em **[!UICONTROL Usuários e funções]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Clique em **[!UICONTROL Funções]** selecione o usuário ao qual deseja conceder acesso e clique em **[!UICONTROL Editar Função]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. Em [!UICONTROL Acessar atividades de marketing], selecione **[!UICONTROL Editar Prioridade de Campanha do Acionador]**. Clique em **[!UICONTROL Salvar]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Substituir prioridade {#override-priority}

1. Localize sua campanha de acionadores. Clique com o botão direito do mouse e selecione **[!UICONTROL Substituir prioridade da campanha]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Clique em **[!UICONTROL Substituir prioridade da campanha]** controle deslizante para ativar. Escolha um novo nível de prioridade e clique em **[!UICONTROL Confirmar o]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   O novo nível de prioridade será exibido na guia Schedule.

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Você pode visualizar a prioridade padrão da sua campanha no [!UICONTROL Fila de campanha] em [!UICONTROL Atividades de marketing]. Para aumentar a taxa de execução, recomendamos definir a prioridade da campanha para um nível superior ao padrão.
>* A prioridade definida pelo usuário se aplica somente a novas pessoas que se qualificam para a campanha; as pessoas que já estão na fila não serão afetadas.
>* As sobreposições de prioridade são capturadas em [Trilha de auditoria](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md).
