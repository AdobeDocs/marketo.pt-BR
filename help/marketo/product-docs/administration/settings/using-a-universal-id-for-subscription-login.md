---
unique-page-id: 10100311
description: Uso de uma Universal ID para logon de assinatura - Documentação do Marketo - Documentação do produto
title: Uso de uma Universal ID para logon de assinatura
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
feature: Administration
source-git-commit: c0f0134972138eb4fa3498028a4acf5233dbe2fe
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Uso de uma Universal ID para logon de assinatura {#using-a-universal-id-for-subscription-login}

A Universal ID permite acessar várias assinaturas do Marketo com um único logon e alternar entre assinaturas rapidamente. No entanto, você pode usar logons diferentes para suas assinaturas, se desejar.

Com a Universal ID, você ainda cria tíquetes de suporte para cada uma de suas assinaturas individuais.

As configurações de nível de assinatura são respeitadas para usuários que usam Universal ID, por exemplo, funções, permissões e políticas de senha. As alterações no nível do perfil do usuário são refletidas em todas as assinaturas, por exemplo, nome, sobrenome e endereço de email.

## Configuração de uma Universal ID {#setting-up-a-universal-id}

Todas as assinaturas do Marketo vêm com o recurso opcional de Universal ID. De cada instância individual, o administrador do Marketo deve convidá-lo para cada uma de suas assinaturas diferentes com o mesmo logon. O Marketo não pode mesclar seus logons existentes automaticamente.

>[!NOTE]
>
>Se você tiver várias IDs de logon de assinatura, também poderá ter vários perfis de comunidade. Certifique-se de escolher a ID da Universal ID conectada ao perfil que você deseja usar para a instância de produção e não para a sandbox.

## Efetuando Login {#logging-in}

Ao fazer logon para aceitar um convite para uma segunda assinatura usando uma Universal ID, você verá a página de logon de Opt-in. Aqui, você deve marcar uma caixa de seleção para aceitar os termos e condições. Depois de aceitar, você verá a página de redefinição normal, não esta, para os logons subsequentes. Ao aceitar os termos e condições, você permite que a Marketo distribua seus dados básicos de perfil (como nome, sobrenome e endereço de email) para os data centers em diferentes locais onde sua assinatura está hospedada.

![](assets/using-a-universal-id-for-subscription-login-1.png)

>[!TIP]
>
>As IDs que você não usa mais permanecem, a menos que o administrador de assinatura as exclua. Recomendamos que você os mantenha, caso, por exemplo, você tenha um relatório privado, atribuído a você mesmo, que só possa ser acessado usando essa ID. Nesse caso, faz sentido mover esses relatórios privados para sua nova Universal ID e, em seguida, excluir sua ID existente.

## Senhas {#passwords}

Com a Universal ID para várias assinaturas, o Marketo aplica automaticamente a política de senha mais rigorosa. Por exemplo, se algumas assinaturas exigirem um comprimento mínimo de senha e outras não, o comprimento mínimo será aplicado a todas as assinaturas.

Com uma Universal ID para várias assinaturas, somente você pode alterar a senha.

>[!NOTE]
>
>O Marketo solicitará aos usuários que desejam usar a Universal ID que redefinam suas senhas se a senha da assinatura atual não estiver em conformidade com a política de senha da segunda assinatura para a qual estão sendo convidados.

## Alternância entre assinaturas {#switching-between-subscriptions}

Usando uma Universal ID, você pode ver a assinatura à qual está conectado e selecionar outras assinaturas às quais você tem acesso de logon. Na maioria dos casos, você pode alternar entre elas sem precisar fazer logoff e logon novamente.

![](assets/using-a-universal-id-for-subscription-login-2.png)

Ao fazer logout e fazer logon novamente, o Marketo automaticamente faz logon na assinatura na qual você fez logon pela última vez. Você pode alternar para uma assinatura diferente, se necessário.

## Perfis da comunidade {#community-profiles}

Se você tiver várias assinaturas, poderá ter vários perfis de comunidade. Recomendamos que você escolha o login vinculado ao seu perfil da comunidade mais ativo.

>[!MORELIKETHIS]
>
>* [Adicionar Logon Único a um Portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md){target="_blank"}
>* [Restringir o logon do usuário somente ao SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md){target="_blank"}
>* [Convidar usuários do Marketo para duas instâncias com Universal ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122){target="_blank"}
