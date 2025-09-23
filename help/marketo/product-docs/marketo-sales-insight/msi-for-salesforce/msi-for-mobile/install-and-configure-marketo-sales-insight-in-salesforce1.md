---
unique-page-id: 7511512
description: Instalar e configurar o Marketo Sales Insight no Salesforce1 - Documentação do Marketo - Documentação do produto
title: Instalar e configurar o Insight de vendas do Marketo no Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 3%

---

# Instalar e Configurar o [!DNL Marketo Sales Insight] no [!DNL Salesforce1] {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Clientes existentes, [Atualize seu pacote MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) antes de continuar!

>[!PREREQUISITES]
>
>Se você tiver o Salesforce Enterprise/Unlimited:
>
>* [Etapa 1 de 3: Adicionar Campos do Marketo a [!DNL Salesforce] (Empresarial/Ilimitada)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Etapa 2 de 3: Criar um [!DNL Salesforce] Usuário para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Etapa 3 de 3: Conectar o Marketo e [!DNL Salesforce] (Empresa/Ilimitado)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configurar [!DNL Marketo Sales Insight] em [!DNL Salesforce] Empresa/Ilimitado](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Se você tiver o Salesforce Professional:
>
>* [Configurar o Marketo Sales Insight no Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>[!DNL Marketo Sales Insight] em [!DNL Salesforce1] inclui: [!DNL BMelhores Opções], Feed de Cliente Potencial, Momentos Interessantes e Adicionar ao Marketo Campaign.

## Habilitar o Aplicativo Móvel [!DNL Salesforce1] {#enable-the-salesforce1-mobile-app}

1. Clique em **[!DNL Setup]** e depois em **[!DNL Mobile Administration]**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Clique em **[!UICONTROL Salesforce1]**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Clique em **[!UICONTROL Configurações do Salesforce1]**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Clique em **[!UICONTROL Habilitar o aplicativo Salesforce1 para navegador móvel]**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Selecione **[!UICONTROL Administração do Mobile]**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Clique em **[!UICONTROL Gerenciar o menu de navegação móvel]**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Selecione **[!UICONTROL Marketo]** e **[!UICONTROL Adicionar]** aos itens de menu **[!UICONTROL Selecionados]**.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Selecione **[!UICONTROL Marketo]**, mova-o **[!UICONTROL Para cima]** para uma área desejada e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Ocultar objeto personalizado desatualizado do Marketo {#hide-outdated-marketo-custom-object}

1. Clique em **[!UICONTROL Instalação]**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Selecione **[!UICONTROL Gerenciar Usuários]**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Selecione **[!UICONTROL Perfis]**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Clique para **[!UICONTROL Editar]** os perfis desejados.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Em **[!UICONTROL Configurações da Guia]**, selecione o _primeiro_ **[!UICONTROL Marketo]**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Selecione **[!UICONTROL Guia Oculta]**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Oculte a guia Marketo para todos os perfis desejados.

## Personalizar guias {#customize-tabs}

1. Clique em **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Clique em **[!UICONTROL Personalizar minhas guias]**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Selecione o **[!UICONTROL Marketo]** e **[!UICONTROL Adicionar]** às Guias Selecionadas.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Selecione **[!UICONTROL Marketo]**, mova-o **[!UICONTROL Para cima]** para uma área desejada e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personalizar Layouts de Página {#customize-page-layouts}

1. Clique em **[!UICONTROL Instalação]**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Clique em **[!UICONTROL Configuração]**, digite **[!UICONTROL Layouts de Página]** e clique em **[!UICONTROL Layouts de Página]** em Clientes Potenciais.

   >[!NOTE]
   >
   >Repita as etapas para cada Layout de página que sua organização usa (marketing, vendas etc.) para objetos de Contato, Conta e Oportunidade.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Clique em **[!UICONTROL Editar]** para fazer alterações no Layout de Cliente Potencial.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Clique em **[!UICONTROL Visualforce Pages]** e arraste **[!UICONTROL Lead Mobile]** para a seção Cartões Móveis.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Altere a Altura para 66 e clique em **[!UICONTROL OK]**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Clique em **[!UICONTROL Campos]** e arraste **[!UICONTROL Adicionar ao Marketo Campaign]** para a seção **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Digite &quot;Adicionar a&quot; na Localização rápida para facilitar a localização de Adicionar ao Marketo Campaign.

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Ufa! Você acabou de instalar o [!DNL Marketo Sales Insight] para [!DNL Salesforce1]! Vá em frente e dê um tapinha nas costas.

>[!MORELIKETHIS]
>
>* [[!DNL Best Bets] em [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Momentos interessantes em [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Enviar emails do Marketo e ações do Campaign e da Lista de favoritos em [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
