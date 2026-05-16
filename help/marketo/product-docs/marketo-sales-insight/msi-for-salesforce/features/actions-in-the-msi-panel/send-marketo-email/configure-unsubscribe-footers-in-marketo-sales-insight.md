---
unique-page-id: 2953373
description: Saiba como configurar rodapés de cancelamento de inscrição no Marketo Sales Insight. Configurar links de cancelamento de inscrição e conformidade para emails de vendas.
title: Configurar rodapés de cancelamento de inscrição no Insight de vendas do Marketo
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/9HUCspCSN2LZQzpNJhCI3yiMVzwOYMxyp06UDJQyT2Y
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 210
ht-degree: 4%

---

# Configurar o Cancelamento de Inscrição de Rodapés em [!DNL Marketo Sales Insight] {#configure-unsubscribe-footers-in-marketo-sales-insight}

Emails de vendas colocam automaticamente o rodapé de cancelamento de inscrição na parte inferior. No entanto, você pode ajustar as configurações para atender às suas necessidades.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

>[!NOTE]
>
>**Definição**
>
>**Emails de vendas** são aqueles enviados de [!DNL Sales Insight] (não inclui aqueles enviados do Plug-in Marketo Outlook).

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/one-1.png)

1. Clique em **[!UICONTROL Sales Insight]** e depois em **[!UICONTROL Editar configurações]**.

   ![](assets/two-1.png)

   Há várias opções. Primeiro, vamos analisar os tipos de emails para os quais você pode alterar as configurações.

   ![](assets/three-1.png)

   * **[!UICONTROL Nenhum Modelo]** - Composto manualmente pelo usuário de vendas.
   * **[!UICONTROL Email Padrão]** - Emails baseados em um modelo.
   * **[!UICONTROL Email Operacional]** - Emails que ignoram os Limites de Cancelamento de Assinatura, de Suspensão de Marketing e de Comunicação (são enviados independentemente do que for).

   Você tem a opção de definir comportamentos diferentes para cada tipo.

   >[!CAUTION]
   >
   >**[!UICONTROL Respeitar Configurações de Cancelamento de Inscrição]**: clientes potenciais com inscrição cancelada NÃO receberão o email mesmo que o email publicado seja &quot;operacional&quot;
   >
   >**[!UICONTROL Ignorar Configurações de Cancelamento de Inscrição]**: clientes potenciais com inscrição cancelada RECEBERÃO o email

1. Faça as alterações desejadas e clique em **[!UICONTROL Salvar]**.

   >[!TIP]
   >
   >As duas últimas opções permitem incluir/excluir dinamicamente o rodapé de cancelamento de inscrição, dependendo do número de recipients (maiores que 1 ou maiores que 5).

   ![](assets/four-1.png)

Ufa! Um pouco complicado, mas muito flexível, certo?
