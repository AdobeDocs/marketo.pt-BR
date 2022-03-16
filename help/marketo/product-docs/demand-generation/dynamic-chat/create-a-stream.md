---
description: Criar um fluxo - Documentos do Marketo - Documentação do produto
title: Criar um fluxo
exl-id: aa44c7a5-f81b-4029-a1a4-5439bea83847
source-git-commit: d2ac03bd01e1dd6998d47aac82383b64ffdd3ee7
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---

# Criar um fluxo {#create-a-stream}

Existem _many_ combinações de fluxo que podem ser criadas. Este artigo contém um exemplo em que o profissional de marketing pergunta ao visitante do site se ele tem alguma dúvida sobre o produto. Em caso positivo, o visitante pode agendar um compromisso. Se não, o visitante recebe a opção de ingressar em uma lista de endereços para correspondência futura. A meta é agendar um compromisso ou coletar o email do visitante.

![](assets/create-a-stream-0.png)

1. Depois de [criar a caixa de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#create-a-new-dialogue), clique no botão **Designer de fluxo** guia .

   ![](assets/create-a-stream-1.png)

1. Arraste e solte o cartão Pergunta .

   ![](assets/create-a-stream-2.png)

1. Em Resposta do Chatbot, diga à sua pergunta como gostaria.

   ![](assets/create-a-stream-3.png)

   >[!NOTE]
   >
   >O poke é definido para ativado por padrão, o que exibe a pergunta de abertura ao lado do ícone de chat sem que o visitante precise clicar nele para vê-la.

1. Insira suas Respostas do Usuário e clique em **Salvar**.

   ![](assets/create-a-stream-4.png)

1. Para &quot;Sim&quot;, queremos agendar um compromisso, portanto, abaixo dessa opção, arraste sobre o cartão do Agendador de Compromissos.

   ![](assets/create-a-stream-5.png)

1. Na coluna à direita, clique em **Salvar**.

   ![](assets/create-a-stream-6.png)

1. Como essa é uma meta, arraste o cartão Meta abaixo do Agendador de Compromissos.

   ![](assets/create-a-stream-7.png)

1. Nomeie sua meta (ou escolha uma existente) e clique em **Salvar**.

   ![](assets/create-a-stream-8.png)

1. Para o &quot;Não&quot;, queremos ver se eles irão ingressar na lista de endereçamento, portanto, abaixo dessa opção, arraste sobre outro Cartão de Perguntas.

   ![](assets/create-a-stream-9.png)

1. Insira sua resposta e adicione opções de resposta para o visitante. Clique em **Salvar** quando concluído.

   ![](assets/create-a-stream-10.png)

   >[!NOTE]
   >
   >Você pode adicionar mais respostas clicando em **Adicionar resposta**.

1. Abaixo da resposta &quot;Sim&quot;, arraste o cartão Captura de informações para coletar o email do visitante.

   ![](assets/create-a-stream-11.png)

1. Clique no botão **Tipo** e selecione **Email**.

   ![](assets/create-a-stream-12.png)

1. Insira uma mensagem de chatbot e um espaço reservado. Verifique se o atributo está mapeado para o campo apropriado no Marketo e clique em **Salvar**.

   ![](assets/create-a-stream-13.png)

   <table>
    <tr>
     <td><strong>Tipo</strong></td>
     <td>O tipo de informação que você deseja capturar: Telefone, Texto, Email.</td>
    </tr>
    <tr>
     <td><strong>Mensagem de chatbot</strong></td>
     <td>A mensagem que o visitante vê solicitando que forneça as informações.</td>
    </tr>
    <tr>
     <td><strong>Espaço reservado</strong></td>
     <td>Exemplo de texto que ajuda o visitante a ver o que inserir.</td>
    </tr>
    <tr>
     <td><strong>Mapear resposta para o atributo</strong></td>
     <td>Permite sincronizar a resposta do visitante com o campo correspondente em seu registro de Pessoa em sua assinatura do Marketo.</td>
    </tr>
   </table>

1. Como coletar seus emails é uma meta, arraste o cartão Meta abaixo de Captura de Informações.

   ![](assets/create-a-stream-14.png)

1. Nomeie sua meta (ou escolha uma existente) e clique em **Salvar**.

   ![](assets/create-a-stream-15.png)

1. Lembre-se de adicionar uma resposta se eles disserem &quot;Não&quot;. Arraste um Cartão de mensagem abaixo dessa opção.

   ![](assets/create-a-stream-16.png)

1. Insira a mensagem e clique em **Salvar**.

   ![](assets/create-a-stream-17.png)

1. Selecione o **Visualizar** alterne para visualizar sua caixa de diálogo.

   ![](assets/create-a-stream-18.png)

1. Quando estiver pronto para ativar sua caixa de diálogo, clique em **Publicar**.

   ![](assets/create-a-stream-19.png)

>[!NOTE]
>
>Antes de clicar em Publicar, lembre-se de ter certeza de que você [introduziu o(s) URL(s) de destino](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md#target).

>[!MORELIKETHIS]
>
>[Diálogos](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md)
