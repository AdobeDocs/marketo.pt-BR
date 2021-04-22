---
unique-page-id: 4719291
description: Definir sobrenome da pessoa padrão e nome da empresa - Documentos do Marketo - Documentação do produto
title: Definir Sobrenome de Pessoa e Nome da Empresa Padrão
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Definir Sobrenome de Pessoa Padrão e Nome da Empresa {#set-default-person-last-name-and-company-name}

O Salesforce requer (mínimo) sobrenome e nome da empresa para seus Clientes Potenciais e Contatos. Registros incompletos não serão sincronizados com o Salesforce. Se quiser sincronizar registros parciais, defina valores padrão para o Marketo usar com o Salesforce.

1. Vá para **Admin** e clique em **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Clique em **Editar Opções de Sincronização**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Insira um **Sobrenome de pessoa padrão** e um **Empresa de pessoa padrão**, em seguida, clique em **Salvar**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >O Marketo atribui um valor padrão somente quando o registro é inicialmente sincronizado com o Salesforce, e somente se um dos campos obrigatórios estiver vazio.

E é isso! Toda vez que uma pessoa não tem um sobrenome e/ou nome de empresa, o Marketo adicionará o valor padrão, pois sincroniza o registro.
