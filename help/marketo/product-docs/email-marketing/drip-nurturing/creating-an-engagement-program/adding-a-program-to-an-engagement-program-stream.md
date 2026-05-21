---
unique-page-id: 10098134
description: Saiba mais sobre programas aninhados em fluxos de engajamento e quando usá-los. Adicione programas para subgrupos, multitoque e etapas de fluxo extras.
title: Adicionar um programa a um fluxo de programa de engajamento
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
TQID: https://experienceleague.adobe.com/kI2v6drF78DnJhhEbgeVSi4TYbF5rExY2wgR0aAK-bI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 479
ht-degree: 4%

---

# Adicionar um programa a um fluxo de programa de engajamento {#adding-a-program-to-an-engagement-program-stream}

## Por que usar um programa aninhado em um fluxo de programa de engajamento? {#why-use-a-nested-program-in-an-engagement-program-stream}

É fácil adicionar um email a um fluxo em um programa de engajamento, e ele funciona bem. No entanto, se as necessidades da sua empresa forem mais complexas, pode fazer sentido colocar o email dentro de um programa. Por exemplo, talvez você queira:

* Enviar um email para um subgrupo de pessoas na transmissão
* Enviar emails *diferentes* para subgrupos dentro do fluxo
* Incluir páginas de aterrissagem, formulários ou outros ativos na criação
* Habilitar atribuição multitoque
* Adicionar etapas de fluxo extras, como emails de alerta

## O que acontece quando você usa um programa em um fluxo? {#what-happens-when-you-use-a-program-in-a-stream}

Ao usar um programa aninhado, a decisão de enviar um email para uma pessoa é baseada na associação ao programa e na ID do programa.

* Se você não for membro de um programa, receberá todos os emails que fazem parte do programa uma vez
* Se você for membro do programa, não receberá o email
* Se você não for mais membro, mas tiver recebido o email anteriormente por meio desse programa, não receberá o email

Quando você usa um programa em um fluxo, não importa se recebeu esse email específico antes. Desde que o email não tenha sido enviado antes de *nesse programa específico*, você poderá recebê-lo novamente.

Pode ser complicado misturar emails e programas em um programa de envolvimento. Talvez você queira usar um ou outro.

>[!TIP]
>
>Use um filtro **[!UICONTROL Membro do Programa de Envolvimento]** em sua lista inteligente.

## O que acontece com as pessoas que não atendem aos critérios da lista inteligente? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Caso alguém seja filtrado para fora da lista inteligente da campanha inteligente de um programa aninhado, ele não avançará para o próximo conteúdo durante o elenco atual. Eles avançarão para a próxima parte do conteúdo no fluxo para o elenco de *seguidores*.

## O que um programa aninhado contém? {#what-does-a-nested-program-contain}

Um programa aninhado bem projetado contém emails, relatórios e campanhas inteligentes. Faz sentido mantê-los juntos.

O email que você usa pode residir no programa, em um programa diferente ou até mesmo no [!UICONTROL Design Studio]. Onde ele mora dependerá de como você deseja usá-lo.

Alterações de relatório com o local do email. Assim, por exemplo, se o email estiver no [!UICONTROL Design Studio], no Relatório de Desempenho de Email, todas as métricas serão mostradas em uma linha - as diferentes conversões são combinadas. No entanto, no Relatório de desempenho do fluxo de engajamento, os diferentes envios são exibidos separadamente.

>[!CAUTION]
>
>Se quiser reenviar algo, é mais seguro criar um novo programa e uma campanha inteligente.

>[!MORELIKETHIS]
>
>* [Adicionar conteúdo a um fluxo](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Noções básicas sobre programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
