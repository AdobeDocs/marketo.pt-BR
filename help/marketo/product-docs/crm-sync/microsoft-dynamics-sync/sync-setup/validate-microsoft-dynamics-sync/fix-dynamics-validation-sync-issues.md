---
unique-page-id: 10095429
description: Corrigir problemas de sincronização de validação do Dynamics - Documentos do Marketo - Documentação do produto
title: Corrigir problemas de sincronização de validação do Dynamics
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 8%

---

# Corrigir problemas de sincronização de validação do Dynamics {#fix-dynamics-validation-sync-issues}

## Validar os resultados da ferramenta de sincronização {#validate-sync-tool-results}

Ao executar a Sincronização do Dynamics Validate, ele gera este relatório. Se houver um ![delete](assets/delete.png) ao lado de uma etapa, consulte abaixo para identificar e corrigir o problema. Em seguida, execute novamente as etapas de validação de sincronização até que o resultado não mostre nada além das marcas de seleção.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL válido {#url-is-valid}

Se você tiver um ![delete](assets/delete.png) aqui, verifique se o URL é válido. Localize-o aqui em Recursos do desenvolvedor e veja o Serviço de organização. O URL pode ser inválido por vários motivos.

1. Faça logon no Dynamics. Clique no ícone Configurações e selecione **Configurações avançadas**.

   ![](assets/one.png)

1. Clique em Configurações e selecione **Personalizações**.

   ![](assets/two.png)

1. Clique em **Recursos do desenvolvedor**.

   ![](assets/three.png)

1. O URL do Serviço de Organização pode ser encontrado em Endpoints de Serviço.

   ![](assets/four.png)

## Nome de usuário e senha válidos {#username-and-password-are-valid}

Se você tiver um ![—](assets/delete.png) aqui, verifique se seu nome de usuário e senha do Microsoft Dynamics são válidos.

## O usuário de sincronização é atribuído à função Usuário de sincronização do Marketo {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Se você tiver um ![—](assets/delete.png) aqui, precisará verificar se a função Usuário de sincronização do Marketo está marcada no Microsoft Dynamics. Consulte a Etapa 2 da documentação de instalação do MIcrosoft Dynamics.

1. Em Dinâmicas, clique no ícone Configurações e selecione **Configurações avançadas**.

   ![](assets/one.png)

1. Clique em **Configurações** e selecione **Segurança**.

   ![](assets/six.png)

1. Clique em **Usuários.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Clique no link para o usuário de sincronização.

   ![](assets/seven.png)

1. Clique em **Gerenciar funções**.

   ![](assets/eight.png)

1. Verifique se a função Usuário de sincronização do Marketo está marcada. Caso contrário, marque-o e clique em **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## A solução Marketo foi devidamente instalada {#marketo-solution-is-properly-installed}

Se você tiver um ![—](assets/delete.png) aqui, vá para o Microsoft Dynamics para verificar se a instalação do Marketo está lá. Consulte a Etapa 1 da documentação de configuração do MIcrosoft Dynamics.

1. Em Dinâmicas, clique no ícone Configurações e selecione **Configurações avançadas**.

   ![](assets/one.png)

1. Clique em **Configurações** e selecione **Soluções.**

   ![](assets/eleven.png)

1. Verifique se a solução está listada.

   ![](assets/twelve.png)

## Todas as etapas da solução estão ativadas {#all-steps-in-the-solution-are-enabled}

Se você tiver um ![—](assets/delete.png) aqui, verifique se nenhuma das etapas padrão foi desativada. Todas as etapas são ativadas automaticamente na instalação, mas podem ser desativadas durante uma personalização.

## Atribui-se o usuário de sincronização à solução Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Se você tiver um ![—](assets/delete.png) aqui, verifique se o usuário de Sincronização está atribuído na página Padrão do Marketo no Microsoft Dynamics.

1. Em Dinâmicas, clique no ícone Configurações e selecione **Configurações avançadas**.

   ![](assets/one.png)

1. Clique em **Configurações** e selecione **Marketo Config**.

   ![](assets/thirteen.png)

1. Verifique se o usuário de sincronização está atribuído como padrão.

   ![](assets/fourteen.png)

## O usuário de sincronização corresponde ao nome de usuário e à senha {#sync-user-matches-username-and-password}

Se você tiver um ![—](assets/delete.png) aqui, atribua o usuário de sincronização correto no campo Usuário do Marketo na etapa de configuração Padrão de configuração do Marketo no Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Validar a Sincronização do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
