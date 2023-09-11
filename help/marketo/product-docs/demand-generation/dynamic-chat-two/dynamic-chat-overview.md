---
description: Visão geral do Dynamic Chat - Documentação do Marketo - Documentação do produto
title: Visão geral do Dynamic Chat
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: c39d30c40f6e067af6a2a6434a26eb8e2bee8a87
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 2%

---

# Visão geral do Dynamic Chat {#dynamic-chat-overview}

O Dynamic Chat permite utilizar uma interface fácil de usar para direcionar pessoas e contas que visitam seu site. Colete conteúdo relevante, como nome, informações de contato e texto livre. Os visitantes do site também podem marcar reuniões com a equipe de vendas. Os dados de atividade e engajamento do Dynamic Chat podem ser usados para adicionar membros a programas do Marketo e acionar atividades entre canais.

>[!NOTE]
>
>O Dynamic Chat está em processo de implantação gradual e está atualmente com disponibilidade limitada. Esta página será atualizada com os detalhes de disponibilidade geral (GA) conforme forem disponibilizados.

>[!TIP]
>
>Visita [esta página](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) para ver vídeos tutoriais do Dynamic Chat.

## Integrações {#integrations}

Um componente importante do Dynamic Chat é sua capacidade de interagir nativamente com sua assinatura do Marketo. Para aproveitar todos os recursos dessa integração, primeiro inicie a sincronização de dados. Dependendo do tamanho do banco de dados do Marketo, pode levar até 24 horas para que os dados sejam [sincronização única](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/connect-dynamic-chat-to-marketo.md) para concluir.

O seguinte está sincronizado:

* Dados do campo de pessoas
* Dados de campo da empresa
* Dados da atividade

## Diálogos {#dialogues}

As caixas de diálogo representam um único engajamento de chat. Pense nisso como um container com todas as coisas que você precisa para ter uma caixa de diálogo de chat envolvente para os visitantes do seu site. Em cada caixa de diálogo, você pode especificar em quais páginas você deseja que a caixa de diálogo apareça, para quem você deseja que ela seja exibida e o conteúdo e o fluxo da própria caixa de diálogo. Além disso, você pode encontrar métricas para ver o desempenho da sua caixa de diálogo. [Saiba mais sobre Caixas de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/dialogue-overview.md){target="_blank"}.

## Configuração {#configuration}

Na guia Configuração, personalize a aparência das várias caixas de diálogo. Altere a fonte, as cores, o tempo de resposta e muito mais! [Saiba mais sobre Configuração](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md){target="_blank"}.

## Calendário {#calendar}

Conecte seu calendário do Outlook ou Gmail para usar no agendamento de compromissos no chatbot. [Saiba mais sobre Calendário](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/calendar.md){target="_blank"}

## Reuniões {#meetings}

É aqui que você verá todos os compromissos agendados pelos visitantes do site por meio de suas várias Caixas de Diálogo. [Saiba mais sobre reuniões](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/meetings.md){target="_blank"}

## Roteamento {#routing}

É aqui que você pode ver uma lista de todos os agentes que conectaram seus calendários, que ordem eles serão apresentados aos visitantes do site e criar regras de roteamento personalizadas. [Saiba mais sobre Roteamento](/help/marketo/product-docs/demand-generation/dynamic-chat/appointment-scheduling/routing.md){target="_blank"}

## Chat ao vivo {#live-chat}

Ofereça aos visitantes da Web qualificados para se conectarem com seus representantes de vendas via [bate-papo ao vivo](/help/marketo/product-docs/demand-generation/dynamic-chat-two/live-chat/agent-inbox.md){target="_blank"}.

## Perguntas frequentes {#faq}

**É possível instalar o Dynamic Chat em qualquer lugar no site da empresa ou ele funciona somente nas páginas de aterrissagem do Marketo?**

O snippet de JavaScript Dynamic Chat pode ser instalado em qualquer site, bem como nas landing pages do Marketo.

**Por quanto tempo os dados são armazenados para relatórios?**

90 dias (ver a lista completa de limites) [abaixo](#limits-in-dynamic-chat)).

**O Dynamic Chat permite o bate-papo ao vivo?**

Não, ele utiliza apenas respostas predeterminadas.

**O Dynamic Chat suporta outros idiomas além do inglês?**

Sim. O Dynamic Chat é compatível com os seguintes idiomas: francês, alemão, japonês, espanhol, italiano, português brasileiro, coreano, chinês simplificado e chinês tradicional. Saiba mais na [seção abaixo](#changing-the-language).

**Você suporta a funcionalidade AI/NLP?**

Não oferecemos suporte à funcionalidade AI/NLP.

**Como posso segmentar pessoas anônimas?**

Na caixa de diálogo, seria necessário usar o _O e-mail da pessoa está vazio_ atributo.

## Alteração do idioma {#changing-the-language}

Siga estas etapas para alterar o idioma do Dynamic Chat.

>[!IMPORTANT]
>
>Alterar o idioma no nível do perfil mudará o idioma para _all_ aplicativos Experience Cloud, não apenas Dynamic Chat.

1. Na sua conta Experience Cloud, clique no ícone de configurações e escolha **Preferências**.

   ![](assets/dynamic-chat-overview-1.png)

1. Clique no idioma atual em seu endereço de email.

   ![](assets/dynamic-chat-overview-2.png)

1. Escolha seu novo idioma (o segundo idioma é opcional) e clique em **Salvar**.

   ![](assets/dynamic-chat-overview-3.png)

   >[!NOTE]
   >
   >Há algumas dezenas de idiomas para escolher, no entanto, o Dynamic Chat só oferece suporte ao seguinte: inglês, francês, alemão, japonês, espanhol, italiano, português brasileiro, coreano, chinês simplificado e chinês tradicional.

Quando você atualiza o idioma, tudo no próprio aplicativo é alterado, exceto as palavras que você preencheu pessoalmente (por exemplo, respostas de transmissão).

## Limites de retenção de dados Dynamic Chat {#dynamic-chat-data-retention-limits}

<table>
  <th>Tipo de dados</th>
  <th>Período de retenção</th>
 <tr>
  <td>Cliente Potencial Anônimo Sem Qualquer Compromisso</td>
  <td>90 dias</td>
 </tr>
 <tr>
  <td>Atividade da meta</td>
  <td>24 meses</td>
 </tr>
 <tr>
  <td>Atividade do documento</td>
  <td>24 meses</td>
 </tr>
 <tr>
  <td>Interagiu com a atividade de diálogo</td>
  <td>90 dias</td>
 </tr>
 <tr>
  <td>Atividade de Reserva de Reunião</td>
  <td>24 meses</td>
 </tr>
</table>
