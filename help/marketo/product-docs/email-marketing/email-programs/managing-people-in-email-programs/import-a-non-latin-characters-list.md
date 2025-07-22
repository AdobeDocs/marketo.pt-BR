---
unique-page-id: 5472678
description: Importar uma lista de caracteres não latinos - Documentação do Marketo - Documentação do produto
title: Importar uma lista de caracteres não latinos
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
feature: Email Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Importar uma lista de caracteres não latinos {#import-a-non-latin-characters-list}

Tentando importar um arquivo que não está em inglês? A lista parece perfeita quando você a abre com o Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Porém, ao importá-lo para o Marketo, você poderá observar que os caracteres que não estão em inglês não são selecionados corretamente.

![](assets/image2015-2-10-9-3a35-3a49.png)

Isso ocorre porque o arquivo não foi salvo corretamente para que o Marketo reconheça todos os caracteres não latinos. A boa notícia é que há algumas etapas simples que você pode seguir para corrigi-lo.

1. Selecione **[!UICONTROL Salvar como]...** no menu **[!UICONTROL Arquivo]** no Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Escolha **[!UICONTROL UTF-16 Texto Unicode (.txt)]** como a opção **[!UICONTROL Formato]**. Isso codificará o arquivo da maneira que o Marketo puder exibi-los.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >O Marketo também é compatível com UTF-8, Shift-JIS ou EUC-JP.

1. O Excel salvará o novo arquivo como um Arquivo de Texto com uma extensão .txt. Mas ela também converte todas as vírgulas no arquivo em guias. Precisamos mudá-la de volta.

   >[!TIP]
   >
   >Você pode abrir o Arquivo de Texto usando **[!DNL Notepad]** se estiver usando o Windows ou **[!DNL TextEdit]** se estiver usando um Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Selecione uma guia no documento e copie-a.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Selecione **[!UICONTROL Localizar e Substituir]...** no menu **[!UICONTROL Editar]**.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >A ação equivalente para usuários do Windows é: **[!UICONTROL Editar] > [!UICONTROL Substituir]...**

1. Cole a guia copiada na etapa 4 na primeira caixa (a ser substituída) e digite uma vírgula na segunda caixa (substituir por). E clique em **[!UICONTROL Todos]**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. E voila, todas as vírgulas estão de volta e estamos prontos para rolar.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importe o novo arquivo para o Marketo e as informações deverão ser exibidas corretamente desta vez.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Qualquer campo de data/hora que for importado será tratado como Hora central. Se você tiver campos de data/hora em um fuso horário diferente, poderá usar uma fórmula do Excel para transformá-la na Hora Central (América/Chicago).

Sabemos que isso é estranho, mas funciona. Feliz Importação!
