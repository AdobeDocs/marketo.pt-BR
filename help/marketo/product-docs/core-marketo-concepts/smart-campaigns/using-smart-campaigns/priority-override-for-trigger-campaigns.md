---
description: Substituição prioritária de campanhas de acionador - Documentos do Marketo - Documentação do produto
title: Substituição de prioridade para campanhas do acionador
hide: true
hidefromtoc: true
source-git-commit: f2b6e0ae4759ed279d4c02ae922e9deba838b1ff
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Substituição de prioridade para campanhas do acionador {#priority-override-for-trigger-campaigns}

Os administradores podem substituir a prioridade determinada do Marketo para acionar campanhas a fim de definir prioridades que estejam mais alinhadas aos objetivos de negócios.

>[!NOTE]
>
>Esse recurso está disponível somente para campanhas do acionador e para usuários que receberam a variável [Permissão &quot;Editar prioridade de campanha do acionador&quot;](#grant-priority-override-access).

>[!CAUTION]
>
>É altamente recomendável usar esse recurso em um conjunto limitado de campanhas críticas para os negócios (25 é o máximo recomendado). O uso do recurso vagamente em um conjunto grande pode afetar negativamente a execução geral da campanha.

## Conceder Acesso de Substituição de Prioridade {#grant-priority-override-access}

>[!CAUTION]
>
>Somente administradores ou usuários com responsabilidades de administrador devem ter acesso de substituição de prioridade de campanha.

1. No [!UICONTROL Administrador] , clique em **[!UICONTROL Usuários e funções]**.

   ![](assets/priority-override-for-trigger-campaigns-1.png)

1. Clique no botão **[!UICONTROL Funções]** , selecione o usuário ao qual deseja conceder acesso e clique em **[!UICONTROL Editar função]**.

   ![](assets/priority-override-for-trigger-campaigns-2.png)

1. Em [!UICONTROL Acessar atividades de marketing], selecione **[!UICONTROL Editar prioridade de campanha do acionador]**. Clique em **[!UICONTROL Salvar]**.

   ![](assets/priority-override-for-trigger-campaigns-3.png)

## Substituir prioridade {#override-priority}

1. Localize sua campanha do acionador. Clique com o botão direito do mouse e selecione **[!UICONTROL Substituir prioridade da campanha]**.

   ![](assets/priority-override-for-trigger-campaigns-4.png)

1. Clique no botão **[!UICONTROL Substituir prioridade da campanha]** controle deslizante para ativar. Escolha um novo nível de prioridade e clique em **[!UICONTROL Confirmar]**.

   ![](assets/priority-override-for-trigger-campaigns-5.png)

   O novo nível de prioridade será exibido na guia Schedule .

   ![](assets/priority-override-for-trigger-campaigns-6.png)

>[!NOTE]
>
>* Você pode visualizar a prioridade padrão da campanha no [!UICONTROL Fila de Campanha] under [!UICONTROL Atividades de marketing]. Para aumentar a taxa de execução, recomendamos configurar a prioridade da campanha para um nível superior ao padrão.
>* A prioridade do conjunto de usuários se aplica somente a novas pessoas que se qualificam para a campanha; as pessoas que já estão na fila não serão afetadas.
>* As substituições de prioridade são capturadas em [Trilha de auditoria](/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md).

