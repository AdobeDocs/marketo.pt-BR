---
unique-page-id: 10095429
description: Corrigir Problemas De Sincronização De Validação Do Dynamics - Documentação Do Marketo - Documentação Do Produto
title: Corrigir Problemas de Sincronização de Validação do Dynamics
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 6%

---

# Corrigir Problemas de Sincronização de Validação do Dynamics {#fix-dynamics-validation-sync-issues}

## Validar Resultados da Ferramenta de Sincronização {#validate-sync-tool-results}

Quando você executa a Sincronização de validação do Dynamics, ela gera um relatório. Se houver um ![x](assets/delete.png) ao lado de uma etapa, consulte as opções abaixo para identificar e corrigir o problema. Em seguida, execute novamente as etapas de validação de sincronização até que o resultado não mostre nada além de marcas de seleção verdes.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL válido {#url-is-valid}

Se você tiver um ![x](assets/delete.png) aqui, verifique se a URL é válida. Encontre-o aqui em Recursos do desenvolvedor e veja o Serviço da organização. O URL pode estar inválido por vários motivos.

1. Faça logon no Dynamics. Clique no ícone Configurações e selecione **Configurações avançadas**.

   ![](assets/one.png)

1. Clique em Configurações e selecione **Personalizações**.

   ![](assets/two.png)

1. Clique em **Recursos do desenvolvedor**.

   ![](assets/three.png)

1. A URL de Serviço da Organização pode ser encontrada em Pontos de Extremidade de Serviço.

   ![](assets/four.png)

## Nome de usuário e senha válidos {#username-and-password-are-valid}

Se você tiver um ![x](assets/delete.png) aqui, verifique se suas credenciais do Microsoft Dynamics são válidas. Para autenticação S2S da API da Web, o nome de usuário no Marketo deve corresponder ao [endereço de email](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) do Usuário do Aplicativo no CRM. Para outros tipos, deve corresponder ao nome de usuário do Usuário de sincronização.

## O usuário de sincronização é atribuído à função Usuário de sincronização do Marketo {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Se você tiver um ![x](assets/delete.png) aqui, pode ser um dos três problemas abaixo.

**Opção Um - Verifique se a Função de Usuário de Sincronização do Marketo está marcada no Microsoft Dynamics**:

1. No Dynamics, clique no ícone Configurações e selecione **Configurações Avançadas**.

   ![](assets/one.png)

1. Clique em **Configurações** e selecione **Segurança**.

   ![](assets/six.png)

1. Clique em **Usuários.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Clique no link para o usuário de sincronização.

   ![](assets/seven.png)

1. Clique em **Gerenciar Funções**.

   ![](assets/eight.png)

1. Verifique se a função Usuário de sincronização do Marketo está marcada. Caso contrário, marque e clique em **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**Opção Dois - Confirmar Consentimento da Concessão**:

1. Revise a [Conceder consentimento para a ID do cliente e o Registro do aplicativo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) para confirmar se o aplicativo tem consentimento administrativo para chamar APIs.

**Opção Três - Sincronizar Usuário**:

1. Verifique se o usuário de sincronização foi adicionado à configuração do Marketo.

## A solução Marketo foi devidamente instalada {#marketo-solution-is-properly-installed}

Se você tiver um ![x](assets/delete.png) aqui, vá para o Microsoft Dynamics para verificar se a instalação do Marketo está lá. Consulte a Etapa 1 da documentação de configuração do Microsoft Dynamics.

1. No Dynamics, clique no ícone Configurações e selecione **Configurações Avançadas**.

   ![](assets/one.png)

1. Clique em **Configurações** e selecione **Soluções.**

   ![](assets/eleven.png)

1. Verifique se a solução está listada.

   ![](assets/twelve.png)

## Todas as etapas da solução estão ativadas {#all-steps-in-the-solution-are-enabled}

Se você tiver um ![x](assets/delete.png) aqui, verifique se nenhuma das etapas padrão foi desativada. Todas as etapas são ativadas automaticamente na instalação, mas podem ser desativadas durante uma personalização.

## Atribui-se o usuário de sincronização à solução Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Se você tiver um ![x](assets/delete.png) aqui, verifique se o usuário de Sincronização está atribuído na página Padrão do Marketo no Microsoft Dynamics.

1. No Dynamics, clique no ícone Configurações e selecione **Configurações Avançadas**.

   ![](assets/one.png)

1. Clique em **Configurações** e selecione **Configuração do Marketo**.

   ![](assets/thirteen.png)

1. Verifique se o usuário de sincronização está atribuído como padrão.

   ![](assets/fourteen.png)

## O usuário de sincronização corresponde ao nome de usuário e à senha {#sync-user-matches-username-and-password}

Se você tiver um ![x](assets/delete.png) aqui, atribua o usuário de sincronização apropriado no campo Usuário do Marketo na etapa de configuração Padrão do Marketo no Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Validar a sincronização do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
