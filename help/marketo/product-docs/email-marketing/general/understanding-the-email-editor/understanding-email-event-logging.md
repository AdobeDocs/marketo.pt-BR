---
unique-page-id: 1147356
description: Saiba mais sobre o registro de eventos de email no Marketo. Entenda como aberturas, cliques e outros eventos são rastreados e armazenados.
title: Noções básicas sobre o registro de eventos de email
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
feature: Email Editor
TQID: 'https://experienceleague.adobe.com/7ldlXmnupXohvFUDiniYCV9Idn1zOMUuynPneV5ovLY'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: eeae636f-f283-4051-94f0-4d74945464fb
    internal-label: Email Editor
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 3%
---
# Noções básicas sobre o registro de eventos de email {#understanding-email-event-logging}

Ao enviar emails, o Marketo registra diferentes pontos de dados nos logs de atividades da pessoa. Aqui estão as básicas.

| Evento | Descrição |
|---|---|
| [!UICONTROL Enviado] | É registrado sempre que um email é enviado dos servidores da Marketo, independentemente de ser realmente entregue. Os emails devolvidos ainda são registrados como &quot;Enviados&quot;. |
| [!UICONTROL Entregue] | É registrado sempre que um email é aceito pelo servidor de email do recipient. Isso não significa que ele evitou filtros de spam. Só pode haver 1 delivery para cada email enviado. |
| [!UICONTROL Devolvido(s) Fortemente] | Algumas rejeições permanentes são o resultado de bloqueios de spam, portanto, não tentaremos enviar um email para essa pessoa por 24 horas em nenhuma campanha. Outras rejeições permanentes, como caixas de entrada não existentes, são permanentes e nunca enviaremos um email para a pessoa novamente de qualquer campanha. |
| [!UICONTROL Devolvido(S) Temporariamente] | É registrado quando uma resposta do servidor não está clara, caixa de correio cheia ou problemas gerais do servidor. Colocamos essas pessoas em uma lógica de nova tentativa por 24 a 36 horas para uma possível entrega futura. Isso não desqualifica a pessoa de outras correspondências. |
| [!UICONTROL Aberto] | É registrado quando um recipient exibe um email com imagens NÃO bloqueadas. Somente um evento aberto por email, por pessoa, por campanha inteligente é registrado. Se abrirem o mesmo email duas vezes em sua caixa de entrada, ele não será registrado mais de uma vez. |
| [!UICONTROL Clicado] | É registrado sempre que um URL decorado do email é carregado no navegador (o resultado do clique no link ). Normalmente, é o clique do recipient, mas também pode ser recortar/colar. |
| [!UICONTROL Cancelamento de assinatura] | É registrado quando uma pessoa clica no link de cancelamento de inscrição de um email e envia o formulário de cancelamento de inscrição. |

>[!CAUTION]
>
>Se o mesmo email for enviado para a mesma pessoa duas vezes da mesma campanha, o evento **[!UICONTROL Aberto]** será registrado no máximo 1 vez.
