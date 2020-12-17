---
unique-page-id: 10100311
description: Uso de uma ID universal para logon de Subscrição - Documentos do Marketing - Documentação do produto
title: Usando uma ID universal para logon de Subscrição
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---


# Usando uma ID universal para logon de Subscrição {#using-a-universal-id-for-subscription-login}

Uma ID universal permite acessar várias subscrições de marketing com um único logon e alternar rapidamente entre o subscrição. No entanto, você pode usar logons diferentes para suas subscrições, se desejar.

Com a ID universal, você ainda cria tíquetes de suporte para cada uma de suas subscrições individuais.

As configurações de nível de subscrição são respeitadas para usuários que usam a ID universal, por exemplo, funções, permissões e políticas de senha. As alterações no nível do perfil do usuário são refletidas em todas as subscrições, por exemplo, nome, sobrenome e endereço de email.

## Configurando uma ID universal {#setting-up-a-universal-id}

De cada instância individual, seu administrador do Marketo deve convidá-lo para cada uma de suas subscrições diferentes com o mesmo logon. O Marketo não pode unir seus logons existentes automaticamente. Depois que você ativar a ID universal, **sua instância do Marketo estará indisponível** por até 30 minutos. Se você tiver uma base de usuários maior, pode ser um pouco mais.

>[!CAUTION]
>
>Se a ID única ou a ID universal estiver ativada para um usuário, suas funções e espaços de trabalho poderão **não** ser editados após sua configuração inicial.

>[!NOTE]
>
>Se você tiver várias IDs de login de subscrição, também é possível ter vários perfis da comunidade. Certifique-se de escolher a ID da Universal que está conectada ao perfil que você deseja usar e que é para a instância de produção, não para a caixa de proteção.

## Logon em {#logging-in}

Ao fazer logon para aceitar um convite para uma segunda subscrição usando uma ID universal, você verá a página de logon de aceitação. Aqui, você deve marcar uma caixa de seleção para aceitar os termos e condições. Depois de aceitar, você verá a página de redefinição normal, não esta, para quaisquer logons subsequentes. Ao aceitar os termos e condições, você está permitindo que o Marketo distribua seus dados básicos de perfil (como nome, sobrenome e endereço de email) para os data centers em diferentes locais onde sua subscrição está hospedada.

![](assets/new-login-reduced-hands-name.png)

>[!TIP]
>
>As IDs que você não usa não permanecem, a menos que o administrador da subscrição as exclua. Recomendamos que você os mantenha, caso, por exemplo, você tenha um relatório privado, atribuído a si mesmo, que só possa ser acessado usando essa ID. Nesse caso, faz sentido mover esses relatórios privados para sua nova ID universal e, em seguida, excluir sua ID existente.

## Senhas {#passwords}

Com a ID universal para várias subscrições, o Marketo aplica automaticamente a política de senha mais rigorosa. Por exemplo, se algumas subscrições exigirem uma duração mínima de senha e outras não, a duração mínima será imposta para todas as subscrições.

Com uma ID universal para várias subscrições, somente você pode alterar a senha.

>[!NOTE]
>
>O Marketo solicitará aos usuários que desejam usar a ID universal que redefinam sua senha se a senha da subscrição atual não estiver em conformidade com a política de senha da segunda subscrição para a qual estão sendo convidados.

## Alternar entre Subscrição {#switching-between-subscriptions}

Usando uma ID universal, é possível ver a subscrição na qual você está conectado e selecionar outras subscrições às quais você tem acesso de logon. Na maioria dos casos, você pode alternar entre eles sem precisar fazer logout e voltar a fazer logon.

![](assets/image2016-11-3-15-3a10-3a16.png)

Quando você faz logout e volta a fazer login, o Marketo automaticamente faz login na subscrição em que você se conectou pela última vez. Você pode alternar para uma subscrição diferente, se necessário.

## Perfis da comunidade {#community-profiles}

Se você tiver várias subscrições, poderá ter vários perfis da comunidade. Recomendamos que você escolha o logon que está vinculado ao seu perfil mais ativo da comunidade.

## Plataforma móvel {#mobile-platform}

Os usuários com a ID universal podem ver seus dados em Momentos de marketing e no aplicativo de check-in do evento iPad a partir da subscrição em que fizeram logon pela última vez. Não é possível alterar as subscrições da plataforma móvel em si.

