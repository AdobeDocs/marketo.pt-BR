---
unique-page-id: 17727995
description: Email CC - Documentação do Marketo - Documentação do produto
title: Email CC
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Email CC {#email-cc}

A CC de email permite que emails especificados sejam enviados pelo Marketo para incluir recipients da CC.

Esse recurso está disponível em todos os ativos de email do Marketo, independentemente de como o email é enviado (campanha em lote ou acionador). O destinatário da CC receberá uma cópia exata do email enviado para a pessoa escolhida do Marketo. Dessa forma, qualquer atividade de envolvimento (aberturas, cliques etc.) será conectado ao registro de atividades da Marketo Person na linha &quot;To&quot; do email. No entanto, a atividade de delivery (enviada, entregue, devolução permanente etc.) _exceto &quot;devolução temporária&quot;_ will **not** registre-se, pois o Marketo não é capaz de distinguir os eventos de delivery da Marketo Person dos recipients do CC. A Marketo só terá até 100 mil pessoas por vez. Se sua lista inteligente excede 100k e é imperativo que todas as pessoas nela tenham CC&#39;d, recomendamos quebrar sua lista.

>[!NOTE]
>
>O CC de email não foi projetado para ser usado com Testes A/B. Você pode usá-lo de qualquer maneira se desejar, no entanto como tecnicamente não é compatível, o Suporte da Marketo não poderá ajudar em nenhuma solução de problemas.

## Configurar Email CC {#set-up-email-cc}

1. Em Minha Marketo, clique em **Administrador**.

   ![](assets/one.png)

1. Na árvore, selecione **Email**.

   ![](assets/two.png)

1. Clique em **Editar configurações de email CC**.

   ![](assets/three.png)

1. Selecione até 25 campos Marketo Lead ou Company (do tipo &quot;Email&quot;) para disponibilizar para uso como endereços CC em emails. Clique em **Salvar** quando concluído.

   ![](assets/four.png)

## Uso do Email CC {#using-email-cc}

1. Selecione seu email e clique em **Editar rascunho**.

   ![](assets/five.png)

1. Clique em **Configurações de email**.

   ![](assets/six.png)

1. Selecione até cinco campos que deseja usar para CCs. Neste exemplo, queremos apenas os CCs do Proprietário Principal. Clique em **Salvar** quando concluído.

   ![](assets/seven.png)

   É tão simples assim! No exemplo acima, ao enviar o email, o Proprietário principal dos recipients que você escolheu será CC&#39;d.

   >[!NOTE]
   >
   >Se um endereço de email inválido estiver em um campo CC, ele será ignorado.

   Para identificação rápida, a exibição Resumo de email mostra se/quais campos CC de email foram selecionados.

   ![](assets/eight.png)

   Se o email for aprovado, mas o Marketo Admin desabilitar um ou mais campos CC antes que o email seja enviado, **essas pessoas não receberão um email**. Nesse cenário, a exibição Resumo de email esmaecerá todos os campos que foram desativados após a aprovação, mas pré-enviam:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >Você também verá o erro acima na seção Configurações de email do rascunho de email.

## Após o envio {#after-the-send}

* Se um recipient CC clicar em um link rastreado no email, clique em atividade (como todas as outras atividades de envolvimento) será associado ao recipient principal do email. Além disso, eles podem clicar em até uma página com o código de rastreamento Web do Marketo (munchkin.js), fazendo com que eles sejam cookies como o recipient principal.

>[!TIP]
>
>Você tem a opção de [desativação de alguns ou todos os links de rastreamento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) em um email.

* Após a execução de uma campanha de email, a atividade Enviar email incluirá uma lista de todos os endereços CC incluídos para cada recipient da correspondência. Se algum endereço CC foi ignorado devido ao cancelamento de inscrição, ele também será observado na atividade .
* Cancele a assinatura de links e páginas normalmente em emails do CCd. Isso permite que os recipients do CC cancelem a assinatura com êxito se desejarem (em conformidade com as regulamentações antisspam) e um registro dessa ação será armazenado no banco de dados do Marketo.
* As pessoas listadas como canceladas na assinatura no seu banco de dados do Marketo serão **not** receba emails via CC.
