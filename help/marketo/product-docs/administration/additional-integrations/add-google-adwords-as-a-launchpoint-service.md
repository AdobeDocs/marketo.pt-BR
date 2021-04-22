---
unique-page-id: 6095008
description: Adicionar o Google AdWords as a LaunchPoint Service - Documentos do Marketo - Documentação do produto
title: Adicionar o Google AdWords como um serviço do LaunchPoint
exl-id: 993a057a-3f98-4a9f-a770-c9c80dedfd81
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 2%

---

# Adicionar o Google AdWords como um Serviço do LaunchPoint {#add-google-adwords-as-a-launchpoint-service}

Vincule sua conta do Google AdWords ao Marketo para fazer upload automático dos dados de conversão offline do Marketo para o Google AdWords. Em seguida, na interface do usuário do AdWords, você poderá ver facilmente quais cliques resultaram em leads qualificados, oportunidades e novos clientes (ou quaisquer estágios de receita que deseja rastrear) depois de [adicionar colunas personalizadas](https://support.google.com/adwords/answer/3073556) no AdWords. Essas informações não são exibidas na interface do usuário do Marketo.

Saiba mais sobre o [recurso de importação de conversão offline do Google](https://support.google.com/adwords/answer/2998031?hl=en).

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Você também pode integrar um [Google AdWords como um serviço do Launchpoint com uma conta de gerente](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md).

1. Vá para a seção **Admin**.

   ![](assets/login-admin.png)

1. Selecione **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Selecione **Novo** e **Novo Serviço**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Insira um nome de exibição e selecione **Google AdWords**.

   ![](assets/new-service-google.png)

1. Selecione **Autorizar Marketo**.

   >[!NOTE]
   >
   >Certifique-se de fazer logoff de sua conta pessoal do Gmail e ativar pop-ups.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Selecione sua conta associada ao Google AdWords.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Selecione **Accept**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. O status será exibido como **Sucesso**. Selecione **Next**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Faça upload de suas conversões offline do Marketo para o Google AdWords **Semanalmente** ou **Diariamente**.

   ![](assets/image2015-2-23-16-3a53-3a4.png)

1. Conversão de atributo para o **Primeiro clique** ou **Último clique**.

   | Tipo | Definição |
   |---|---|
   | Primeiro clique | As conversões offline serão atribuídas ao primeiro AdWords e uma pessoa clicou nos últimos 90 dias |
   | Último clique | As conversões offline serão atribuídas ao último AdWords e que uma pessoa clicou |

   >[!NOTE]
   >
   >Usar um modelo de atribuição consistente no Marketo e no AdWords fornece os dados mais precisos.

   ![](assets/image2015-2-23-16-3a57-3a49.png)

1. Clique em **Criar**.

   ![](assets/image2015-2-23-17-3a50-3a9.png)

   >[!NOTE]
   >
   >[A ](https://support.google.com/adwords/answer/1752125?hl=en) marcação automática deve ser selecionada para que esse recurso funcione. A desativação deve ser feita no AdWords.

Ótimo! Agora consulte o artigo relacionado abaixo para saber como mapear conversões offline do AdWords em seu modelo de receita.

>[!MORELIKETHIS]
>
>[Definir conversões do Google AdWords no modelo de receita](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model.md)
