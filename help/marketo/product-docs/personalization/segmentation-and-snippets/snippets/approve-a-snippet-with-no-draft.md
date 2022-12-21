---
unique-page-id: 10095644
description: Aprovar um trecho sem rascunho - Documentos da Marketo - Documentação do produto
title: Aprovar um trecho sem rascunho
exl-id: a06aa77a-68f1-41a4-b2bd-bf1882b81578
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Aprovar um trecho sem rascunho {#approve-a-snippet-with-no-draft}

## Aprovar o trecho {#approve-the-snippet}

Nenhum rascunho é acionado sempre que um trecho é aprovado. Isso inclui um trecho compartilhado ou referenciado por ativos em outros espaços de trabalho.

1. Ir para **Design Studio**.

   ![](assets/go-to-design-studio.png)

1. Selecione um snippet e no **Ações de trecho** , escolha **Aprovar**.

   ![](assets/approve-snippet.png)

1. Selecione uma opção na caixa de diálogo Aprovar trecho e clique em **Aprovar**:

   * **Atualizar tudo**: Essa opção não criará rascunhos dos ativos aprovados usando o trecho. Todos os ativos obtêm as atualizações e mantêm seus status anteriores. Um módulo de progresso aparece no lado superior direito do ecrã; pode ser fechado a qualquer momento. Para restaurá-lo, clique com o botão direito do mouse no nome do trecho e selecione Mostrar status de aprovação.
   * **Criar rascunhos**: Essa opção criará rascunhos dos ativos aprovados usando o trecho. Selecione esta opção se as alterações de trecho precisarem ser revisadas primeiro. Todos os rascunhos devem ser aprovados manualmente.

   ![](assets/snippet-dialog-box.png)

   >[!NOTE]
   >
   >Para um novo trecho que ainda não foi usado, essa tela Aprovar rascunho não é exibida. Ele é exibido quando o trecho é usado em um ou mais ativos.

>[!CAUTION]
>
>Esse recurso foi projetado para economizar tempo com o fluxo de trabalho de aprovação de trecho. No entanto, há algumas limitações a serem observadas. Consulte [este documento](https://nation.marketo.com/docs/DOC-4415) para obter detalhes. O documento também contém informações sobre tratamento de erros e solução de problemas.

>[!MORELIKETHIS]
>
>[Ativar Sem rascunho para trechos](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/enable-no-draft-for-snippets.md)
