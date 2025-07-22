---
description: Regras de validação do formulário global - Documentação do Marketo - Documentação do produto
title: Regras globais de validação de formulários
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 2%

---

# Regras globais de validação de formulários {#global-form-validation-rules}

Esse recurso permite bloquear o envio de domínios específicos para formulários do Marketo Engage.

## Como habilitar o acesso {#how-to-enable-access}

Antes de utilizar esse recurso, é necessário habilitar a permissão de acordo com a função desejada.

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-1.png)

1. Clique em **[!UICONTROL Usuários e funções]**.

   ![](assets/global-form-validation-rules-2.png)

1. Clique na guia **[!UICONTROL Funções]**.

   ![](assets/global-form-validation-rules-3.png)

1. Clique duas vezes na função à qual você deseja conceder permissões.

   ![](assets/global-form-validation-rules-4.png)

1. Clique no sinal **+** ao lado de **Acessar Administrador**.

   ![](assets/global-form-validation-rules-5.png)

1. Role para baixo, selecione **[!UICONTROL Acessar Regras de Validação de Formulário]** e clique em **[!UICONTROL Salvar]**.

   ![](assets/global-form-validation-rules-6.png)

## Criar nova regra de validação de formulário {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Essas regras serão aplicadas a todos os formulários em suas assinaturas do Marketo Engage.

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/global-form-validation-rules-7.png)

1. Clique em **[!UICONTROL Regra de validação de formulário global]**.

   ![](assets/global-form-validation-rules-8.png)

1. Clique em **[!UICONTROL Nova regra de validação de formulário]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >O menu suspenso [!UICONTROL Ações de Regra de Validação de Formulário] permite excluir ou editar regras existentes.

1. Nomeie sua regra, forneça uma descrição opcional a ela e insira a mensagem de erro que você deseja que os visitantes do formulário vejam. Insira o(s) domínio(s) que deseja bloquear na caixa de regras, selecione **[!UICONTROL Ativar Regra]** e clique em **[!UICONTROL Criar]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>O Marketo Engage tem uma inclui na lista de bloqueios definida de domínios de email de consumidor livre que são bloqueados ao usar a regra pré-carregada &quot;Inclui na lista de bloqueios de domínio de email do consumidor&quot;. [Exibir esta lista aqui](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv) (para baixar, verifique se o seu navegador está atualizado e pode aceitar downloads).

## Como desativar o acesso por formulário{#how-to-disable-access-per-form}

Uma vez ativadas, as regras se aplicam a todos os formulários. Entretanto, se você tiver um formulário com requisitos específicos e não quiser que nada seja rejeitado, poderá desabilitar [!UICONTROL Regras Globais de Validação de Formulário] nas configurações do formulário.

1. No formulário desejado, clique em **[!UICONTROL Configurações de Formulário]** e depois em **[!UICONTROL Configurações]**.

   ![](assets/global-form-validation-rules-11.png)

1. Clique no menu suspenso **[!UICONTROL Regras de validação de formulário global]** e escolha **[!UICONTROL Desabilitado]**.

   ![](assets/global-form-validation-rules-12.png)

Quando você aprovar e publicar seu formulário, ele ignorará suas [!UICONTROL Regras de validação de formulário globais].
