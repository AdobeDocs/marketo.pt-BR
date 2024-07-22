---
unique-page-id: 14352514
description: Como O Sales Connect Lida Com A Eliminação Da Duplicação De Email - Documentação Do Marketo - Documentação Do Produto
title: Como o Sales Connect lida com a eliminação da duplicação de email
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Como o Sales Connect lida com a eliminação da duplicação de email {#how-sales-connect-handles-email-de-duping}

Quando você está [carregando um arquivo CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) no Sales Connect, mesclamos todos os contatos semelhantes no CSV antes da importação.

Fazemos isso com base em endereços de email semelhantes. Portanto, se houver dois endereços de email idênticos, nós os mesclamos em um contato.

Posteriormente, se você tentar adicionar/carregar manualmente o mesmo contato, não o mesclaremos.

Se você tentar adicionar um contato que já está em seu banco de dados, impediremos que você o adicione.
