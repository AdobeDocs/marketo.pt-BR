---
description: Regras globais de validação de formulário - Documentos do Marketo - Documentação do produto
title: Regras globais de validação de formulário
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
source-git-commit: d9e605d31e9a3434849ba800ba527775885ab34a
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Regras globais de validação de formulário {#global-form-validation-rules}

Esse recurso permite bloquear o envio de domínios específicos para formulários Marketo Engage.

## Como ativar o acesso {#how-to-enable-access}

Antes de utilizar esse recurso, é necessário habilitar a permissão de acordo com a função desejada.

1. No Marketo, clique em **Administrador**.

   ![](assets/global-form-validation-rules-1.png)

1. Clique em **Usuários e funções**.

   ![](assets/global-form-validation-rules-2.png)

1. Clique no botão **Funções** guia .

   ![](assets/global-form-validation-rules-3.png)

1. Clique duas vezes na função para a qual deseja conceder permissões.

   ![](assets/global-form-validation-rules-4.png)

1. Clique no botão **+** assine ao lado de Administrador de acesso.

   ![](assets/global-form-validation-rules-5.png)

1. Role para baixo e selecione **Acessar regras de validação de formulário** e clique em **Salvar**.

   ![](assets/global-form-validation-rules-6.png)

## Criar nova regra de validação de formulário {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Essas regras se aplicarão a todos os formulários na(s) assinatura(s) do Marketo Engage.

1. No Marketo, clique em **Administrador**.

   ![](assets/global-form-validation-rules-7.png)

1. Clique em **Regra de validação de formulário global**.

   ![](assets/global-form-validation-rules-8.png)

1. Clique em **Nova regra de validação de formulário**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >A lista suspensa Ações da regra de validação de formulário permite excluir ou editar regras existentes.

1. Nomeie sua regra, forneça uma descrição opcional e insira a mensagem de erro que deseja que os visitantes do formulário vejam. Digite os domínios que deseja bloquear na caixa de regras e selecione **Ativar regra** e clique em **Criar**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>O Marketo Engage tem uma lista de bloqueios definida de domínios de email gratuitos do consumidor que são bloqueados ao usar nossa regra pré-carregada de &quot;Lista de bloqueios de domínio de email do consumidor&quot;. [Veja essa lista aqui](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv).

## Como desativar o acesso por formulário{#how-to-disable-access-per-form}

Depois de ativadas, as regras se aplicam a todos os formulários. No entanto, se você tiver um formulário com requisitos específicos e não quiser que nada seja rejeitado, poderá desativar as Regras de validação de formulário global nas configurações do formulário.

1. No formulário desejado, clique em **Configurações do formulário**, em seguida **Configurações**.

   ![](assets/global-form-validation-rules-11.png)

1. Clique no menu suspenso Regras globais de validação de formulário e escolha **Desabilitado**.

   ![](assets/global-form-validation-rules-12.png)

Ao aprovar e publicar seu formulário, ele ignorará suas Regras globais de validação de formulário.
