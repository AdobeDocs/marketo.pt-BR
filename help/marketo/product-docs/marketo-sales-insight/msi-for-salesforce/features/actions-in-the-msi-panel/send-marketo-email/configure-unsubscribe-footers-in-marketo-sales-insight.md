---
unique-page-id: 2953373
description: Configurar os rodapés de cancelamento de inscrição no Marketo Sales Insight - Documentação do Marketo - Documentação do produto
title: Configurar o cancelamento de inscrição de rodapés no Marketo Sales Insight
exl-id: 16c1fcba-6826-400c-ab7c-371d8653d4ad
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Configurar o cancelamento de inscrição de rodapés no Marketo Sales Insight {#configure-unsubscribe-footers-in-marketo-sales-insight}

Emails de vendas colocam automaticamente o rodapé de cancelamento de inscrição na parte inferior. No entanto, você pode ajustar as configurações para atender às suas necessidades.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>**Definição**
>
>**Emails de vendas** são aqueles enviados pelo Sales Insight (não incluem aqueles enviados pelo plug-in do Marketo Outlook).

1. Vá para a área **Administrador**.

   ![](assets/one-1.png)

1. Clique em **Insight de vendas** e depois em **Editar configurações**.

   ![](assets/two-1.png)

   Há várias opções. Primeiro, vamos analisar os tipos de emails para os quais você pode alterar as configurações.

   ![](assets/three-1.png)

   * **Nenhum Modelo** - Composto manualmente pelo usuário de vendas.
   * **Email Padrão** - Emails baseados em um modelo.
   * **Email Operacional** - Emails que ignoram os Limites de Cancelamento de Assinatura, de Suspensão de Marketing e de Comunicação (são enviados independentemente do que for).

   Você tem a opção de definir comportamentos diferentes para cada tipo.

   >[!CAUTION]
   >
   >**Respeitar Configurações de Cancelamento de Inscrição**: clientes potenciais com inscrição cancelada NÃO receberão o email mesmo que o email publicado seja &quot;operacional&quot;
   >
   >**Ignorar Configurações de Cancelamento de Inscrição**: clientes potenciais com inscrição cancelada RECEBERÃO o email

1. Faça as alterações desejadas e clique em **Salvar**.

   >[!TIP]
   >
   >As duas últimas opções permitem incluir/excluir dinamicamente o rodapé de cancelamento de inscrição, dependendo do número de recipients (maiores que 1 ou maiores que 5).

   ![](assets/four-1.png)

Ufa! Um pouco complicado, mas muito flexível, certo?
