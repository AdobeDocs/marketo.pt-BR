---
description: Promover um webinário interativo - Documentação do Marketo - Documentação do produto
title: Promover um webinário interativo
feature: Interactive Webinars
exl-id: d26f91ce-3a95-4247-9a52-085260bb15e8
source-git-commit: 88c1e40734a980b54f9d7f056399cf9ec2e0e100
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Promover um webinário interativo {#promoting-an-interactive-webinar}

A promoção de um webinário interativo é semelhante à promoção de um webinário de parceiro por meio do Launchpoint. Ao criar um programa de evento Webinar interativo, você pode adicionar membros executando uma campanha ou importando membros para o programa. Para verificar os membros que foram adicionados ao Programa de Evento de Webinars Interativos, clique na guia **Membros**.

![](assets/promoting-an-interactive-webinar-1.png)

Depois que os membros forem adicionados ou importados, você poderá criar uma campanha de email dentro do programa de evento Webinar interativo para enviar um convite a todos os membros do programa e alterar seu status para &quot;convidado&quot; depois que o email for entregue.

>[!NOTE]
>
>Se você quiser adicionar um co-host ou apresentador como membro do público-alvo do programa Evento de webinário interativo, use uma ID de email diferente para ele, caso contrário, ele receberá um erro &quot;este email já está registrado&quot;.

O email pode conter detalhes específicos do programa, bem como incluir um URL de página de aterrissagem que redirecionaria o recipient para uma página específica onde mais informações sobre o webinário (por exemplo, conteúdo, informações do apresentador etc.) podem ser adicionadas. Essa landing page pode ser criada como um ativo local no programa de evento de webinários interativos.

Você pode solicitar o registro para esse webinário ativando um formulário na página de aterrissagem e vinculando os cliques do formulário ao registro ativado no programa de evento de webinário interativo. Uma campanha pode ser criada usando envios de formulários como um acionador e alterando o Status do programa de &quot;convidado&quot; para &quot;registrado&quot;.

>[!NOTE]
>
>A transição de &quot;convidado&quot; para &quot;registrado&quot; não é automática em Webinars interativos, pois pode haver vários acionadores que criam a transição.

Depois que um membro estiver no status &quot;registrado&quot; do programa em um programa de evento de webinário interativo, um registro será feito automaticamente no webinário criado no Adobe Connect. Os dados de registro, como Nome, Sobrenome e ID de email, são transferidos para o Adobe Connect. Isso significa que quando o usuário ingressar no webinário como participante, as informações estarão disponíveis para o apresentador ou host durante o webinário.

Após alguns minutos do registro, o URL do webinário do membro é preenchido na Guia Membros. Se não conseguir localizar a coluna para o URL do webinário, verifique se a coluna foi adicionada à visualização. Este é um URL personalizado para cada membro registrado poder entrar no webinário no horário agendado sem exigir autenticação. Os tokens trocados internamente cuidam da autenticação dos membros.

Você pode usar o `{{member.webinar url}}` [token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} para incluir a URL do webinário para membros individuais em uma campanha por email para comunicar que eles foram registrados no evento e usar a URL de ingresso para entrar no webinário no horário agendado. Os tokens de calendário podem ser usados na mesma campanha de email para garantir que a programação do webinário possa ser adicionada aos calendários dos membros.

Os links estão disponíveis no lado direito da guia Visão geral no Programa de evento para criar uma Página de aterrissagem, bem como uma campanha de email. O restante das promoções relacionadas a um evento permanecem as mesmas que webinários de parceiros usando a integração do Launchpoint.

![](assets/promoting-an-interactive-webinar-2.png)

Webinars interativos permitem solicitar registro antes, durante ou depois de um webinário. Em todos os casos, bastaria compartilhar o URL do webinário com o lead. Clicar no link antes do início do webinário os envia para uma página de aterrissagem pré-webinário. Clicar nele durante o webinário os leva para o webinário em andamento. Clicar nele depois do webinário os leva para uma gravação do webinário.

## Tokens de webinários interativos {#interactive-webinars-tokens}

Use tokens para promover Webinars interativos em emails e Landing Pages sem precisar adicionar detalhes do webinário manualmente. Isso melhora a eficiência geral, pois qualquer alteração feita nos metadados do webinário (como título do webinário, data de início etc.) será refletida automaticamente em seus ativos.

![](assets/promoting-an-interactive-webinar-3.png)

**Lista de tokens**

* program.webinarCapacity
* program.webinarDuration
* program.webinarEndDate
* program.webinarEndTime
* program.webinarGenericURL
* program.webinarLanguage
* program.webinarStartDate
* program.webinarStartTime
* program.webinarTimezone
* program.webinarTitle
