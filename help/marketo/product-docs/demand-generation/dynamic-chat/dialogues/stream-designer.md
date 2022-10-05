---
description: Stream Designer - Documentos do Marketo - Documentação do produto
title: Designer de sequência
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: e0f0a89076beaa1be0340e908a59459389b89baa
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 2%

---

# Designer de sequência {#stream-designer}

Existem _many_ combinações de fluxo possíveis. Este artigo contém um exemplo em que o profissional de marketing pergunta ao visitante do site se ele tem alguma dúvida sobre o produto. Em caso positivo, o visitante pode agendar um compromisso. Se não, o visitante recebe a opção de ingressar em uma lista de endereços para correspondência futura. Eles também têm PDF grátis. O objetivo final é agendar um compromisso ou coletar o email do visitante.

>[!PREREQUISITES]
>
>Antes de poder usar o Cartão de documento, você deve primeiro [configurar](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target=&quot;_blank&quot;} em sua conta do Adobe.

## Cartões do Designer de fluxo {#stream-designer-cards}

O designer de fluxo contém vários cartões que podem ser adicionados para moldar a conversa de bate-papo.

<table>
 <tr>
  <td><strong>Mensagem</strong></td>
  <td>Use quando quiser fazer uma declaração sem nenhuma resposta necessária (por exemplo: "Oi! Todos os itens estão 25% de desconto hoje com código SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Pergunta</strong></td>
  <td>Use quando quiser fazer uma pergunta de múltipla escolha, da qual você fornece as respostas disponíveis (por exemplo: Em que tipo de veículo você está interessado? Respostas = SUV, Compacto, Caminhão, etc.).</td>
 </tr>
 <tr>
  <td><strong>Documento</strong></td>
  <td>Permite incorporar documentos do PDF em Caixas de diálogo e rastrear a atividade de envolvimento de documentos dos visitantes (quantas páginas foram visualizadas, se o documento foi baixado e/ou quaisquer termos de pesquisa que foram usados).</td>
 </tr>
 <tr>
  <td><strong>Captura de dados</strong></td>
  <td>Use quando desejar coletar informações. Os três campos a serem escolhidos são Endereço de email, Número de telefone e Texto (o que permite que o visitante grave sua própria mensagem).</td>
 </tr>
 <tr>
  <td><strong>Scheduler de compromissos</strong></td>
  <td>Fornece ao visitante um calendário de datas disponíveis para agendar um acompanhamento. A disponibilidade do calendário reflete <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">o próximo agente em linha</a>.</td>
 </tr>
 <tr>
  <td><strong>Meta</strong></td>
  <td>Este é o único cartão que os visitantes não verão. Cabe a você determinar em qual ponto uma meta é alcançada dentro do chat específico (por exemplo: se coletar o email do visitante for sua meta, coloque o cartão Meta imediatamente após Captura de informações no stream).</td>
 </tr>
</table>

## Ícones do Designer de fluxo {#stream-designer-icons}

No canto superior direito do Designer de fluxo, você verá alguns ícones. Aqui está o que eles fazem.

<table>
 <tr>
  <td><img src="assets/stream-designer-1.png"></td>
  <td>Adiciona uma grade ao plano de fundo para quem prefere essa visualização</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-2.png"></td>
  <td>Aumenta o zoom, criando cartões maiores</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-3.png"></td>
  <td>Diminui o zoom, criando cartões menores</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-4.png"></td>
  <td>Abre uma janela para testar o chat (pressione o mesmo botão para fechar)</td>
 </tr>
 <tr>
  <td><img src="assets/stream-designer-5.png"></td>
  <td>Organiza todas as placas em seu fluxo</td>
 </tr>
</table>

## Criar um fluxo {#create-a-stream}

1. Depois de ter [criou a caixa de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}, clique no link **Designer de fluxo** guia .

   ![](assets/stream-designer-6.png)

1. Arraste e solte o cartão Pergunta .

   ![](assets/stream-designer-7.png)

1. Em Resposta do Chatbot, diga à sua pergunta como gostaria.

   ![](assets/stream-designer-8.png)

   >[!NOTE]
   >
   >O poke é definido para ativado por padrão, o que exibe a pergunta de abertura ao lado do ícone de chat sem que o visitante precise clicar nele para vê-la. O Poke só está disponível no primeiro cartão da conversa.

1. Insira suas Respostas do Usuário e clique em **Salvar**.

   ![](assets/stream-designer-9.png)

   >[!NOTE]
   >
   >**Editar valores armazenados** é uma etapa opcional para quem gostaria de armazenar um valor diferente no banco de dados do que está sendo exibido para os visitantes no chatbot para atributos mapeados no Cartão de perguntas (por exemplo: O visitante vê &quot;Otimização do mecanismo de pesquisa&quot;, você armazena esse valor como &quot;SEO&quot;).

1. Para &quot;Sim&quot;, queremos agendar um compromisso, portanto, abaixo dessa opção, arraste sobre o cartão do Agendador de Compromissos.

   ![](assets/stream-designer-10.png)

1. Na coluna à direita, clique em **Salvar**.

   ![](assets/stream-designer-11.png)

1. Como essa é uma meta, arraste o cartão Meta abaixo do Agendador de Compromissos.

   ![](assets/stream-designer-12.png)

1. Nomeie sua meta (ou escolha uma existente) e clique em **Salvar**.

   ![](assets/stream-designer-13.png)

1. Para o &quot;Não&quot;, queremos ver se eles irão ingressar na lista de endereçamento, portanto, abaixo dessa opção, arraste sobre outro Cartão de Perguntas.

   ![](assets/stream-designer-14.png)

1. Insira sua resposta e adicione opções de resposta para o visitante. Clique em **Salvar** quando concluído.

   ![](assets/stream-designer-15.png)

   >[!NOTE]
   >
   >Você pode adicionar mais respostas clicando em **Adicionar resposta**.

1. Abaixo da resposta &quot;Sim&quot;, arraste o cartão Captura de informações para coletar o email do visitante.

   ![](assets/stream-designer-16.png)

1. Clique no botão **Tipo** e selecione **Email**.

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
     <td>Exemplo de texto que ajuda o visitante a ver o que inserir.</td>
    </tr>
    <tr>
     <td><strong>Mapear resposta ao atributo</strong></td>
     <td>Permite sincronizar a resposta do visitante com o campo correspondente em seu registro de Pessoa em sua assinatura do Marketo.</td>
    </tr>
   </table>

1. Como coletar seus emails é uma meta, arraste o cartão Meta abaixo de Captura de Informações.

   ![](assets/stream-designer-19.png)

1. Nomeie sua meta (ou escolha uma existente) e clique em **Salvar**.

   ![](assets/stream-designer-20.png)

1. Lembre-se de adicionar uma resposta se eles disserem &quot;Não&quot;. Uma opção é arrastar um cartão de mensagem abaixo e dizer &quot;obrigado mesmo assim&quot;. Mas neste exemplo, nós lhes forneceremos um documento de PDF gratuito.

   ![](assets/stream-designer-21.png)

1. Neste exemplo, criaremos um novo documento. Dê um nome a ele, insira o URL do PDF já hospedado e clique em **Salvar**.

   ![](assets/stream-designer-22.png)

1. Selecione o **Visualizar** alterne para visualizar sua caixa de diálogo.

   ![](assets/stream-designer-23.png)

1. Quando estiver pronto para ativar sua caixa de diálogo, clique em **Publicar**.

   ![](assets/stream-designer-24.png)

>[!NOTE]
>
>Antes de clicar em Publicar, lembre-se de ter certeza de que você [introduziu o(s) URL(s) de destino](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md#target){target=&quot;_blank&quot;}.

>[!MORELIKETHIS]
>
>* [Criar uma caixa de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Critérios de público-alvo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/audience-criteria.md){target=&quot;_blank&quot;}
>* [Relatórios](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}
>* [Usando a placa de documento](/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/using-the-document-card.md){target=&quot;_blank&quot;}

