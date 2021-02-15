---
unique-page-id: 14352514
description: Como o Sales Connect lida com a remoção de e-mails - Documentos do Marketing - Documentação do produto
title: Como o Sales Connect lida com a remoção de mensagens por email
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---


# Como o Sales Connect lida com a remoção de e-mail {#how-sales-connect-handles-email-de-duping}

Quando você estiver [carregando um arquivo CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) no Sales Connect, nós unimos todos os contatos semelhantes no CSV antes que a importação ocorra.

Fazemos isso com base em endereços de email similares. Portanto, se houver dois endereços de email idênticos, nós os mesclamos em um único contato.

Se você tentar adicionar/carregar manualmente o mesmo contato mais tarde, nós não o mesclaremos.

Se tentar adicionar um contato que já esteja no banco de dados, evitaremos que você o adicione.
