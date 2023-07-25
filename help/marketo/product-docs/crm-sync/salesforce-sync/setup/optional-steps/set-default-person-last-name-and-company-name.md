---
unique-page-id: 4719291
description: Definir sobrenome da pessoa padrão e nome da empresa - Documentação do Marketo - Documentação do produto
title: Definir sobrenome da pessoa padrão e nome da empresa
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Definir sobrenome da pessoa padrão e nome da empresa {#set-default-person-last-name-and-company-name}

O Salesforce requer (no mínimo) o sobrenome e o nome da empresa para seus clientes em potencial e contatos. Registros incompletos não serão sincronizados com o Salesforce. Se quiser sincronizar registros parciais, defina valores padrão para o Marketo para usar com o Salesforce.

1. Ir para **Admin** e clique em **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Clique em **Editar Opções de Sincronização**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Insira um **Sobrenome da pessoa padrão** e uma **Empresa pessoal padrão** e clique em **Salvar**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >O Marketo somente atribui um valor padrão quando o registro é sincronizado inicialmente com o Salesforce e somente se qualquer um dos campos obrigatórios estiver vazio.

E é isso! Toda vez que uma pessoa não tiver um sobrenome e/ou nome da empresa, o Marketo adicionará o valor padrão à medida que sincroniza o registro.
