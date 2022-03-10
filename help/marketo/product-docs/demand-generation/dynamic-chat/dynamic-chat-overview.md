---
description: Visão geral do bate-papo dinâmico - Documentos do Marketo - Documentação do produto
title: Visão geral do bate-papo dinâmico
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: c386d5ae542f4f19ba2acf6d2472a0c9d79c20a3
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# Visão geral do bate-papo dinâmico {#dynamic-chat-overview}

O Dynamic Chat permite que você aproveite uma interface fácil de usar para direcionar pessoas e contas que visitam seu site. Colete conteúdo relevante, como nome, informações de contato e texto livre. Os visitantes do site também podem marcar reuniões com sua equipe de vendas. Os dados dinâmicos de atividade de bate-papo e envolvimento podem ser usados para adicionar membros a programas do Marketo e acionar atividades entre canais.

>[!NOTE]
>
>O Dynamic Chat está sendo lançado gradualmente e está atualmente em disponibilidade limitada. Esta página será atualizada com os detalhes de disponibilidade geral (GA) à medida que forem sendo disponibilizados.

>[!TIP]
>
>Visita [esta página](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) para visualizar vídeos tutoriais do Dynamic Chat.

## Integrações {#integrations}

Um componente essencial do Dynamic Chat é sua capacidade de fazer interface nativa com sua assinatura do Marketo. Para aproveitar todo o recurso dessa integração, primeiro será necessário iniciar a sincronização de dados. Dependendo do tamanho do banco de dados do Marketo, pode levar até 24 horas para os dados iniciais, [sincronização única](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) para concluir.

O seguinte é sincronizado:

* Dados do campo de pessoa
* Dados do campo da empresa
* Dados da atividade

## Diálogos {#dialogues}

As caixas de diálogo representam um único envolvimento de chat. Pense nele como um contêiner com tudo o que você precisa para ter um diálogo de bate-papo envolvente com os visitantes do seu site. Em cada caixa de diálogo, você pode especificar em quais páginas deseja que a caixa de diálogo seja exibida, para quem deseja que ela seja exibida e o conteúdo e fluxo da própria caixa de diálogo. Além disso, você pode encontrar métricas para ver o desempenho da caixa de diálogo. [Saiba mais sobre Diálogos](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## Configuração {#configuration}

Na guia Configuração , personalize a aparência das várias caixas de diálogo. Alterar fonte, cores, tempo de resposta e muito mais! [Saiba mais sobre a configuração](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Calendário {#calendar}

Na guia Calendário , conecte seu calendário (Outlook ou Gmail) para uso na programação de compromissos no chatbot. Quando o calendário de um usuário estiver conectado ao Dynamic Chat, ele será adicionado à fila e seu calendário estará disponível para os visitantes do site agendarem compromissos.

Você também pode personalizar o corpo do convite enviado ao visitante quando ele agendar um compromisso no calendário do usuário.

## Reuniões {#meetings}

É aqui que você verá todos os compromissos agendados pelos visitantes do site por meio de suas várias Diálogos. Aqui você encontrará o endereço de e-mail da pessoa que reservou o compromisso, com qual agente eles reservaram o compromisso, quando o compromisso está programado para ocorrer e se a reunião aconteceu ou não.

## Roteamento {#routing}

É aqui que você pode ver uma lista de todos os agentes que conectaram seus calendários, bem como a ordem em que serão apresentados aos visitantes do site. As reuniões são ao estilo do robin, então se você tem cinco agentes e o agente três tomou a última reunião, o agente quatro terá a próxima, seguido pelo agente cinco, e então de volta ao agente um.

## Perguntas frequentes {#faq}

**O Bate-papo dinâmico permite o bate-papo ao vivo?**

Não, ele utiliza apenas respostas predeterminadas.

**Como posso direcionar pessoas anônimas?**

Na caixa de diálogo, é necessário usar o _O e-mail da pessoa está vazio_ atributo.

**Você suporta a funcionalidade AI/NLP?**

Não oferecemos suporte à funcionalidade AI/NLP.

**Os dados são armazenados por quanto tempo?**

90 dias.

**O Dynamic Chat oferece idiomas além do inglês?**

Não neste momento.

## Limites no bate-papo dinâmico {#limits-in-dynamic-chat}

<table>
  <th>Parâmetro</th>
  <th>Descrição</th>
  <th>Limite</th>
 <tr>
  <td>Total de caixas de diálogo</td>
  <td>Número total de Diálogos (publicados e rascunho)</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Caixas de diálogo publicadas</td>
  <td>Número de caixas de diálogo publicadas salvas</td>
  <td>100</td>
 </tr>
 <tr>
  <td>Direcionar URLs por caixa de diálogo</td>
  <td>Número de URLs de destino que podem ser adicionados a uma única caixa de diálogo</td>
  <td>20º</td>
 </tr>
 <tr>
  <td>Atributos por caixa de diálogo</td>
  <td>Número de atributos que podem ser adicionados aos critérios de público-alvo para uma única caixa de diálogo</td>
  <td>100</td>
 </tr>
 <tr>
  <td>Grupos</td>
  <td>Número de grupos que podem ser adicionados a uma única caixa de diálogo</td>
  <td>10º</td>
 </tr>
 <tr>
  <td>Atributos por grupo</td>
  <td>Número de atributos que podem ser adicionados a um grupo</td>
  <td>10º</td>
 </tr>
 <tr>
  <td>Cartões</td>
  <td>Número de cartões que podem ser adicionados à tela por caixa de diálogo</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Período Anônimo de Retenção de Dados de Lead</td>
  <td>Duração por quanto tempo as informações de um lead anônimo sem qualquer envolvimento serão retidas</td>
  <td>90 dias</td>
 </tr>
 <tr>
  <td>Período de retenção da atividade de meta</td>
  <td>A quantidade de tempo que os dados da atividade da meta são retidos</td>
  <td>24 meses</td>
 </tr>
 <tr>
  <td>Período de retenção da atividade do documento</td>
  <td>Tempo em que os dados da atividade do documento são retidos</td>
  <td>24 meses</td>
 </tr>
 <tr>
  <td>Interagido com Período de Retenção da Atividade de Diálogo</td>
  <td>A quantidade de tempo que interagiu com os dados da atividade Dialog é retida</td>
  <td>90 dias</td>
 </tr>
 <tr>
  <td>Período de Retenção da Atividade de Reserva de Reunião</td>
  <td>A atividade de reserva de horário será armazenada no Bate-papo dinâmico</td>
  <td>24 meses</td>
 </tr>
</table>
