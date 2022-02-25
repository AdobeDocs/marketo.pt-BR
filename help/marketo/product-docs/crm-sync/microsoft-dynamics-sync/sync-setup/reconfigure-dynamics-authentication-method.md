---
description: Reconfigure o método de autenticação do Dynamics - Documentos do Marketo - Documentação do produto
title: Reconfigure o método de autenticação do Dynamics
exl-id: 2bd6a992-3dfd-4e91-bec5-9fb3f7bbb840
source-git-commit: ab20d9683aa5987778970fd32793dc0f3056c84b
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Reconfigure o método de autenticação do Dynamics {#reconfigure-dynamics-authentication-method}

Siga as etapas abaixo para atualizar seu método de autenticação do Dynamics.

>[!PREREQUISITES]
>
>Configure o aplicativo no Microsoft Dynamics e no Ative Diretory (Azure AD/ADFS) usando o método de autenticação desejado de um dos seguintes artigos:
>
>* [Etapa 2 de 3: Configurar a solução Marketo com conexão de servidor para servidor](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)
>* [Etapa 2 de 4: Configurar a solução Marketo com a conexão de controle de senha do proprietário de recursos](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)


1. No Marketo, clique em **Administrador**.

   ![](assets/reconfigure-dynamics-authentication-method-1.png)

1. Clique em **Microsoft Dynamics**, em seguida **Desativar Sincronização**.

   ![](assets/reconfigure-dynamics-authentication-method-2.png)

   >[!NOTE]
   >
   >Você deve desativar temporariamente a sincronização global para atualizar o Método de autenticação.

1. Clique no botão **Reconfigurar Novo Método de Autenticação** guia .

   ![](assets/reconfigure-dynamics-authentication-method-3.png)

1. Selecione o novo Método de autenticação desejado (neste exemplo, estamos escolhendo a API da Web).

   ![](assets/reconfigure-dynamics-authentication-method-4.png)

1. Insira as credenciais necessárias para o novo Método de autenticação e clique em **Validar**.

   ![](assets/reconfigure-dynamics-authentication-method-5.png)

   >[!NOTE]
   >
   >* Os campos específicos variam de acordo com o método de autenticação escolhido e o formulário será atualizado automaticamente, dependendo do método de autenticação anterior.
   >* Se você tiver sincronizado antes, os dados no formulário acima poderão ser preenchidos previamente. Insira novamente todas as credenciais para garantir os valores corretos.


1. Se tudo estiver bem, a Validar Sincronização gerará todas as marcas de seleção verdes ![](assets/green-check.png). Revise a mensagem e clique em **Switch** para atualizar o Método de autenticação.

   ![](assets/reconfigure-dynamics-authentication-method-6.png)

   >[!NOTE]
   >
   >Se você vir um ![](assets/red-x.png), essa etapa tem um problema. Consulte [Corrigir problemas de sincronização de validação do Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) para identificar e corrigir o(s) problema(s). Em seguida, execute novamente as etapas de validação de sincronização até que o resultado se pareça com a imagem acima.

1. Clique em **Confirmar** para continuar.

   ![](assets/reconfigure-dynamics-authentication-method-7.png)

1. Clique em **Confirmar** novamente.

   ![](assets/reconfigure-dynamics-authentication-method-8.png)

1. Clique em **OK**.

   >[!IMPORTANT]
   >
   >O sistema leva 15 minutos para aceitar o novo modo de autenticação. Aguarde 15 minutos a partir do momento do comutador antes de reativar a sincronização.
