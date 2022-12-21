---
unique-page-id: 2953373
description: Configurar rodapés de cancelamento de inscrição no Marketo Sales Insight - Documentos da Marketo - Documentação do produto
title: Configurar rodapés de cancelamento de inscrição no Marketo Sales Insight
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Configurar rodapés de cancelamento de inscrição no Marketo Sales Insight {#configure-unsubscribe-footers-in-marketo-sales-insight}

Os emails de vendas colocam automaticamente o rodapé de cancelamento de inscrição na parte inferior. No entanto, você pode ajustar as configurações para atender às suas necessidades.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>**Definição**
>
>**Emails de vendas** são enviadas do Sales Insight (não inclui as enviadas pelo plug-in do Marketo Outlook).

1. Vá para o **Administrador** área.

   ![](assets/one-1.png)

1. Clique em **Insight de vendas**, em seguida **Editar configurações**.

   ![](assets/two-1.png)

   Há várias opções. Primeiro vamos analisar os tipos de emails para os quais você pode alterar as configurações.

   ![](assets/three-1.png)

   * **Sem modelo** - Composto manualmente pelo usuário de vendas.
   * **Email padrão** - Emails com base em um template.
   * **Email operacional** - Emails que ignoram a assinatura cancelada, o marketing suspenso e os limites de comunicação (eles enviam independentemente do que for).

   Você tem a opção de definir comportamentos diferentes para cada tipo.

   >[!CAUTION]
   >
   >**Respeitar configurações de cancelamento de inscrição**: os leads cancelados NÃO receberão o email mesmo se o email publicado for &quot;operacional&quot;
   >
   >**Ignorar configurações de cancelamento de inscrição**: os leads não subscritos receberão o email

1. Faça as alterações desejadas e clique em **Salvar**.

   >[!TIP]
   >
   >As duas últimas opções permitem incluir/excluir dinamicamente o rodapé de cancelamento de inscrição, dependendo do número de recipients (maior que 1 ou maior que 5).

   ![](assets/four-1.png)

Uau! Um pouco complicado, mas bastante flexível, certo?
