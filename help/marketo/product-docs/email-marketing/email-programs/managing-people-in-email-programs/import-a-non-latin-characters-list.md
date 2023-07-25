---
unique-page-id: 5472678
description: Importar uma lista de caracteres não latinos - Documentação do Marketo - Documentação do produto
title: Importar uma lista de caracteres não latinos
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Importar uma lista de caracteres não latinos {#import-a-non-latin-characters-list}

Tentando importar um arquivo que não está em inglês? A lista parece perfeita quando você a abre com o Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Porém, ao importá-lo para o Marketo, você poderá observar que os caracteres que não estão em inglês não são selecionados corretamente.

![](assets/image2015-2-10-9-3a35-3a49.png)

Isso ocorre porque o arquivo não foi salvo corretamente para que o Marketo reconheça todos os caracteres não latinos. A boa notícia é que há algumas etapas simples que você pode seguir para corrigi-lo.

1. Selecionar **Salvar como...** do **Arquivo** no Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Escolher **Texto Unicode UTF-16 (.txt)** como o **Formato** opção. Isso codificará o arquivo da maneira que o Marketo puder exibi-los.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >O Marketo também é compatível com UTF-8, Shift-JIS ou EUC-JP.

1. O Excel salvará o novo arquivo como um Arquivo de Texto com uma extensão .txt. Mas ela também converte todas as vírgulas no arquivo em guias. Precisamos mudá-la de volta.

   >[!TIP]
   >
   >É possível abrir o arquivo de texto usando **Bloco de notas** se você estiver usando o Windows ou **EdiçãoDeTexto** se você estiver usando uma Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Selecione uma guia no documento e copie-a.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Selecionar **Localizar e substituir...** do **Editar** menu.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >A ação equivalente para usuários do Windows é: **Editar > Substituir...**

1. Cole a guia copiada na etapa 4 na primeira caixa (a ser substituída) e digite uma vírgula na segunda caixa (substituir por). E clique em **Todos**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. E voila, todas as vírgulas estão de volta e estamos prontos para rolar.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importe o novo arquivo para o Marketo e as informações deverão ser exibidas corretamente desta vez.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Qualquer campo de data/hora que for importado será tratado como Hora central. Se você tiver campos de data/hora em um fuso horário diferente, poderá usar uma fórmula do Excel para transformá-la na Hora Central (América/Chicago).

Sabemos que isso é estranho, mas funciona. Feliz Importação!
