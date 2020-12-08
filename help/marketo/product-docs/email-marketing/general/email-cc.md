---
unique-page-id: 17727995
description: Email CC - Documentos do Marketing Cloud - Documentação do produto
title: Email CC
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---


# Email CC {#email-cc}

O Email CC permite que emails especificados sejam enviados pelo Marketo para incluir recipient CC.

Este recurso está disponível em todos os ativos de email do Marketing para, independentemente de como o email é enviado (campanha de lote ou acionador). O recipient CC receberá uma cópia exata do e-mail enviado à pessoa selecionada do Marketing Cloud. Dessa forma, qualquer atividade de envolvimento (abre, clica etc.) será registrado no registro de atividades da Pessoa de marketing na linha &quot;Para&quot; do email. No entanto, a atividade do delivery (enviada, entregue, rejeição em disco, etc.) *diferente de &quot;salto suave&quot;* **não** será registrado, pois o Marketo não é capaz de distinguir eventos de delivery para a Pessoa de marketing dos recipient CC. O Marketo só contará com até 100 mil pessoas por vez. Se sua lista inteligente exceder 100 mil e for imperativo que cada pessoa nela tenha CC&#39;d, recomendamos quebrar sua lista.

>[!NOTE]
>
>O Email CC não foi projetado para ser usado com testes A/B. Você pode usá-lo mesmo assim se desejar, no entanto, como tecnicamente não é suportado, o suporte do Marketo não seria capaz de ajudar em qualquer solução de problemas.

## Configurar Email CC {#set-up-email-cc}

1. Em Meu Marketo, clique em **Admin**.

   ![](assets/one.png)

1. Na árvore, selecione **Email**.

   ![](assets/two.png)

1. Clique em **Editar configurações** de e-mail CC.

   ![](assets/three.png)

1. Selecione até 25 campos de venda ou Empresa (do tipo &quot;Email&quot;) para disponibilizar para uso como endereços CC em emails. Clique em **Salvar** quando concluído.

   ![](assets/four.png)

## Uso do Email CC {#using-email-cc}

1. Selecione seu email e clique em **Editar rascunho**.

   ![](assets/five.png)

1. Clique em Configurações **de** email.

   ![](assets/six.png)

1. Selecione até cinco campos que deseja usar para CCs. Neste exemplo, só queremos a CC do proprietário principal. Clique em **Salvar** quando concluído.

   ![](assets/seven.png)

   É tão simples quanto isso! No exemplo acima, ao enviar o email, o Proprietário Principal dos recipient escolhidos será CC&#39;d.

   >[!NOTE]
   >
   >
   >Se um endereço de email inválido estiver em um campo CC, ele será ignorado.

   Para uma identificação rápida, a visualização Resumo do email mostra se/quais campos de Email CC foram selecionados.  ![](assets/eight.png)

   Se o email for aprovado, mas o Administrador de marketing desativar um ou mais campos CC antes do email ser enviado, **essas pessoas não receberão um email**. Nesse cenário, a visualização Resumo de email cinza todos os campos que foram desativados após a aprovação, mas pré-enviados:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >Você também verá o erro acima na seção Configurações de e-mail do rascunho do e-mail.

## Após o envio {#after-the-send}

* Se um recipient CC clicar em um link rastreado no email, clique em atividade (como toda a atividade de envolvimento) será associado ao recipient principal do email. Além disso, eles podem clicar até uma página com o código de rastreamento da Web do Marketo (munchkin.js), fazendo com que eles sejam cookies como o recipient principal.

>[!TIP]
>
>Você tem a opção de [desativar alguns ou todos os links](http://docs.marketo.com/x/IwAd) de rastreamento em um email.

* Depois que uma campanha de email é executada, a atividade Enviar email incluirá uma lista de todos os endereços CC que foram incluídos para cada recipient do correio. Se algum endereço CC foi ignorado devido ao cancelamento da inscrição, ele também será anotado na atividade.
* Os links e páginas de cancelamento de assinatura funcionam normalmente em emails CC&#39;d. Isso permite que os recipient da CC cancelem a assinatura com êxito se desejarem (em conformidade com as regulamentações antisspam), e um registro dessa ação será armazenado no Banco de Dados do Marketing.
* As pessoas que estão listadas como não assinadas no seu Banco de Dados de Marketing **não** receberão emails via CC.

