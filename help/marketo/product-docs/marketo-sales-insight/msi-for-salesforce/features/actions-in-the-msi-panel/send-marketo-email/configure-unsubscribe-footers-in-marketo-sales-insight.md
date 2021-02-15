---
unique-page-id: 2953373
description: Configurar os rodapés de cancelamento de assinatura no Marketing Insight de vendas - Documentos do Marketing Cloud - Documentação do produto
title: Configurar os rodapés de cancelamento de assinatura no Marketing Insight de vendas
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---


# Configurar os rodapés de cancelamento de assinatura no Marketing Insight de vendas {#configure-unsubscribe-footers-in-marketo-sales-insight}

Os emails de vendas colocam automaticamente o rodapé de cancelamento de assinatura na parte inferior. No entanto, você pode ajustar as configurações para atender às suas necessidades.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>**Definição**
>
>**Os** emails de vendas são enviados do Sales Insight (não inclui os enviados do Plug-in Marketing para Outlook).

1. Vá para a área **Admin**.

   ![](assets/one-1.png)

1. Clique em **Sales Insight** e, em seguida, em **Editar configurações**.

   ![](assets/two-1.png)

   Há várias opções. Primeiro vamos analisar os tipos de e-mails para os quais você pode alterar as configurações.

   ![](assets/three-1.png)

   * **Nenhum modelo**  - Composto manualmente pelo usuário de vendas.
   * **Email**  padrão - Emails com base em um modelo.
   * **E-mail**  operacional: os e-mails que ignoram os Limites de não assinatura, de suspensão de marketing e de comunicação (eles enviam independentemente do que for).

   Você tem a opção de definir um comportamento diferente para cada tipo.

   >[!CAUTION]
   >
   >**Respeite as configurações** de cancelamento de assinatura: os clientes potenciais não inscritos NÃO receberão o email, mesmo se o email publicado for &quot;operacional&quot;
   >
   >**Ignorar configurações** de cancelamento de inscrição: clientes potenciais não inscritos receberão o email

1. Faça as alterações desejadas e clique em **Salvar**.

   >[!TIP]
   >
   >As duas últimas opções permitem que você inclua/exclua dinamicamente o rodapé de cancelamento de inscrição dependendo do número de recipient (maior que 1 ou maior que 5).

   ![](assets/four-1.png)

Uuu! Um pouco complicado, mas bastante flexível, certo?
