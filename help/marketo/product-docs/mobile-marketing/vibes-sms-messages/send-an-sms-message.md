---
description: Enviar uma mensagem SMS - Documentação do Marketo - Documentação do produto
title: Enviar uma mensagem SMS
feature: Mobile Marketing
exl-id: 2c863ded-f441-4217-9541-6dcc442d9831
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Enviar uma mensagem SMS {#send-a-vibes-sms-message}

Você [criou sua mensagem SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, agora é hora de enviá-la. Você pode enviá-lo por Lote ou Acionar a campanha.

>[!NOTE]
>
>Ao enviar mensagens SMS:
>
>* Desduplicação de Marketo Engage por número de telefone. Assim, se várias pessoas tiverem o mesmo número de telefone, somente uma pessoa receberá a mensagem se for membro de apenas uma lista de assinaturas Vibes. A desduplicação é feita no nível da lista de assinaturas Vibes, não no nível do programa Marketo.
>* O Marketo incluir na lista de bloqueios não enviará para as pessoas que estão aprovadas ou com suspensão de marketing.
>* Uma mensagem SMS não enviará a ninguém que tenha cancelado a assinatura se não estiver na lista do banco de dados móvel do Vibes.

## Enviar um SMS em lote {#send-a-batch-sms}

1. Em Minha Marketo, clique em **Atividades de marketing**.

   ![](assets/send-an-sms-message-1.png)

1. Localize e selecione a Campanha inteligente desejada.

   ![](assets/send-an-sms-message-2.png)

1. Clique na guia **Smart List** e defina o público-alvo do SMS. Neste exemplo, estamos enviando para todos em nosso banco de dados que têm &quot;Adobe&quot; listado como sua empresa.

   ![](assets/send-an-sms-message-3.png)

1. Na guia **Fluxo**, arraste por **Enviar Mensagem SMS**. Selecione a lista de mensagens e vibrações SMS desejada nos menus suspensos.

   ![](assets/send-an-sms-message-4.png)

   >[!NOTE]
   >
   >O seletor da Lista de vibrações atua como um filtro adicional para o público-alvo já identificado na Lista inteligente para direcionar somente as pessoas que pertencem a essa lista de vibrações.

1. Clique na guia **Agendar** e agende seu SMS.

   ![](assets/send-an-sms-message-5.png)

## Enviar um SMS de acionador {#send-a-trigger-sms}

1. Em Minha Marketo, clique em **Atividades de marketing**.

   ![](assets/send-an-sms-message-6.png)

1. Localize e selecione a Campanha inteligente desejada.

   ![](assets/send-an-sms-message-7.png)

1. Clique na guia **Smart List**, selecione o acionador desejado e defina seu valor. Neste exemplo, estamos usando o **Formulário de Preenchimento**.

   ![](assets/send-an-sms-message-8.png)

1. Na guia **Fluxo**, arraste por **Enviar Mensagem SMS**. Selecione a lista de mensagens e vibrações SMS desejada nos menus suspensos.

   ![](assets/send-an-sms-message-9.png)

   >[!NOTE]
   >
   >O seletor da Lista de vibrações atua como um filtro adicional para o público-alvo já identificado na Lista inteligente para direcionar somente as pessoas que pertencem a essa lista de vibrações.

1. Clique na guia **Agendar** e em **Ativar**.

   ![](assets/send-an-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Criar uma mensagem de vibrações](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}
>* [Usando Opções de SMS em uma Campanha Inteligente](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/using-sms-options-in-a-smart-campaign.md){target="_blank"}
