---
unique-page-id: 4719291
description: Definir o sobrenome da pessoa padrão e o nome da Empresa - Documentos de marketing - Documentação do produto
title: Definir o sobrenome da pessoa padrão e o nome da Empresa
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---


# Definir o sobrenome da pessoa padrão e o nome da Empresa {#set-default-person-last-name-and-company-name}

O Salesforce requer (mínimo) sobrenome e nome da empresa para seus Clientes potenciais e Contatos. Os registros incompletos não serão sincronizados com o Salesforce. Se desejar sincronizar registros parciais, defina os valores padrão para que o Marketo possa ser usado com o Salesforce.

1. Vá para **Admin** e clique em **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Clique em **Editar opções de sincronização**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Digite um **sobrenome de pessoa padrão** e um **Padrão ****empresa de pessoa** e clique em **Salvar**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >O Marketo só atribui um valor padrão quando o registro é sincronizado inicialmente com o Salesforce e somente se um dos campos obrigatórios estiver vazio.

E é isso! Sempre que uma pessoa não tiver um sobrenome e/ou nome de empresa, o Marketo adicionará o valor padrão conforme sincroniza o registro.
