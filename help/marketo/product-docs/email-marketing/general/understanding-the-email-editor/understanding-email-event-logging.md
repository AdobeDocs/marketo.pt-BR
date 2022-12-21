---
unique-page-id: 1147356
description: Como entender o registro de eventos de email - Documentos do Marketo - Documentação do produto
title: Como entender o registro de eventos de email
exl-id: 107d7f4a-ad38-44e4-95d8-760539aacede
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 3%

---

# Como entender o registro de eventos de email {#understanding-email-event-logging}

Ao enviar emails, o Marketo registra diferentes pontos de dados nos registros de atividades da pessoa. Aqui estão os básicos.

| Evento | Descrição |
|---|---|
| Enviado | É registrado sempre que um email é enviado dos servidores da Marketo, independentemente de ser realmente entregue. Os emails devolvidos ainda são registrados como &quot;Enviados&quot;. |
| Entregue | É registrado sempre que um email é aceito pelo servidor de email do recipient. Isso não significa que tenha evitado filtros de spam. Só pode haver 1 delivery para cada email enviado. |
| Devolvido permanentemente | Algumas devoluções permanentes são resultado de blocos de spam, então não tentaremos enviar um email para essa pessoa por 24 horas em nenhuma campanha. Outras devoluções permanentes, como caixas de entrada inexistentes, são permanentes e nunca mais enviaremos um email para a pessoa de qualquer campanha. |
| Devolvido temporariamente | É registrado quando uma resposta do servidor não é clara, a caixa de correio está cheia ou problemas gerais do servidor. Colocamos essas pessoas com uma lógica de repetição por 24 a 36 horas para uma possível entrega futura. Isso não desqualifica a pessoa de outras correspondências. |
| Aberto | É registrado quando um recipient exibe um email com imagens NÃO bloqueadas. Somente um evento aberto por email, por pessoa, por campanha inteligente é registrado. Se eles abrirem o mesmo email de sua caixa de entrada duas vezes, ele não será registrado mais de uma vez. |
| Clicado | É registrado sempre que um URL decorado do email é carregado no navegador (o resultado de clicar no link). Geralmente, esse é o recipient que clica, mas também pode ser um recorte/colar. |
| Inscrição cancelada | É registrado quando uma pessoa clica no link de cancelamento de inscrição de um email e envia o formulário de cancelamento de inscrição. |

>[!CAUTION]
>
>Se o mesmo email for enviado para a mesma pessoa duas vezes da mesma campanha, a variável **Aberto** será registrado no máximo 1 vez.
