---
unique-page-id: 2953188
description: Saiba mais sobre filtros inferidos em Smart Lists. Entenda como o Marketo infere filtros de ativos vinculados.
title: Filtros inferidos
exl-id: 6db4ff4d-7fab-4722-94b1-1bf92ba4651d
feature: Smart Lists
TQID: https://experienceleague.adobe.com/-dKeAfCxfD1ErbfBzLqARUMwFY-I9RdkWGC0b-ZtNyE
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 218
ht-degree: 1%

---

# Filtros inferidos {#inferred-filters}

Quando alguém visita o seu site, o [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} faz o cookie e o coloca no sistema. O sistema pesquisa o IP em um banco de dados especial e infere todos os tipos de informações.

>[!NOTE]
>
>Para garantir que os valores de campo inferidos permaneçam atuais, o banco de dados usado para pesquisas de endereço IP é atualizado periodicamente. As atualizações do banco de dados podem apresentar novos valores de campo inferidos que talvez você precise adicionar às definições de filtro da Smart List.
>
>As atualizações de banco de dados podem ocorrer durante uma [versão do produto Marketo Engage](/help/marketo/release-notes/release-schedule.md){target="_blank"}. Quando ocorrer uma atualização, as [notas de versão do Marketo Engage](/help/marketo/release-notes/current.md){target="_blank"} conterão uma explicação de quaisquer alterações nos valores de campo inferidos.

![](assets/inferred-filters-1.png)

![](assets/inferred-filters-2.png)

![](assets/inferred-filters-3.png)

![](assets/inferred-filters-4.png)

![](assets/inferred-filters-5.png)

![](assets/inferred-filters-6.png)

Ao usar qualquer um desses filtros em uma Smart List, os resultados produzirão pessoas com essas informações inferidas.

>[!TIP]
>
>Use esses filtros em um relatório de atividades da Web. Use os territórios dos representantes de vendas e inscreva-os em um relatório diário personalizado com os visitantes do site nas últimas 24 horas. Eles vão adorar!
>
>* Página da Web visitada - Últimas 24 horas
>* O Estado inferido é [selecionar seu território]

Esses visitantes anônimos são convertidos automaticamente em pessoas quando clicam em um link de email ou preenchem um formulário. No entanto, elas mantêm todas as informações inferidas.

>[!NOTE]
>
>Saiba mais sobre [atividade anônima e clientes potenciais](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/understanding-anonymous-activity-and-people.md){target="_blank"}.
