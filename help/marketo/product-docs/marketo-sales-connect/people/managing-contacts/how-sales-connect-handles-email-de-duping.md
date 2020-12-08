---
unique-page-id: 14352514
description: Como o Sales Connect lida com a remoção de e-mails - Documentos do Marketing - Documentação do produto
title: Como o Sales Connect lida com a remoção de mensagens por email
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# Como o Sales Connect lida com a remoção de mensagens por email {#how-sales-connect-handles-email-de-duping}

Quando você está [fazendo upload de um arquivo CSV](http://docs.marketo.com/x/VADb) no Sales Connect, nós mesclamos todos os contatos semelhantes no CSV antes da importação.

Fazemos isso com base em endereços de email similares. Portanto, se houver dois endereços de email idênticos, nós os mesclamos em um único contato.

Se você tentar adicionar/carregar manualmente o mesmo contato mais tarde, nós não o mesclaremos.

Se tentar adicionar um contato que já esteja no banco de dados, evitaremos que você o adicione.

