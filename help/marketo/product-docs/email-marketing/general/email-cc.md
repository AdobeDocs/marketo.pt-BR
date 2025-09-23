---
unique-page-id: 17727995
description: Email CC - Documentação do Marketo - Documentação do produto
title: Email em cópia (CC)
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 1%

---

# Email em cópia (CC) {#email-cc}

Email CC permite que emails especificados enviados pelo Marketo incluam recipients CC.

Esse recurso está disponível em todos os ativos de email do Marketo, independentemente de como o email é enviado (campanha em lote ou de acionador). O recipient CC receberá uma cópia exata do email enviado para a pessoa escolhida do Marketo. Dessa forma, qualquer atividade de engajamento (aberturas, cliques etc.) será registrada no log de atividades da pessoa do Marketo na linha &quot;Para&quot; do email. No entanto, a atividade de entrega (enviada, entregue, rejeição permanente, etc.) _diferente de &quot;rejeição temporária&quot;_ **não** será registrada, pois a Marketo não pode distinguir os eventos de entrega para a Pessoa Marketo dos destinatários CC. A Marketo só terá CC de até 100.000 pessoas por vez. Se sua lista inteligente exceder 100k e for imperativo que cada pessoa nela tenha CCd, recomendamos dividir sua lista.

>[!NOTE]
>
>O Email CC não foi projetado para ser usado com Testes A/B. Você pode usá-lo de qualquer maneira se desejar. No entanto, como não é tecnicamente suportado, o Suporte da Marketo não poderá ajudá-lo com nenhuma solução de problemas.

## Configurar Email CC {#set-up-email-cc}

1. Em Minha Marketo, clique em **[!UICONTROL Administrador]**.

   ![](assets/one.png)

1. Na árvore, selecione **[!UICONTROL Email]**.

   ![](assets/two.png)

1. Clique em **[!UICONTROL Editar configurações de email CC]**.

   ![](assets/three.png)

1. Selecione até 25 campos de Líder ou Empresa do Marketo (do tipo &quot;Email&quot;) para disponibilizar para uso como endereços CC em emails. Clique em **Salvar** quando terminar.

   ![](assets/four.png)

## Usando o Email CC {#using-email-cc}

1. Selecione seu email e clique em **[!UICONTROL Editar Rascunho]**.

   ![](assets/five.png)

1. Clique em **[!UICONTROL Configurações de email]**.

   ![](assets/six.png)

1. Selecione os campos que deseja usar para CC de pessoas. _Há um limite de cinco por email_. Neste exemplo, queremos apenas o CC do proprietário do lead. Clique em **Salvar** ao concluir.

   ![](assets/seven.png)

   É tão simples quanto isso! No exemplo acima, ao enviar o email, o Proprietário principal dos destinatários escolhidos será CCd.

   >[!NOTE]
   >
   >Se um endereço de email inválido estiver em um campo CC, ele será ignorado.

   Para identificação rápida, a visualização Resumo de email mostra se/quais campos de Email CC foram selecionados.

   ![](assets/eight.png)

   Se o email for aprovado, mas o Administrador do Marketo desabilitar um ou mais campos CC antes do email ser enviado, **essas pessoas não receberão um email**. Nesse cenário, a visualização Resumo de email esmaecerá todos os campos que foram desativados após a aprovação, mas foram pré-enviados:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >Você também verá o erro acima na seção Configurações de email do rascunho de email.

## Após o envio {#after-the-send}

* Se um recipient CC clicar em um link rastreado no email, a atividade de clique (como todas as outras atividades de engajamento) será associada ao recipient principal do email. Além disso, eles podem clicar para acessar uma página com o código de rastreamento Web do Marketo (munchkin.js), fazendo com que sejam diagnosticados como o recipient principal.

>[!TIP]
>
>Você tem a opção de [desabilitar alguns ou todos os links de rastreamento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) em um email.

* Depois que uma campanha de email for executada, a atividade Enviar email incluirá uma lista de todos os endereços CC incluídos para cada destinatário da correspondência. Se algum endereço CC for ignorado devido ao cancelamento de inscrição, ele também será anotado na atividade.
* Os links para cancelar a inscrição e as páginas funcionam normalmente em emails com CCd. Isso permite que os recipients do CC cancelem a inscrição com êxito, se desejarem (em conformidade com as regulamentações antisspam), e um registro dessa ação será armazenado no Banco de dados do Marketo.
* As pessoas listadas como não inscritas no banco de dados do Marketo **não** receberão emails via CC.
