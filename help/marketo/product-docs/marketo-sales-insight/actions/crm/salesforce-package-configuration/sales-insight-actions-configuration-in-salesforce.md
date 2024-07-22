---
description: Configuração das ações do Sales Insight no Salesforce - Documentação do Marketo - Documentação do produto
title: Configuração das ações do Sales Insight no Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 1%

---

# Configuração das ações do Sales Insight no Salesforce {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Instalar](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) ou [Atualizar](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) pacote Sales Insight na sua instância do Salesforce
>* [Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## Adicionar novo site remoto no Salesforce {#add-new-remote-site-in-salesforce}

1. No Salesforce, clique em **Configurar**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Procure por &quot;site remoto&quot; e selecione **Configurações do Site Remoto**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Clique em **Novo Site Remoto**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoSalesInsight1&quot;). Insira a URL do Site Remoto `https://ims-na1.adobelogin.com` e clique em **Salvar**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Clique novamente em **Novo Site Remoto**.

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoSalesInsight2&quot;). Insira a URL do Site Remoto `https://mkto-sales-connect.adobe.io` e clique em **Salvar**.

## Ativação de ações do Sales Insight no CRM {#enabling-sales-insight-actions-across-the-crm}

1. No Salesforce, clique na guia **Configuração do Marketo Sales Insight**.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Se você não vir &quot;Configuração do Marketo Sales Insight&quot; em sua barra superior, clique no sinal **+** e localize-o em Todas as guias.

1. Marque a caixa de seleção **Habilitar Ações MSI**.

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Insira a chave secreta da API.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Se você não tiver sua Chave de Segurança de API disponível, poderá encontrá-la seguindo as etapas em [este artigo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Clique em **Salvar** quando terminar.

Isso ativará automaticamente todos os recursos de Ações do MSI descritos no artigo de visão geral do recurso.

>[!NOTE]
>
>Você pode desativar todos os recursos de Ações MSI simplesmente desmarcando a caixa de seleção &quot;Ativar ações MSI&quot;.

## Governação das ações IMS {#msi-actions-governance}

1. Você pode desativar Campanhas de vendas e/ou a guia Tarefa na seção futura. Isso será aplicável aos painéis de cliente potencial, contato, conta e oportunidade.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Você pode desativar as Ações MSI ao desmarcar os recursos correspondentes nas configurações Ações.

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>As configurações de governança são aplicáveis a todos os usuários de MSI.
