---
unique-page-id: 14352514
description: Entenda como o Sales Connect lida com a eliminação de duplicação de email. Saiba como os contatos duplicados são mesclados ou tratados durante a sincronização.
title: Como o Sales Connect lida com a eliminação de duplicações de email
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/gO6I2rCotAEDOGQNdRleeJbqMIix1wQizZe84JZSLPs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 107
ht-degree: 6%

---

# Como O [!DNL Sales Connect] Lida Com A Eliminação Da Duplicação De Emails {#how-sales-connect-handles-email-de-duping}

Quando você está [carregando um arquivo CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) no [!DNL Sales Connect], mesclamos todos os contatos semelhantes no CSV antes da importação.

Fazemos isso com base em endereços de email semelhantes. Portanto, se houver dois endereços de email idênticos, nós os mesclamos em um contato.

Posteriormente, se você tentar adicionar/carregar manualmente o mesmo contato, não o mesclaremos.

Se você tentar adicionar um contato que já está em seu banco de dados, impediremos que você o adicione.
