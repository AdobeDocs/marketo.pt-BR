---
unique-page-id: 10100311
description: Usar uma ID universal para logon de assinatura - Documentos do Marketo - Documentação do produto
title: Uso de uma ID universal para logon de assinatura
exl-id: 75cf1323-0468-49e9-83ca-e55aa30744ac
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

# Usar uma ID universal para o logon de assinatura {#using-a-universal-id-for-subscription-login}

Uma ID universal permite que você acesse várias assinaturas do Marketo com um único logon e alterne entre assinaturas rapidamente. No entanto, você pode usar logons diferentes para assinaturas se desejar.

Com a ID universal, você ainda cria tíquetes de suporte para cada assinatura individual.

As configurações de nível de assinatura são respeitadas para usuários que usam a ID universal, por exemplo, funções, permissões e políticas de senha. As alterações no nível do perfil do usuário são refletidas em todas as subscrições, por exemplo, nome, sobrenome e endereço de email.

## Configuração de uma ID universal {#setting-up-a-universal-id}

De cada instância individual, o administrador do Marketo deve convidá-lo para cada uma de suas diferentes subscrições com o mesmo logon. O Marketo não pode mesclar seus logons existentes automaticamente. Depois de habilitar a ID universal, **a instância do Marketo estará indisponível** por até 30 minutos. Se você tiver uma base de usuário maior, pode ser um pouco mais longa.

>[!CAUTION]
>
>Se a ID única ou a ID universal estiver ativada para um usuário, suas funções e espaços de trabalho poderão **não** ser editados após sua configuração inicial.

>[!NOTE]
>
>Se você tiver várias IDs de logon de assinatura, também poderá ter vários perfis da comunidade. Certifique-se de escolher a ID da Universal que está conectada ao perfil que você deseja usar e que é para a instância de produção, não para a sandbox.

## Conectando {#logging-in}

Ao fazer logon para aceitar um convite para uma segunda assinatura usando uma ID universal, você verá a página de logon de Opt-in . Aqui, você deve marcar uma caixa de seleção para aceitar os termos e condições. Depois de aceitar, você verá a página normal de redefinição, não esta, para quaisquer logons subsequentes. Ao aceitar os termos e condições, você está permitindo que o Marketo distribua seus dados básicos de perfil (como nome, sobrenome e endereço de email) para os data centers em locais diferentes onde sua assinatura está hospedada.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>As IDs que você não usa mais permanecem, a menos que o administrador da assinatura as exclua. Recomendamos que você os mantenha, caso, por exemplo, você tenha um relatório privado, atribuído a si mesmo, que só pode ser acessado usando essa ID. Nesse caso, faz sentido mover esses relatórios privados para sua nova ID universal e, em seguida, excluir sua ID existente.

## Senhas {#passwords}

Com a ID universal para várias assinaturas, a Marketo aplica automaticamente a política de senha mais rígida. Por exemplo, se algumas subscrições exigirem um comprimento mínimo de senha e outras não, o comprimento mínimo será aplicado para todas as subscrições.

Com uma ID universal para várias assinaturas, somente você pode alterar a senha.

>[!NOTE]
>
>A Marketo pedirá aos usuários que desejam usar a ID universal para redefinir sua senha se a senha da assinatura atual não estiver em conformidade com a política de senha da segunda assinatura para a qual estão sendo convidados.

## Alternando entre assinaturas {#switching-between-subscriptions}

Usando uma ID universal, você pode ver a assinatura na qual está conectado e selecionar outras assinaturas nas quais tem acesso de logon. Na maioria dos casos, você pode alternar entre eles sem ter que fazer logoff e voltar a fazer logon.

![](assets/image2016-11-3-15-3a10-3a16.png)

Quando você faz logoff e faz logon novamente, a Marketo automaticamente faz logon na assinatura em que você se conectou pela última vez. Você pode alternar para uma assinatura diferente, se necessário.

## Perfis da comunidade {#community-profiles}

Se você tiver várias subscrições, poderá ter vários perfis da comunidade. Recomendamos que você escolha o logon vinculado ao seu perfil da comunidade mais ativa.

## Plataforma móvel {#mobile-platform}

Os usuários com a ID universal podem ver seus dados no Marketo Moments e no aplicativo de check-in do evento do iPad a partir da assinatura em que fizeram logon pela última vez. Não é possível alterar assinaturas da plataforma móvel propriamente dita.

>[!MORELIKETHIS]
>
>* [Adicionar logon único a um portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Login de usuário restrito apenas a SSO](/help/marketo/product-docs/administration/additional-integrations/restrict-user-login-to-sso-only.md)
>* [Convidar usuários do Marketo para duas instâncias com ID universal](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

