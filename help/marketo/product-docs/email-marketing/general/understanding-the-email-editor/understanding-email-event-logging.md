---
unique-page-id: 1147356
description: Como entender o registro de Eventos por email - Documentos do Marketing - Documentação do produto
title: Como entender o registro de Eventos por email
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---


# Como entender o registro de Eventos por email {#understanding-email-event-logging}

Ao enviar emails, o Marketo registra diferentes pontos de dados nos registros de atividades da pessoa. Aqui estão os mais básicos.

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

| Evento | Descrição |
|---|---|
| Enviados | É registrado sempre que um email é enviado dos servidores de marketing, independentemente de ser realmente entregue. E-mails salvos ainda são registrados como &quot;Enviados&quot;. |
| Entregue | É registrado sempre que um e-mail é aceito pelo servidor de e-mail do recipient. Isso não significa que tenha evitado filtros de spam. Só pode haver 1 delivery para cada email enviado. |
| Disparado intenso | Algumas rejeições são resultado de blocos de spam, então não tentaremos enviar um email para essa pessoa por 24 horas em nenhuma campanha. Outras rejeições difíceis como caixas de entrada inexistentes são permanentes, e nunca mais enviaremos email para a pessoa de nenhuma campanha. |
| Rejeitado macio | É registrado quando uma resposta do servidor não está clara, a caixa de correio está cheia ou apresenta problemas gerais ao servidor. Nós colocamos essas pessoas através de uma lógica de repetição por 24 a 36 horas para um potencial delivery futuro. Isso não desqualifica a pessoa de outras correspondências. |
| Aberto | É registrado quando um recipient visualização um email com imagens NÃO bloqueadas. Somente um evento aberto por email, por pessoa, por campanha inteligente é registrado. Se eles abrirem o mesmo email de sua caixa de entrada duas vezes, ele não será registrado mais de uma vez. |
| Clicado | É registrado sempre que um URL decorado do email é carregado no navegador (o resultado de clicar no link). Geralmente, esse é o clique do recipient, mas também pode ser um recorte/colagem. |
| Inscrito | É registrado quando uma pessoa clica no link para cancelar a assinatura de um email e envia o formulário de cancelamento de assinatura. |

>[!CAUTION]
>
>Se o mesmo email for enviado para a mesma pessoa duas vezes da mesma campanha, o evento **Aberto** será registrado no máximo 1 vez.

