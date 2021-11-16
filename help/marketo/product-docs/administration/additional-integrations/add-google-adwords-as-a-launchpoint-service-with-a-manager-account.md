---
unique-page-id: 7504893
description: Adicionar o Google AdWords as a Launchpoint Service com uma conta do gerente - Documentos da Marketo - Documentação do produto
title: Adicionar o Google AdWords como um serviço do Launchpoint com uma conta do gerente
exl-id: aac106f4-6615-49d5-a561-0dd965c7b0ff
source-git-commit: ab8eb044b89c925accc3b6a4ac4def53e3927321
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 1%

---

# Adicionar o Google AdWords como um serviço do Launchpoint com uma conta do gerente {#add-google-adwords-as-a-launchpoint-service-with-a-manager-account}

Vincule sua conta do Google AdWords ao Marketo para fazer upload automático dos dados de conversão offline do Marketo para o Google AdWords. Em seguida, na interface do usuário do AdWords, você poderá ver facilmente quais cliques resultaram em leads qualificados, oportunidades e novos clientes (ou em quaisquer estágios de receita que deseja rastrear) após  [adicionar colunas personalizadas](https://support.google.com/adwords/answer/3073556) no AdWords. Essas informações não são exibidas na interface do usuário do Marketo.

Se você tiver várias contas Google AdWords, poderá usar um [Conta do gerente do Google AdWords](https://www.google.com/adwords/manager-accounts/) (anteriormente conhecido como Meu centro do cliente) para integrá-los ao Marketo.

Saiba mais sobre [Recurso de importação de conversão offline da Google](https://support.google.com/adwords/answer/2998031?hl=en).

>[!AVAILABILITY]
>
>Nem todos os clientes compraram esse recurso. Entre em contato com o Gerente de sucesso do cliente para obter detalhes.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Também é possível integrar uma [conta Google AdWords independente como um serviço do Launchpoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md).

1. Vá para o **Administrador** seção.

   ![](assets/login-admin-1.png)

1. Selecionar **LaunchPoint**.

   ![](assets/image2014-12-5-14-3a35-3a27.png)

1. Selecionar **Novo** e **Novo Serviço**.

   ![](assets/image2015-2-23-14-3a54-3a50.png)

1. Insira um Nome de exibição e selecione **Google AdWords**.

   ![](assets/new-service-google-1.png)

1. Selecionar **Autorizar Marketo**.

   >[!NOTE]
   >
   >Certifique-se de fazer logoff de sua conta pessoal do Gmail e ativar pop-ups.

   ![](assets/image2015-2-26-20-3a54-3a1.png)

1. Selecione sua conta associada ao **Google AdWords**.

   ![](assets/image2015-2-23-15-3a31-3a16.png)

1. Selecionar **Aceitar**.

   ![](assets/image2015-2-23-16-3a32-3a45.png)

1. O status será exibido como **Sucesso**. Selecionar **Próximo**.

   ![](assets/image2015-2-26-20-3a55-3a21.png)

1. Fazer upload de suas conversões offline do Marketo para o Google AdWords **Semanalmente** ou **Diariamente**.

   ![](assets/image2015-3-27-14-3a7-3a45.png)

1. Conversão de atributo para a **Primeiro clique** ou **Último clique**.

   | Tipo | Definição |
   |---|---|
   | Primeiro clique | As conversões offline serão atribuídas ao primeiro AdWords e uma pessoa clicou nos últimos 90 dias |
   | Último clique | As conversões offline serão atribuídas ao último AdWords e que uma pessoa clicou |

   ![](assets/image2015-3-27-14-3a10-3a46.png)

   >[!NOTE]
   >
   >[Marcação automática](https://support.google.com/adwords/answer/1752125?hl=en) deve ser selecionado para que este recurso funcione. Ele deve ser ativado no AdWords.

1. Clique em **Próximo**.

   ![](assets/image2015-3-27-14-3a11-3a31.png)

1. Desmarque as contas que não deseja atualizar. Clique em **Criar**.

   ![](assets/image2015-3-27-14-3a12-3a51.png)

   Agora, consulte o artigo relacionado abaixo sobre como mapear conversões offline do AdWords em seu modelo de receita.

   >[!MORELIKETHIS]
   >
   >[Definir conversões do Google AdWords no modelo de receita com uma conta de gerente](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account.md)
