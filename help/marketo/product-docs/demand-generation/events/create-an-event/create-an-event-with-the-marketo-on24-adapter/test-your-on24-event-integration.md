---
unique-page-id: 10096677
description: Teste a integração do evento ON24 - Documentação do Marketo - Documentação do produto
title: Teste a integração do evento ON24
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Teste a integração do evento ON24 {#test-your-on-event-integration}

Certifique-se de testar completamente a integração do evento.

## Sequência De Teste Recomendada Antes De Executar A Primeira Campanha {#recommended-test-sequence-before-running-your-first-campaign}

1. Preencha o formulário de registro do evento e use um endereço de email válido para testar.
1. Confirme se o nome do teste aparece com o status **Registrado** na grade de associação do seu evento Marketo.
1. Confirme se o nome do teste também aparece como **Registrado** no ON24.
1. Confirme se o endereço de email válido que você usou para registrar o nome de teste recebeu um email de confirmação para o Evento e se o URL exclusivo foi resolvido no email.

   >[!NOTE]
   >
   >Você deve usar o token `{{member.webinar url}}` no email de confirmação para que o URL exclusivo seja exibido no email de cada inscrito.

## Após o evento {#after-the-event}

Veja como os dados são atualizados após a ocorrência do evento:

* O Marketo recupera os dados dos participantes do ON24 todas as noites.
* Depois que os dados do participante forem sincronizados entre o Marketo e o ON24, o Marketo atualizará o status da associação para Participou, Participou sob demanda ou Não apareceu. Na guia **Resumo** do evento, o status do evento é atualizado para **Evento concluído**.

>[!MORELIKETHIS]
>
>* [Exemplo de Integração de Eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Noções Básicas sobre os Eventos do Adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
