---
unique-page-id: 14352514
description: Como O Sales Connect Lida Com A Eliminação Da Duplicação De Email - Documentação Do Marketo - Documentação Do Produto
title: Como o Sales Connect lida com a eliminação de duplicações de email
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 6%

---

# Como O [!DNL Sales Connect] Lida Com A Eliminação Da Duplicação De Emails {#how-sales-connect-handles-email-de-duping}

Quando você está [carregando um arquivo CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) no [!DNL Sales Connect], mesclamos todos os contatos semelhantes no CSV antes da importação.

Fazemos isso com base em endereços de email semelhantes. Portanto, se houver dois endereços de email idênticos, nós os mesclamos em um contato.

Posteriormente, se você tentar adicionar/carregar manualmente o mesmo contato, não o mesclaremos.

Se você tentar adicionar um contato que já está em seu banco de dados, impediremos que você o adicione.
