---
description: Como As Ações Do Sales Insight Lidam Com A Eliminação Da Duplicação De Emails - Documentação Do Marketo - Documentação Do Produto
title: Como as ações do Sales Insight lidam com a eliminação da duplicação de email
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Como As Ações Do Sales Insight Lidam Com A Eliminação Da Duplicação De Emails? {#how-does-sales-insight-actions-handle-email-de-duping}

Quando você está [carregando um arquivo CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) no Sales Insight Actions, mesclamos todos os contatos semelhantes no CSV antes da importação.

Fazemos isso com base em endereços de email semelhantes. Portanto, se houver dois endereços de email idênticos, nós os mesclamos em um contato.

Posteriormente, se você tentar adicionar/carregar manualmente o mesmo contato, não o mesclaremos.

Se você tentar adicionar um contato que já está em seu banco de dados, impediremos que você o adicione.
