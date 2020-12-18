---
unique-page-id: 10096677
description: Teste a integração do Evento ON24 - Documentos do Marketing - Documentação do produto
title: Teste sua integração de Evento ON24
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Teste sua integração de Evento ON24 {#test-your-on-event-integration}

Certifique-se de testar a integração do evento completamente.

## Sequência de teste recomendada antes de executar sua primeira Campanha {#recommended-test-sequence-before-running-your-first-campaign}

1. Preencha o formulário de inscrição do evento e use um endereço de email válido para testar.
1. Confirme se o nome do teste é exibido com um status **Registered** na grade Membros do evento de marketing.
1. Confirme se o nome do teste também aparece como **Registrado** em ON24.
1. Confirme se o endereço de email válido que você usou para registrar o nome do teste recebeu um email de confirmação para o Evento e se o URL exclusivo foi resolvido no email.

   >[!NOTE]
   >
   >Você deve usar o token `{{member.webinar url}}` em seu email de confirmação para que o URL exclusivo seja exibido no email de cada registrante.

## Após o Evento {#after-the-event}

Veja como os dados são atualizados depois que o evento acontece:

* O Marketo recupera dados de participantes do ON24 todas as noites.
* Quando os dados do participante forem sincronizados entre Marketo e ON24, o Marketo atualizará o status de associação para Participante, Participante sob demanda ou Não mostrar. Na guia evento **Resumo**, o status do evento é atualizado para **Evento Concluído**.

>[!MORELIKETHIS]
>
>* [Exemplo de integração de Evento ON24](example-on24-event-integration.md)
>* [Noções Gerais dos Eventos do adaptador do Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



