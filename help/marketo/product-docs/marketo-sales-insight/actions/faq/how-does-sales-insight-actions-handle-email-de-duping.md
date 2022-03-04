---
description: Como as ações de insight de vendas lidam com a remoção de e-mails - Documentos do Marketo - Documentação do produto
title: Como as ações de insight de vendas lidam com a remoção de emails
hide: true
hidefromtoc: true
source-git-commit: 47b0f31b410f0bf4b41740aa6440c2a0484ab835
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# Como As Ações De Insight De Vendas Lidam Com A Eliminação De Emails? {#how-does-sales-insight-actions-handle-email-de-duping}

Quando você estiver [upload de um CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) nas Ações de insight de vendas, unimos todos os contatos semelhantes no CSV antes que a importação ocorra.

Fazemos isso com base no mesmo endereço de email. Portanto, se houver dois endereços de email idênticos, os mesclamos em um único contato.

Posteriormente, se você tentar adicionar/carregar manualmente o mesmo contato, não o mesclaremos.

Se tentar adicionar um contato que já esteja no banco de dados, impediremos que você o adicione.
