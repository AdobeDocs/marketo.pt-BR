---
unique-page-id: 14352514
description: Como o Sales Connect lida com a remoção de e-mails - Documentos da Marketo - Documentação do produto
title: Como o Sales Connect lida com a remoção de e-mails
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Como o Sales Connect lida com a remoção de e-mails {#how-sales-connect-handles-email-de-duping}

Quando você estiver [upload de um CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) no Sales Connect, unimos todos os contatos semelhantes no CSV antes que a importação ocorra.

Fazemos isso com base no mesmo endereço de email. Portanto, se houver dois endereços de email idênticos, os mesclamos em um único contato.

Posteriormente, se você tentar adicionar/carregar manualmente o mesmo contato, não o mesclaremos.

Se tentar adicionar um contato que já esteja no banco de dados, impediremos que você o adicione.
