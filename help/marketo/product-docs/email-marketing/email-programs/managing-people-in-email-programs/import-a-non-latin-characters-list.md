---
unique-page-id: 5472678
description: Importar uma Lista de caracteres não latinos - Documentos do Marketing - Documentação do produto
title: Importar uma Lista de caracteres não latinos
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Importar uma Lista de caracteres não latinos {#import-a-non-latin-characters-list}

Tentando importar um arquivo que não está em inglês? A lista parece perfeita quando você a abre com o Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Mas ao importá-lo para o Marketo, você pode ver que os caracteres que não são do inglês não são coletados corretamente.

![](assets/image2015-2-10-9-3a35-3a49.png)

Isso ocorre porque o arquivo não é salvo corretamente para que o Marketo reconheça todos os caracteres não latinos. A boa notícia é que há alguns passos simples a serem seguidos para consertá-lo.

1. Selecione **Salvar como...** do menu **Arquivo** no Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Escolha **UTF-16 Texto Unicode (.txt)** como a opção **Format**. Isso codificará o arquivo da maneira que o Marketo pode exibi-los.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >O Marketo também é compatível com UTF-8, Shift-JIS ou EUC-JP.

1. O Excel salvará o novo arquivo como um Arquivo de texto com uma extensão .txt. Mas também converte todas as vírgulas do arquivo em guias. Precisamos mudar de volta.

   >[!TIP]
   >
   >Você pode abrir o Arquivo de texto usando **Bloco de notas** se estiver usando o Windows ou **TextEdit** se estiver usando um Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Selecione uma guia no documento e copie-a.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Selecione **Localizar e Substituir...** no menu **Editar**.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >A ação equivalente para usuários do Windows é: **Editar > Substituir...**

1. Cole a guia copiada na etapa 4 na primeira caixa (a ser substituída) e digite uma vírgula na segunda caixa (substituir por). E clique em **All**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. E voila, todas as vírgulas voltaram e estamos prontos para rodar.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importe o novo arquivo para o Marketo e as informações devem ser exibidas corretamente desta vez.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Todos os campos de data/hora que estão sendo importados são tratados como Hora Central. Se você tiver campos de data/hora em um fuso horário diferente, poderá usar uma fórmula do Excel para transformá-la em Hora Central (América/Chicago).

Sabemos que isso é estranho, mas funciona. Feliz importação!