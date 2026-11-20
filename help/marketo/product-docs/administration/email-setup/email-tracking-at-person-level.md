---
description: Saiba como as Substituições de rastreamento de email em nível de pessoa permitem controlar a abertura de emails e o rastreamento de cliques de cada pessoa para oferecer suporte aos requisitos de consentimento e privacidade.
title: Rastreamento de email no nível da pessoa
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/kF-5V-G6-xr3uV-NQBTmFNfhQnk-r-RYt-v0HvJ-4Go'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a913c84b1c4f8927c951af685884edfc792ff213
workflow-type: tm+mt
source-wordcount: '1593'
ht-degree: 2%
---
# Rastreamento de email no nível da pessoa {#email-tracking-at-person-level}

As substituições de rastreamento de email em nível de pessoa permitem aplicar um padrão no nível de ambiente do Marketo e, em seguida, alterar esse padrão para pessoas individuais. O rastreamento de aberturas e de cliques é controlado de forma independente.

Use esse recurso quando seus requisitos de privacidade ou políticas organizacionais exigirem consentimento antes que o engajamento no email seja rastreado.

>[!IMPORTANT]
>
>Esse recurso fornece controles que podem ajudar a suportar suas obrigações de conformidade; ele não determina quais leis se aplicam ou quais pessoas precisam fornecer consentimento. Trabalhe com suas equipes jurídicas e de privacidade para decidir como configurar o rastreamento e como coletar e manter o consentimento.

## Como as decisões de rastreamento funcionam {#how-tracking-decisions-work}

Três configurações funcionam juntas:

| Configuração | Nível | O que ele faz |
|---|---|---|
| **Substituições de rastreamento de email em nível de pessoa** | Ambiente | Ativa ou desativa o recurso. Quando desativado, o Marketo Engage ignora o padrão do ambiente e os campos de substituição de pessoa e usa o comportamento normal de rastreamento. |
| **Acompanhamento de email desativado por padrão** | Ambiente | Define o padrão para rastreamento de aberturas e cliques. Quando desativado, o rastreamento é ativado por padrão. Quando ativado, o rastreamento é desativado por padrão. |
| **Substituir Padrão de Rastreamento Aberto** e **Substituir Padrão de Rastreamento de Cliques** | Pessoa | Campos de pessoa booleanos. Um valor de `true` aplica o oposto do padrão de ambiente para esse tipo de rastreamento. Um valor de `false` ou vazio segue o padrão do ambiente. |

Os campos de substituição não significam &quot;aceitar&quot; ou &quot;recusar&quot; por si só. **`true`sempre significa &quot;o oposto do padrão de ambiente&quot;.**

### Tabela de decisão de rastreamento {#tracking-decision-table}

A Marketo Engage aplica essa decisão separadamente para aberturas de email e cliques de email.

| Recurso | Ambiente padrão | A substituição de pessoa é `false` ou está vazia | A substituição de pessoa é `true` |
|---|---|---|---|
| Ativado | Rastreamento ativado por padrão | Rastreado | Não rastreado |
| Ativado | Rastreamento desativado por padrão | Não rastreado | Rastreado |
| Desativado | Não aplicável | Rastreamento normal; substituição e padrão são ignorados | Rastreamento normal; substituição e padrão são ignorados |

### Exemplo {#example}

Suponha que o recurso esteja ativado e o ambiente padrão esteja rastreando ativado. Uma pessoa tem **Substituir Padrão de Rastreamento Aberto** definido como `true`, enquanto **Substituir Padrão de Rastreamento de Cliques** está vazio. O Marketo Engage não rastreia as aberturas de email dessa pessoa, mas continua a rastrear os cliques de email.

## Escolha um modelo de rastreamento {#choose-a-tracking-model}

Escolha o modelo que corresponde aos requisitos de consentimento e privacidade antes de ativar o recurso ou preencher campos de pessoa.

| Modelo | Ambiente padrão | Definir a substituição para `true` quando | Uso típico |
|---|---|---|---|
| Recusar | Rastreamento ativado por padrão | Uma pessoa se opõe ao rastreamento | Rastreie a maioria das pessoas, mas pare o rastreamento de pessoas que se opõem. |
| Opt-in (consentimento) | Rastreamento desativado por padrão | Uma pessoa consente com o rastreamento | Exigir consentimento antes do rastreamento, incluindo para destinatários abrangidos pelas orientações aplicáveis da CNIL ou da Garante. |

>[!CAUTION]
>
>Escolha seu modelo antes de preencher os campos de substituição e evite alterar o padrão do ambiente posteriormente. Como `true` significa &quot;o oposto do padrão&quot;, a alteração do padrão reverte o efeito de cada valor de substituição existente. Por exemplo, alternar entre o rastreamento ativado por padrão e desativado por padrão pode fazer com que as pessoas que antes se opunham ao rastreamento sejam rastreadas. Se precisar alterar o padrão, atualize os valores de substituição para todas as pessoas afetadas antes que a alteração entre em vigor.

## Ativar o recurso {#enable-the-feature}

As Substituições de rastreamento de email de nível de pessoa estão desativadas por padrão. Para ativá-lo, entre em contato com o Suporte ao cliente da Adobe. Você também pode especificar se deseja que o status padrão do recurso seja **Habilitado** ou **Desabilitado** para o seu ambiente do Marketo.

>[!NOTE]
>
>Você precisa ser um administrador do Marketo para enviar esta solicitação.

>[!TIP]
>
>Antes de pedir ao Adobe para ativar o recurso, preencha os campos de substituição para pessoas existentes. Isso ajuda a garantir que o comportamento de rastreamento desejado se aplique a partir do primeiro email preparado após a ativação.

## Definir valores de substituição para pessoas {#set-override-values-for-people}

Os campos de substituição são campos de pessoa booleanos. Defina-os usando o método que se adapta ao seu fluxo de trabalho:

| Método | Observações |
|---|---|
| [Alterar etapa do fluxo de Valor de Dados](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value){target="_blank"} | Use uma Campanha inteligente para definir um campo quando uma pessoa atender aos seus critérios, como enviar uma caixa de seleção de consentimento em um formulário. |
| Formulários | Mapeie uma caixa de seleção ou um campo oculto em um formulário do Marketo Engage para o campo de pessoa. |
| Importação de lista | Inclua o campo como uma coluna no arquivo de importação. |
| API REST | Use os nomes de campo de API `overrideOpenTrackingDefault` e `overrideClickTrackingDefault`. |

Defina cada campo de acordo com o consentimento da pessoa. Se o seu idioma de consentimento tratar aberturas e cliques separadamente, configure cada campo independentemente.

## O que muda no email {#what-changes-in-the-email}

Quando o Marketo Engage não rastreia uma pessoa, ele altera o conteúdo do email enviado para essa pessoa.

| Rastreamento desativado para | O que muda | O que ainda funciona |
|---|---|---|
| Aberturas | O email não inclui o pixel de rastreamento aberto. Nenhuma atividade de **Email aberto** foi registrada. | Outra funcionalidade de email, incluindo rastreamento de cliques, se permanecer habilitada. |
| Cliques | Os links são direcionados para seus destinos em vez de serem direcionados ao domínio de rastreamento do Marketo Engage. O link de rastreamento oculto não é adicionado. Nenhuma atividade de **Clique em Email** foi registrada. | Os links para cancelar inscrição, o link para opção de não participação do rodapé do email, `list-unsubscribe` e os links para **Exibir como Página da Web** continuam a funcionar. O uso destes links não registra uma atividade de **Clique em Email**. |

## Quais emails são afetados {#which-emails-are-affected}

| Tipo de email | Substituições aplicadas? |
|---|---|
| Emails em lote, como emails enviados de uma Campanha inteligente em lote ou de um programa de email | Sim |
| Emails de acionamento, como emails enviados de um acionador do Smart Campaign | Sim |
| Emails com testes A/B ou variantes de campeão/desafiante | Sim. O rastreamento é decidido separadamente para cada pessoa, independentemente da variante que ela recebe. |
| Exibir como página da Web | Sim. A versão da Web segue as configurações atuais da pessoa. Uma alteração pode levar até uma hora para ser exibida. |
| [Emails operacionais](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational){target="_blank"} | Não. Eles seguem um comportamento normal de rastreamento. |
| Emails de amostra (teste) | Não. Eles seguem um comportamento normal de rastreamento. |
| Visualizações de email | Sem mudanças. As visualizações não são rastreadas. |
| Emails de alerta | Sem mudanças. Os alertas não são rastreados. |
| Mensagens de SMS | Não. Esse recurso se aplica somente a emails. |

## Quando a Marketo Engage toma a decisão de rastreamento {#when-marketo-engage-makes-the-tracking-decision}

O Marketo Engage lê os valores de substituição de uma pessoa ao preparar o email para envio.

- **Entrega agendada ou atrasada:** se um email for preparado agora e entregue posteriormente (por exemplo, com [Início principal](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs){target="_blank"} ou [Fuso horário do destinatário](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone){target="_blank"}), os valores no momento da preparação serão aplicados. Uma alteração feita após a preparação não altera esse email.
- **Emails já entregues:** alterar a substituição de uma pessoa não altera os emails que ela já recebeu. Os cliques nos links em emails enviados anteriormente ainda poderão ser rastreados se esses links forem preparados com o rastreamento ativado.
- **Emails futuros:** uma alteração se aplica aos emails que o Marketo Engage prepara após a alteração.

Se uma pessoa retirar o consentimento, atualize o valor de substituição assim que possível para que a alteração se aplique ao próximo email preparado para ela.

## Impacto nos relatórios, nas listas inteligentes e na pontuação {#impact-on-reporting-smart-lists-and-scoring}

Quando o Marketo Engage não rastreia uma pessoa, ele não registra atividades de **Email aberto** ou **Email clicado**. Como resultado:

- **Smart Lists/Campanhas:** Filtros e acionadores como **Email Aberto** e **Link de Cliques no Email** não correspondem ou são acionados para essa pessoa quando a atividade correspondente não é rastreada.
- **Relatórios e painéis:** As taxas de abertura de email, as taxas de clique e o desempenho do link refletem apenas as pessoas rastreadas. As métricas de engajamento podem diminuir, pois mais pessoas não são rastreadas.
- **Pontuação e êxito do programa:** regras e etapas de sucesso do programa com base em aberturas ou cliques não se aplicam às pessoas cujas atividades não são rastreadas. Revise essas regras para que as pessoas não tenham pontuações ou avançado de forma injusta.
- **Associação de atividade da Web:** quando o rastreamento de cliques está desativado, os links de email não têm o token de rastreamento do Marketo Engage. Se a pessoa ainda não for conhecida pelo Munchkin, uma visita de site por meio desse email não será associada à pessoa por meio do link.

>[!NOTE]
>
>As atividades enviadas, entregues, devolvidas e canceladas não são afetadas.

## Como isso funciona com outras configurações de rastreamento {#how-this-works-with-other-tracking-settings}

As Substituições de rastreamento de email de nível de pessoa podem desativar o rastreamento para uma pessoa. Ele não ativa o rastreamento quando outra configuração já o desativou. Por exemplo, os links marcados com a classe `mktNoTrack` permanecem sem rastreamento mesmo quando as configurações da pessoa permitem o rastreamento de cliques.

## Desativar o recurso {#disable-the-feature}

Para desativar as Substituições de rastreamento de email em nível de pessoa, entre em contato com o Suporte ao cliente da Adobe.

>[!NOTE]
>
>Você precisa ser um administrador do Marketo para enviar esta solicitação.

Ao desabilitar, os emails preparados após a alteração retornam ao comportamento normal de rastreamento. Os valores de substituição permanecem em registros de pessoa, mas são ignorados. Se o recurso for ativado novamente mais tarde, os valores armazenados serão aplicados novamente.

## Perguntas frequentes {#frequently-asked-questions}

### Posso rastrear aberturas, mas não cliques de uma pessoa, ou o inverso? {#can-i-track-opens-but-not-clicks-for-a-person-or-the-reverse}

Sim. O rastreamento de aberturas e cliques é decidido de maneira independente. Defina somente o campo de substituição para o tipo de rastreamento que deseja alterar.

### Esse recurso impede que eu envie emails para uma pessoa? {#does-this-feature-stop-me-from-sending-emails-to-a-person}

Não. Controla somente o rastreamento. Para interromper o envio de emails de marketing para uma pessoa, use os recursos existentes de cancelamento de inscrição e consentimento.

### As pessoas que não são rastreadas ainda veem links de cancelamento de inscrição em funcionamento? {#do-people-who-are-not-tracked-still-see-working-unsubscribe-links}

Sim. Os links para cancelar inscrição e os links para **Exibir como Página da Web** continuam a funcionar para todas as pessoas.

### Por que uma pessoa que optou por não participar ainda tem uma atividade Clicar em email? {#why-does-a-person-who-opted-out-still-have-a-click-email-activity}

Provavelmente, eles clicaram em um link em um email que foi preparado antes da alteração de seu valor de substituição. As alterações se aplicam a emails preparados após a alteração.

### Preciso alterar meus modelos de email? {#do-i-need-to-change-my-email-templates}

Não. A Marketo Engage aplica a decisão de rastreamento ao criar cada email. Não é necessário alterar seus modelos ou emails.
