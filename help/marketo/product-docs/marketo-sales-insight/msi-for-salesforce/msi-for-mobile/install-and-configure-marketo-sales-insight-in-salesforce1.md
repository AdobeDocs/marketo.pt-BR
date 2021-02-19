---
unique-page-id: 7511512
description: Instalar e configurar o Marketing Sales Insight no Salesforce1 - Documentos do Marketing - Documentação do produto
title: Instalar e configurar o Marketingto Sales Insight no Salesforce1
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Instalar e configurar o Marketingto Sales Insight no Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Clientes existentes, [Atualize seu pacote MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) antes de continuar!

>[!PREREQUISITES]
>
>Se você tiver o Salesforce Enterprise/Unlimited:
>
>* [Etapa 1 de 3: Adicionar campos de marketing ao Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Etapa 2 de 3: Criar um usuário do Salesforce para o Marketing (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Etapa 3 de 3: Connect Marketing e Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configurar o Marketing to Sales Insight no Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

>
>
Se você tiver o Salesforce Professional:
>
>* [Configurar o Marketing Sales Insight no Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)

>



>[!NOTE]
>
>O Marketing to Sales Insight no Salesforce1 inclui: Melhores apostas, feed principal, momentos interessantes e Campanha Adicionar ao marketing.

## Ative o aplicativo móvel Salesforce1 {#enable-the-salesforce1-mobile-app}

1. Clique em **Configuração** e em **Administração Móvel**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Clique em **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Clique em **Configurações do Salesforce1**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Clique em **Ativar o aplicativo do navegador móvel Salesforce1**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Clique em **Salvar**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Selecione **Administração móvel**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Clique em **Gerenciar o menu de navegação móvel**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Selecione **Marketo** e **Adicione** aos itens de menu **Selecionado**.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Selecione **Marketo**, mova-o **Para cima** para uma área desejada e clique em **Guardar**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Ocultar objeto personalizado Marketo desatualizado {#hide-outdated-marketo-custom-object}

1. Clique em **Configuração**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Selecione **Gerenciar usuários**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Selecione **Perfis**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Clique para **editar** quaisquer perfis desejados.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Em **Configurações de tabulação**, selecione _first_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Selecione **Tabulação oculta**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Certifique-se de ocultar a guia Marketo para todos os perfis desejados!

## Personalizar guias {#customize-tabs}

1. Clique em **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Clique em **Personalizar minhas guias**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Selecione **Marketo** e **Adicionar** às Guias Selecionadas.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Selecione **Marketo**, mova-o **Para cima** para uma área desejada e clique em **Guardar**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personalizar layouts de página {#customize-page-layouts}

1. Clique em **Configuração**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Clique em **Configuração**, digite **Layouts de página** e clique em **Layouts de página** em Clientes potenciais.

   >[!NOTE]
   >
   >Repita as etapas para cada Layout de página que sua organização usa (marketing, vendas etc.) para objetos de Contato, Conta e Oportunidade.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Clique em **Editar** para fazer alterações no Layout principal.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Clique em **Visualforce Pages** e arraste **Lead Mobile** para a seção Mobile Cards.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Altere a Altura para 66 e clique em **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Clique em **Campos** e arraste **Adicionar à Campanha de marketing** para a seção **Marketing to Sales Insight**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Digite &quot;Adicionar a&quot; na Localização Rápida para facilitar a localização da Campanha Adicionar ao Marketing.

1. Clique em **Salvar**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Ufa! Finalmente, você terminou de instalar o Marketing Insight Sales para Salesforce1! Vá em frente e dê um tapinha nas costas.

>[!MORELIKETHIS]
>
>* [Melhores apostas no Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Momentos interessantes em Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Enviar ações de Campanha e email para marketing e lista de vigias no Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)

