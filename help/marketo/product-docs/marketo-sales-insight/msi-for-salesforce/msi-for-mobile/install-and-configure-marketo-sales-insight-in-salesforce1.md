---
unique-page-id: 7511512
description: Instalar e configurar o Marketo Sales Insight no Salesforce1 - Marketo Docs - Documentação do produto
title: Instalar e configurar o Marketo Sales Insight no Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Instalar e configurar o Marketo Sales Insight no Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Clientes existentes, [Atualizar o pacote MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) antes de continuar!

>[!PREREQUISITES]
>
>Se você tiver o Salesforce Enterprise/Unlimited:
>
>* [Etapa 1 de 3: Adicionar campos do Marketo ao Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Etapa 2 de 3: Criar um usuário do Salesforce para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Etapa 3 de 3: Conecte a Marketo e o Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Se tiver o Salesforce Professional:
>
>* [Configurar o Marketo Sales Insight no Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>


>[!NOTE]
>
>O Marketo Sales Insight no Salesforce1 inclui: Melhores ideias, alimentação de clientes potenciais, momentos interessantes e adição ao Marketo Campaign.

## Ativar o aplicativo móvel do Salesforce1 {#enable-the-salesforce1-mobile-app}

1. Clique em **Configuração** e depois **Administração móvel**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Clique em **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Clique em **Configurações do Salesforce1**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Clique em **Ativar o aplicativo do navegador móvel do Salesforce1**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Clique em **Salvar**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Selecionar **Administração móvel**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Clique em **Gerenciar o menu de navegação móvel**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Selecionar **Marketo** e **Adicionar** para **Selecionado** itens de menu.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Selecionar **Marketo**, mova-a **Up** para uma área desejada e clique em **Salvar**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Ocultar objeto personalizado Marketo desatualizado {#hide-outdated-marketo-custom-object}

1. Clique em **Configuração**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Selecionar **Gerenciar usuários**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Selecionar **Perfis**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Clique para **editar** qualquer perfil desejado.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Em **Configurações da guia**, selecione o _first_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Selecionar **Tabulação oculta**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Certifique-se de ocultar a guia Marketo para todos os perfis desejados!

## Personalizar guias {#customize-tabs}

1. Clique em **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Clique em **Personalizar Minhas Guias**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Selecionar **Marketo** e **Adicionar** para as guias Selecionadas.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Selecionar **Marketo**, mova-a **Up** para uma área desejada e clique em **Salvar**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personalizar layouts de página {#customize-page-layouts}

1. Clique em **Configuração**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Clique em **Configuração**, tipo **Layouts de página** e clique em **Layouts de página** em Leads.

   >[!NOTE]
   >
   >Repita as etapas para cada Layout de página que sua organização usa (marketing, vendas etc.) para objetos Contato, Conta e Oportunidade.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Clique em **Editar** para fazer alterações no Layout de lead.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Clique em **Páginas da força de visita** e depois arraste **Dispositivo móvel líder** à seção Cartões móveis .

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Altere a Altura para 66 e clique em **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Clique em **Campos** e arrastar **Adicionar ao Marketo Campaign** para **Insight sobre vendas da Marketo** seção.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Digite &quot;Adicionar a&quot; na Localização rápida para facilitar a localização de Adicionar ao Marketo Campaign.

1. Clique em **Salvar**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Ufa! Você acabou de instalar o Marketo Sales Insight for Salesforce1! Vá em frente e dê um tapete nas costas.

>[!MORELIKETHIS]
>
>* [Melhores vantagens no Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Momentos interessantes em Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Enviar email do Marketo e ações de campanha e lista de favoritos no Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)

