---
unique-page-id: 1147108
description: Importar um programa - Documentação do Marketo - Documentação do produto
title: Importar um programa
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
feature: Programs
source-git-commit: 0adb780ea1622d12b8daafc502fd6a9151757ad3
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Importar um programa {#import-a-program}

Um programa pode ser importado de uma assinatura de Marketo Engage para outra. Por exemplo, você pode criar um programa em uma sandbox e importá-lo para a sua assinatura em tempo real. Além disso, é possível importar um programa pré-criado da [Biblioteca de programas da Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview.md){target="_blank"}.

>[!CAUTION]
>
>Programas que possuem Smart Lists contendo um acionador &quot;Objeto personalizado atualizado&quot; farão com que a importação falhe. Remova esse acionador de todas as Smart Lists antes de seguir as etapas descritas abaixo.

## Importando um programa {#importing-a-program}

1. Ir para **[!UICONTROL Atividades de marketing]**.

   ![](assets/import-a-program-1.png)

1. Clique em **[!UICONTROL Novo]** e selecione **[!UICONTROL Importar programa]**.

   ![](assets/import-a-program-2.png)

   >[!NOTE]
   >
   >* A Importação de programa só está disponível para usuários com as funções com a permissão Importar programa habilitada. Saiba mais sobre [gerenciamento de funções e permissões de usuário](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.
   >
   >* Para conectar uma conta de sandbox à sua assinatura live, entre em contato com [Suporte ao Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

1. Selecionar um Marketo **[!UICONTROL Inscrição]** e um programa para importar. Clique em **[!UICONTROL Próxima]**.

   ![](assets/import-a-program-3.png)

1. Especificar um **[!UICONTROL Pasta do Campaign]** para o programa importado. Clique em **[!UICONTROL Próxima]**.

   ![](assets/import-a-program-4.png)

   >[!NOTE]
   >
   >Verifique se **[!UICONTROL Usar conflito padrão]** regras está selecionada. As regras de conflito são necessárias ao importar programas para uma instância que tenha ativos com o mesmo nome.

1. Escolha os Detalhes do Conflito desejados e clique em **[!UICONTROL Próxima]**.

   ![](assets/import-a-program-5.png)

   >[!NOTE]
   >
   >Ao importar um programa que use Etapas de fluxo personalizadas ou regras de Smart List derivadas de um Serviço de Etapa de Fluxo para uma instância de destino em que haja mais de um provedor de serviços compatível, o usuário importador será solicitado a atribuir etapas ou regras ao provedor de serviços correto na instância de destino.

1. Visualizar detalhes e **[!UICONTROL Importar]** programa.

   ![](assets/import-a-program-6.png)

Você receberá uma confirmação por email após a conclusão da importação.

>[!NOTE]
>
>Você precisará reagendar campanhas em lote importadas e ativar campanhas de acionador. O sistema desativa automaticamente os cronogramas da campanha e aciona campanhas no programa importado.

## Impacto nos ativos externos durante as importações de programa {#impact-on-external-assets-during-program-imports}

Os programas usam ativos externos, como modelos de email, modelos de landing page, imagens, formulários, tokens e tags de programa. Você pode configurar como os modelos de página de aterrissagem e as tags de programa são tratados, e o Marketo gerencia o restante automaticamente.

**Modelos de email/página de aterrissagem:** Os modelos de email/landing page são importados para o Design Studio. Você pode usar as regras de conflito para configurar o comportamento quando existir um modelo com o mesmo nome. Usando a regra padrão, um número será anexado a um modelo se existir um com o mesmo nome. Por exemplo, se você já tiver um modelo chamado &quot;Modelo padrão&quot;, o novo será chamado de &quot;Modelo padrão - 1&quot;.

**Landing Pages/Forms:** Se existir um formulário ou uma Landing page com o mesmo nome no Design Studio, eles ainda serão importados, mas com um número anexado ao nome (por exemplo: Landing Page - 1).

**Imagens:** Imagens usadas por Landing Pages são importadas para o design studio, a menos que exista uma com o mesmo nome.

**Tokens:** Os tokens localizados fora de um programa serão convertidos em tokens locais durante o processo de importação.

>[!CAUTION]
>
>Meus tokens de tipo de imagem não são compatíveis com importações de programas. Se um programa com tipo de imagem de meus tokens for importado, _não_ tokens aparecerão.

**Tags do programa:** Você pode usar regras de conflito para controlar como as tags de programa que não existem na conta de destino serão tratadas. Usar a regra padrão criará as tags do programa ou você poderá optar por ignorá-las.

>[!CAUTION]
>
>Ao importar um programa, os emails/Landing Pages que contêm [conteúdo dinâmico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md){target="_blank"} serão ignorados.
