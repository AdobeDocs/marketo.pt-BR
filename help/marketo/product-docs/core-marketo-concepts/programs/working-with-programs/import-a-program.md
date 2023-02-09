---
unique-page-id: 1147108
description: Importar um programa - Documentos do Marketo - Documentação do produto
title: Importar um programa
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
source-git-commit: adff42d54d7953c9ec72e4d736ce0153502be960
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Importar um programa {#import-a-program}

Um programa pode ser importado de uma assinatura Marketo para outra. Por exemplo, você pode criar um programa em uma sandbox e depois importá-lo para a sua assinatura ativa. Além disso, você pode importar um programa pré-criado da Biblioteca de programas da Marketo.

## Importação de um programa {#importing-a-program}

1. Ir para **Atividades de marketing.**

   ![](assets/import-a-program-1.png)

1. Clique em **Novo** menu suspenso. Selecionar **Programa de importação**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >A Importação de Programa só está disponível para usuários que têm funções com a permissão Importar Programa ativada. Saiba mais sobre [gerenciamento de funções e permissões de usuários](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >Para conectar uma conta sandbox à sua assinatura ativa, entre em contato com [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Selecionar um Marketo **Assinatura** e um programa a importar. Clique em **Próximo**.

   ![](assets/import-a-program-3.png)

1. Especifique um **Pasta da campanha** para o programa importado. Clique em **Próximo.**

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Certifique-se de **Usar conflito padrão** for selecionada. As regras de conflito são necessárias ao importar programas em uma instância que tenha ativos com o mesmo nome.

1. Escolha os Detalhes de conflito desejados e clique em **Próximo**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Importando um programa que usa Etapas de fluxo personalizadas ou Regras de lista inteligente derivadas de um Serviço de etapa de fluxo para uma instância de destino em que há mais de um provedor de serviços compatível, o usuário importador será solicitado a atribuir etapas ou regras ao provedor de serviços correto na instância de destino.

1. Visualizar detalhes e **Importar** o programa.

   ![](assets/import-a-program-6.png)

Você receberá uma confirmação por email após a conclusão da importação.

>[!NOTE]
>
>Você precisará reprogramar campanhas em lote importadas e ativar campanhas de acionador. O sistema desativa automaticamente os cronogramas de campanha e aciona campanhas no programa importado.

## Impacto em ativos externos durante as importações do programa {#impact-on-external-assets-during-program-imports}

Os programas usam ativos externos, como modelos de email, modelos de landing page, imagens, formulários, tokens e tags de programa. Você pode configurar como os modelos de página de aterrissagem e as tags de programa são manipulados e o Marketo gerencia automaticamente o restante.

**Modelos de email/página de aterrissagem:** Os modelos de Email/Landing page são importados para o Design Studio. Você pode usar regras de conflito para configurar o comportamento quando existir um modelo com o mesmo nome. Usando a regra padrão, um número será anexado a um modelo se existir um com o mesmo nome. Por exemplo, se você já tiver um modelo chamado &quot;Modelo padrão&quot;, o novo será denominado &quot;Modelo padrão - 1&quot;.

**Páginas de aterrissagem/Forms:** Se um formulário ou uma landing page com o mesmo nome existir no Design Studio, eles ainda serão importados, mas com um número anexado ao seu nome (por exemplo: Página de aterrissagem - 1).

**Imagens:** As imagens usadas pela landing pages são importadas para o estúdio de design, a menos que exista uma com o mesmo nome.

**Tokens:** Tokens que vivem fora de um programa serão convertidos em tokens locais durante o processo de importação.

>[!CAUTION]
>
>O tipo de imagem que meus tokens não são suportados em importações de programa. Se um programa que tenha o tipo de imagem meus tokens for importado, **não** os tokens serão exibidos.

**Tags do programa:** Você pode usar regras de conflito para controlar como as tags de programa que não existem na conta de destino serão tratadas. O uso da regra padrão criará as tags de programa, ou você poderá optar por ignorar as tags.

>[!CAUTION]
>
>Ao importar um programa, emails/landing pages que contêm [conteúdo dinâmico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) serão ignoradas.
