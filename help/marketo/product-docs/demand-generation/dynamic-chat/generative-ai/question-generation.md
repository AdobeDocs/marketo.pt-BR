---
description: Geração de perguntas - Documentação do Marketo - Documentação do produto
title: Geração de pergunta
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: a711da0fe04e967bfc525be4f3df59d978021592
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Geração de pergunta {#question-generation}

Veja todas as suas tarefas e os detalhes pertinentes, como quando elas foram geradas, o número total de perguntas, o status de aprovação e muito mais.

## Gerar perguntas {#generate-questions}

1. Em IA gerativa, clique em **[!UICONTROL Respostas assistidas]**.

   ![](assets/question-generation-1.png)

1. Clique em **[!UICONTROL Gerar perguntas]**.

   ![](assets/question-generation-2.png)

1. Nomeie sua tarefa e insira um URL de origem (até 10) do qual todo o conteúdo será extraído. Digite os tópicos/palavras-chave desejados e pressione Enter no teclado. Quando terminar, clique em **[!UICONTROL Gerar]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Para garantir que o Marketo Engage possa extrair o conteúdo dos URLs fornecidos, primeiro você deve incluir na lista de permissões vários endereços IP. [Veja os detalhes a seguir](#ip-addresses-to-allowlist).

   >[!NOTE]
   >
   >Os sites/páginas devem ser públicos (ou seja, não devem estar ocultos por um logon) para que suas informações sejam compiladas.

1. Com base no seu conteúdo, a geração de perguntas e respostas pode levar até 30 minutos. Clique em **[!UICONTROL OK]**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Clique em Atualizar para ver o status mais recente da geração de perguntas.

   ![](assets/question-generation-5.png)

## Baixar perguntas e respostas {#download-questions-and-responses}

>[!NOTE]
>
>As perguntas e respostas geradas também são exibidas na [Biblioteca de respostas](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Localize a tarefa desejada e clique no ícone de download ao lado do seu nome.

   ![](assets/question-generation-6.png)

1. Localize a pasta de downloads no seu navegador e selecione o arquivo. Pode parecer diferente dependendo do navegador usado.

   ![](assets/question-generation-7.png)

1. No arquivo do Excel, **[!DNL Task details]** mostra exatamente isso, vários detalhes sobre a tarefa, incluindo instruções sobre como adicionar/editar perguntas e/ou respostas.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Se você decidir adicionar/editar perguntas e/ou respostas em massa, [saiba como recarregá-las aqui](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. A guia **[!DNL Q&Rs]** fornece detalhes adicionais, incluindo as perguntas e respostas geradas.

   ![](assets/question-generation-9.png)

## Endereços IP para Incluir na lista de permissões {#ip-addresses-to-allowlist}

Incluir na lista de permissões Para habilitar a extração de conteúdo dos URLs da Web durante a geração de perguntas e respostas, localize sua região abaixo e verifique se o endereço IP associado a ele é gravado pela equipe da Web.

<table width="450">
<thead>
  <tr>
    <th>América do Norte</th>
    <th>Europa</th>
    <th>APAC</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>13.68.17.252</td>
    <td>20.105.150.224</td>
    <td>20.213.91.77</td>
  </tr>
</tbody>
</table>
