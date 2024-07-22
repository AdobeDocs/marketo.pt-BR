---
unique-page-id: 10098134
description: Adicionar um programa a um fluxo de programa de engajamento - Documentação do Marketo - Documentação do produto
title: Adicionar um programa a um fluxo de programa de engajamento
exl-id: 44c2ce45-439b-4b29-8130-8cc218e04bbf
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Adicionar um programa a um fluxo de programa de engajamento {#adding-a-program-to-an-engagement-program-stream}

## Por que usar um programa aninhado em um fluxo de programa de engajamento? {#why-use-a-nested-program-in-an-engagement-program-stream}

É fácil adicionar um email a um fluxo em um programa de engajamento e ele funciona bem. No entanto, se as necessidades da sua empresa forem mais complexas, pode fazer sentido colocar o email dentro de um programa. Por exemplo, talvez você queira:

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

Quando você usa um programa em um fluxo, não importa se você recebeu esse email específico antes. Desde que o email não tenha sido enviado antes de *nesse programa específico*, você poderá recebê-lo novamente.

Pode ser complicado misturar emails e programas em um programa de envolvimento. Talvez você queira usar um ou outro.

>[!TIP]
>
>Certifique-se de usar um filtro **Membro do Programa de Envolvimento** em sua lista inteligente.

## O que acontece com as pessoas que não atendem aos critérios da lista inteligente? {#what-happens-to-people-who-dont-meet-the-smart-list-criteria}

Caso alguém seja filtrado para fora da lista inteligente da campanha inteligente de um programa aninhado, ele não avançará para o próximo conteúdo durante o elenco atual. Eles avançarão para a próxima parte do conteúdo no fluxo para o elenco de *seguidores*.

## O que um programa aninhado contém? {#what-does-a-nested-program-contain}

Um programa aninhado bem projetado contém emails, relatórios e campanhas inteligentes. Faz sentido mantê-los juntos.

O email que você usa pode residir no programa, em um programa diferente ou até mesmo no Design Studio. Onde ele mora dependerá de como você deseja usá-lo.

Alterações de relatório com o local do email. Assim, por exemplo, se o email estiver no Design Studio, no Relatório de desempenho de email, todas as métricas serão mostradas em uma linha - as diferentes conversões são combinadas. No entanto, no Relatório de desempenho do fluxo de engajamento, os diferentes envios são exibidos separadamente.

>[!CAUTION]
>
>Se quiser reenviar algo, é mais seguro criar um novo programa e uma campanha inteligente.

>[!MORELIKETHIS]
>
>* [Adicionar conteúdo a um fluxo](/help/marketo/product-docs/email-marketing/drip-nurturing/creating-an-engagement-program/add-content-to-a-stream.md)
>* [Noções básicas sobre programas](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md)
