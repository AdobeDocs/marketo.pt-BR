---
description: Usar mensagens SMS de vibrações em acionadores e filtros de lista inteligente - Documentação do Marketo - Documentação do produto
title: Usar mensagens SMS de vibrações em acionadores e filtros de lista inteligente
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Usar mensagens SMS de vibrações em acionadores e filtros de lista inteligente {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Depois de [criar uma mensagem SMS do Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"}, você deverá usar os disparadores e filtros da Smart List em uma Campanha Inteligente para obter os benefícios. Veja como.

1. Em Minha Marketo, clique em **[!UICONTROL Atividades de marketing]**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Escolha uma Campanha inteligente na qual você deseja usar seus ativos de SMS. Arraste sobre um acionador. Neste exemplo, estamos usando o **Formulário de Preenchimento**.

   ![](assets/fills-out-form-pull-over.jpg)

## Acionadores de SMS {#sms-triggers}

Há outros acionadores de SMS disponíveis. Os acionadores de SMS são exibidos somente se o serviço Vibes estiver ativado.

ENVIAR UMA MENSAGEM SMS:

* Atividades de marketing > escolher nova campanha inteligente
   * Smart List > Escolher filtro da lista de vibrações e lógica correta > lista de vibrações: escolha a lista na lista suspensa (lista de banco de dados móvel que é sincronizada a partir da plataforma Vibes)
      * Podem refinar a segmentação e utilizar filtros e acionadores de SMS e de email em uma campanha
      * Filtros de vibrações: inscrito na lista de vibrações vs. membro da lista de vibrações - a lógica é consistente com o email
         * Inscrito na lista de vibrações - participantes que já se inscreveram nessa lista mesmo que tenham cancelado a inscrição.  - usado principalmente para esforços de marketing entre canais
            * Observação: uma mensagem SMS não enviará a ninguém que tenha cancelado a assinatura se não estiver na lista do banco de dados móvel do Vibes
         * Membro da Lista de Vibes - assinante ativo e confirmado
         * Adicionado à lista - as listas de vibrações não serão preenchidas com esse filtro; isso é para listas do Marketo

![](assets/new-sms-search2.png)

Veja alguns exemplos:

O gatilho **Rejeições de Mensagens SMS** inicia um fluxo, como o envio de um email, quando uma mensagem SMS é rejeitada.

![](assets/sms-message-bounces-real.jpg)

O gatilho **[!UICONTROL Inscreve-se na Lista de Vibrações]** inicia um fluxo quando uma pessoa se inscreve.

![](assets/subscribes-to-vibes-list-real.jpg)

O acionador **[!UICONTROL Link de Cliques na Mensagem SMS]** inicia um fluxo quando uma pessoa clica em um link na mensagem SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtros de SMS {#sms-filters}

Você também pode usar filtros de Vibes em listas inteligentes. O filtro **[!UICONTROL Inscrito na Lista de Vibrações]** encontra qualquer pessoa que *já* tenha inscrito nas Vibes. Isso inclui pessoas canceladas e excluídas, mesmo que as pessoas excluídas sejam omitidas do fluxo. Esse filtro é mais adequado para relatórios.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Por outro lado, o filtro **Membro da Lista de Vibrações** encontra *qualquer pessoa* inscrita atualmente nas Vibes e é mais adequado para uso em Campanhas ou listas inteligentes.

![](assets/image001.png)

>[!NOTE]
>
>Todos os filtros SMS incluem a restrição **[!UICONTROL Data de Atividade]** por padrão.

Após configurar os disparadores e filtros de Vibes na sua lista inteligente, você pode [definir o fluxo](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definir lista inteligente para campanha inteligente | Acionador](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Localizar e Adicionar Filtros a uma Lista Inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
