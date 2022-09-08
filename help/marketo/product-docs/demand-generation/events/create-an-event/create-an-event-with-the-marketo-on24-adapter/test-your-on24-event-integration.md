---
unique-page-id: 10096677
description: Teste sua integração de evento ON24 - Documentos da Marketo - Documentação do produto
title: Teste sua integração de evento ON24
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Teste sua integração de evento ON24 {#test-your-on-event-integration}

>[!IMPORTANT]
>
>A partir de agosto de 2022, o ON24 não será mais compatível com novas integrações do Marketo. As informações neste artigo se aplicam apenas aos usuários existentes.

Teste a integração do evento completamente.

## Sequência De Teste Recomendada Antes De Executar Sua Primeira Campanha {#recommended-test-sequence-before-running-your-first-campaign}

1. Preencha o formulário de registro do evento e use um endereço de email válido para testar.
1. Confirme se o nome do teste é exibido com uma **Registrado** na grade Associação do evento do Marketo.
1. Confirme se o nome do teste também é exibido como **Registrado** em ON24.
1. Confirme se o endereço de email válido usado para registrar o nome de teste recebeu um email de confirmação para o Evento e se o URL exclusivo foi resolvido no email.

   >[!NOTE]
   >
   >Você deve usar o `{{member.webinar url}}` token no email de confirmação para que o URL único seja exibido no email de cada registrando.

## Após o evento {#after-the-event}

Veja como os dados são atualizados após o evento ocorrer:

* O Marketo recupera dados de participantes do ON24 todas as noites.
* Depois que os dados do participante forem sincronizados entre o Marketo e o ON24, a Marketo atualizará o status de associação para Participado, Participado sob demanda ou Sem programa. No **Resumo** , o status do evento é atualizado para **Evento concluído**.

>[!MORELIKETHIS]
>
>* [Exemplo de integração de evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [Noções básicas sobre os eventos do adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)

