---
unique-page-id: 3571830
description: Etapa 3 de 3 - Conectar a solução Marketo com a conexão S2S - Documentos da Marketo - Documentação do produto
title: Etapa 3 de 3 - Conectar a solução Marketo com a conexão S2S
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
source-git-commit: eb200f085b41489c8d7e11bb2fd059a311e5349c
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 1%

---

# Etapa 3 de 3: Conecte a solução Marketo com a conexão S2S {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

Esta é a última etapa da sincronização. Estamos quase lá!

>[!PREREQUISITES]
>
>* [Etapa 1 de 3: Instalar a solução Marketo com a conexão S2S](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)
>* [Etapa 2 de 3: Configurar a solução Marketo com a conexão S2S](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!IMPORTANT]
>
>Se estiver atualizando da Autenticação Básica para o OAuth, será necessário entrar em contato com o [Suporte Marketo](https://nation.marketo.com/t5/support/ct-p/Support) para obter ajuda com a atualização dos parâmetros adicionais. Habilitar esse recurso interromperá a sincronização temporariamente até que novas credenciais sejam inseridas e a sincronização seja reativada. O recurso pode ser desativado (até abril de 2022) se você desejar reverter para o modo de autenticação antigo.

>[!NOTE]
>
>Antes de inserir novas credenciais, é possível [validá-los aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

## Inserir informações do usuário de sincronização dinâmica {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Administrador**.

   ![](assets/login-admin.png)

1. Clique em **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Selecionar **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Clique em **Editar** em **Etapa 1: Inserir Credenciais**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Certifique-se de que o URL da organização esteja correto, pois não podemos reverter as alterações subsequentes do esquema após o envio. Se um URL de organização incorreto for usado, você terá que obter uma nova assinatura do Marketo. Se você não souber o URL, [saiba como encontrá-lo aqui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

1. Insira o **Nome do usuário**, **Senha**, **ID do cliente**, **Segredo do cliente** e Microsoft Dynamics **URL**. Clique em **Salvar** quando concluído.

   ![](assets/step-3-of-3-connect-s2s-5.png)

   >[!NOTE]
   >
   >O Nome de usuário no Marketo deve corresponder ao Nome de usuário para o usuário de sincronização no CRM. O formato pode ser `user@domain.com` ou DOMÍNIO\usuário.

## Selecionar campos para a sincronização {#select-fields-to-sync}

1. Clique em **Editar** em **Etapa 2: Selecionar Campos para Sincronizar**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Selecione os campos que deseja sincronizar com o Marketo para que sejam pré-selecionados. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>O Marketo armazena uma referência aos campos a serem sincronizados. Se você excluir um campo no Dynamics, recomendamos fazer isso com a variável [sincronização desativada](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Em seguida, atualize o esquema no Marketo editando e salvando o [Selecionar Campos para Sincronizar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, acesse e selecione os novos campos a serem sincronizados com o Marketo.

1. Acesse Admin e selecione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e verifique-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer coisa. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Ativar sincronização {#enable-sync}

1. Clique em **Editar** em **Etapa 3: Ativar Sincronização**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >O Marketo não removerá automaticamente a duplicação em relação a uma sincronização do Microsoft Dynamics ou quando você inserir pessoas ou leads manualmente.

1. Leia tudo na janela pop-up , insira seu endereço de email e clique em **Iniciar Sincronização**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. A primeira sincronização pode levar algumas horas. Quando terminar, você receberá uma notificação por email.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Excelente trabalho!
