---
description: Stream Designer - Documentação do Marketo - Documentação do produto
title: Designer de fluxo
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 863e5e542e2006ee15f44ad949e876e56a9b39e3
workflow-type: tm+mt
source-wordcount: '1024'
ht-degree: 2%

---

# Designer de fluxo {#stream-designer}

Há _muitos_ combinações de fluxo possíveis. Este artigo contém um exemplo em que o profissional de marketing pergunta ao visitante do site se ele tem alguma pergunta sobre o produto. Em caso positivo, o visitante pode agendar um compromisso. Se não, o visitante terá a opção de ingressar em uma lista de endereçamento para correspondência futura. Eles também recebem um PDF gratuito. O objetivo final é agendar um compromisso ou coletar o email do visitante.

>[!PREREQUISITES]
>
>Antes de usar o cartão Documento, você deve [configurar](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"} na sua conta Adobe.

## Cartões de Designer de Stream {#stream-designer-cards}

O designer de fluxo contém vários cartões que você pode adicionar para moldar a conversa de chat.

<table>
 <tr>
  <td><strong>Mensagem</strong></td>
  <td>Use quando quiser fazer uma declaração sem precisar de resposta (por exemplo: "Olá! Todos os itens têm 25% de desconto hoje com o código SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Pergunta</strong></td>
  <td>Use quando quiser fazer uma pergunta de múltipla escolha, da qual você fornece as respostas disponíveis (por exemplo: Em que tipo de veículo você está interessado? Respostas = SUV, Compacto, Caminhão, etc.).</td>
 </tr>
 <tr>
  <td><strong>Documento</strong></td>
  <td>Permite incorporar documentos PDF em caixas de diálogo e rastrear a atividade de envolvimento de documentos dos visitantes (quantas páginas foram visualizadas, se o documento foi baixado e/ou quaisquer termos de pesquisa usados).</td>
 </tr>
 <tr>
  <td><strong>Captura de informações</strong></td>
  <td>Use quando quiser coletar informações. Os três campos para escolher são Endereço de email, Número de telefone e Texto (o que permite que o visitante escreva sua própria mensagem).</td>
 </tr>
 <tr>
  <td><strong>Agendador de compromissos</strong></td>
  <td>Fornece ao visitante um calendário de datas disponíveis para agendar um acompanhamento. A disponibilidade do calendário reflete <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">o próximo agente na linha</a>. Também há uma opção para transmitir atributos como o nome ou endereço de email do agente.</td>
 </tr>
 <tr>
  <td><strong>Reserva de Reunião</strong></td>
  <td>Fornece ao visitante um calendário de datas disponíveis para agendar uma reunião. Escolha a disponibilidade do calendário por meio do round robin, de um agente específico ou usando regras personalizadas.</td>
 </tr>
 <tr>
  <td><strong>Meta</strong></td>
  <td>Essa é a única carta que os visitantes não verão. Cabe a você determinar em qual ponto uma meta é alcançada no chat específico (por exemplo: se coletar o email do visitante for a sua meta, coloque o cartão de Meta imediatamente após a Captura de informações no stream).</td>
 </tr>
 <tr>
  <td><strong>Ação</strong></td>
  <td>Semelhante aos campos ocultos em um formulário, com o cartão de ação é possível preencher qualquer atributo de cliente potencial ou de empresa com valores implícitos que você gostaria de capturar em um registro de cliente potencial. Você pode adicionar o cartão de ação em qualquer ponto da conversa e atualizar os respectivos atributos com um valor ou tokens nativos que preenchem automaticamente o respectivo valor.</td>
 </tr>
 <tr>
  <td><strong>Chat ao vivo</strong></td>
  <td>Use o cartão de chat ao vivo quando quiser que os visitantes conversem com um agente ao vivo.
  <li>O cartão de chat ao vivo deve ser o último cartão na ramificação.</li>
  <li>Os visitantes serão encaminhados para um agente assim que chegarem a este cartão no stream, portanto, é recomendável preceder este cartão com um cartão de perguntas perguntando aos visitantes se eles gostariam de conversar com um agente ao vivo.</li></td>
 </tr>
</table>

## Ícones do Designer de fluxo {#stream-designer-icons}

No canto superior direito do Stream Designer, você verá vários ícones. Aqui está o que eles fazem.

<table>
 <tr>
  <td><img src="assets/stream-designer-1.png"></td>
  <td>Aumenta o zoom, criando cartões maiores</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-2.png"></td>
  <td>Diminui o zoom, criando cartões menores</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-3.png"></td>
  <td>Abre uma janela para que você teste o seu bate- papo (pressione o mesmo botão para fechar)</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-4.png"></td>
  <td>Permite pesquisar tipos de cartão ou conteúdo em seu fluxo</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-5.png"></td>
  <td>Organiza todos os cartões em seu stream</td>
 </tr>
</table>

## Criar um fluxo {#create-a-stream}

1. Depois de ter [criou seu diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}, clique no link **Designer de fluxo** guia.

   ![](assets/stream-designer-6.png)

1. Arraste e solte o cartão Pergunta.

   ![](assets/stream-designer-7.png)

1. Em Resposta do Chatbot, escreva sua pergunta como você gostaria.

   ![](assets/stream-designer-8.png)

   >[!TIP]
   >
   >Você pode personalizar a experiência de visitantes de bate-papo conhecidos usando tokens (por exemplo: Hello `{{lead.leadFirstName:""}}`). Basta clicar no ícone de chave à direita e fazer a seleção. Adicione um valor padrão entre as aspas se quiser que visitantes anônimos vejam algo genérico (por exemplo: Hello `{{lead.leadFirstName:"there"}}`).

   >[!NOTE]
   >
   >O Poke está definido como ativado por padrão, o que exibe a pergunta de abertura ao lado do ícone do chat sem que o visitante precise clicar nele para vê-lo. O Poke só está disponível no primeiro cartão da conversa.

1. Insira suas respostas de usuário e clique em **Salvar**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**Editar valores armazenados** é uma etapa opcional para quem gostaria de armazenar um valor diferente no banco de dados do que está sendo exibido para os visitantes no chatbot para atributos mapeados no cartão de Pergunta (por exemplo: o visitante vê &quot;Otimização do mecanismo de pesquisa&quot;, você armazena esse valor como &quot;SEO&quot;).

1. Para &quot;Sim&quot;, queremos agendar um compromisso. Portanto, abaixo dessa opção, arraste o cartão Agendador de Compromissos.

   ![](assets/stream-designer-10.png)

1. Na coluna à direita, clique em **Salvar**.

   ![](assets/stream-designer-11.png)

1. Como essa é uma meta, arraste o cartão Meta para baixo do Agendador de Compromissos.

   ![](assets/stream-designer-12.png)

1. Nomeie sua meta (ou escolha uma existente) e clique em **Salvar**.

   ![](assets/stream-designer-13.png)

1. Para &quot;Não&quot; queremos ver se eles vão se juntar à lista de discussão, então abaixo dessa opção arraste sobre outro cartão Pergunta.

   ![](assets/stream-designer-14.png)

1. Insira sua resposta e adicione opções de resposta para o visitante. Clique em **Salvar** quando terminar.

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >Você pode adicionar mais respostas clicando em **Adicionar resposta**.

1. Abaixo da resposta &quot;Sim&quot;, arraste o cartão Captura de informações para poder coletar o email do visitante.

   ![](assets/stream-designer-16.png)

1. Clique em **Tipo** e selecione **E-mail**.

   ![](assets/stream-designer-17.png)

1. Insira uma mensagem de chatbot e um espaço reservado. Verifique se o atributo está mapeado para o campo apropriado no Marketo e clique em **Salvar**.

   ![](assets/stream-designer-18.png)

   <table>
    <tr>
     <td><strong>Tipo</strong></td>
     <td>O tipo de informação que você deseja capturar: Telefone, Texto, Email.</td>
    </tr>
    <tr>
     <td><strong>Mensagem do chatbot</strong></td>
     <td>A mensagem que o visitante vê solicitando que forneça as informações.</td>
    </tr>
    <tr>
     <td><strong>Espaço reservado</strong></td>
     <td>Texto de amostra que ajuda o visitante a ver o que inserir.</td>
    </tr>
    <tr>
     <td><strong>Mapear resposta ao atributo</strong></td>
     <td>Permite sincronizar a resposta do visitante ao campo correspondente no registro Person na sua assinatura do Marketo.</td>
    </tr>
   </table>

1. Como coletar o email é um objetivo, arraste o cartão de Objetivo abaixo de Captura de Informações.

   ![](assets/stream-designer-19.png)

1. Nomeie sua meta (ou escolha uma existente) e clique em **Salvar**.

   ![](assets/stream-designer-20.png)

1. Lembre-se de adicionar uma resposta se eles responderem &quot;Não&quot;. Uma opção é arrastar um cartão de mensagem abaixo e dizer &quot;obrigado mesmo assim&quot;. Mas, neste exemplo, forneceremos a eles um documento PDF gratuito.

   ![](assets/stream-designer-21.png)

1. Neste exemplo, criaremos um novo documento. Nomeie, insira o URL do PDF que você já hospedou e clique em **Salvar**.

   ![](assets/stream-designer-22.png)

1. Selecione o **Visualizar** alternar para visualizar sua caixa de diálogo.

   ![](assets/stream-designer-23.png)

1. Quando estiver pronto para ativar sua caixa de diálogo, clique em **Publish**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>Antes de clicar em Publicar, lembre-se de ter certeza de que [inseriu o(s) URL(s) de destino](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Criar uma caixa de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target="_blank"}
>* [Critérios de público](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target="_blank"}
>* [Relatórios](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target="_blank"}
>* [Uso do Cartão de Documento](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target="_blank"}
