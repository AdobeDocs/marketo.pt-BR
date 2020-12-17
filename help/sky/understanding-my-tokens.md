---
title: entender-meus-tokens
description: Como entender meus tokens
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---


# Como entender meus tokens

<br> 

Meus tokens são variáveis personalizadas que você pode criar e usar em suas pastas de programas ou campanhas. Eles se parecem com isto: `{{_my.Name of Token_}}`

## Exemplos

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

Para acessar e criar Meus tokens, selecione sua pasta programa ou campanha e vá para a guia [!UICONTROL Meus Tokens]. Arraste e solte qualquer token na tela [!UICONTROL Tokens locais].

![Imagem Um](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>Os nomes dos meus tokens não podem ser alterados depois de terem sido salvos, então escolha cuidadosamente.

>[!NOTE]
>
>Meus tokens não serão resolvidos ao enviar um email do Sales Insight no Microsoft Dynamics ou no Salesforce; somente os tokens padrão serão preenchidos (cliente potencial, Empresa etc.). No entanto, os valores padrão para tokens funcionarão.

>[!NOTE]
>
>Os tokens de link não funcionam em emails somente de texto.

## Aninhamento de tokens

Quando você cria um novo token, ele pode ser referenciado por outros objetos na árvore. É possível substituir variáveis globais em níveis mais baixos na árvore. Há uma estrutura de nomenclatura para a qual o token foi criado para facilitar o gerenciamento.

* **Token local:** o token foi criado diretamente nesse programa ou pasta.
* **[Token substituído:](/help/sky/override-an-inherited-my-token.md)** o token foi herdado, mas foi feita uma exceção neste programa ou pasta.
* **Token herdado:** o token foi criado na árvore em algum lugar em um programa ou pasta de nível superior.

Você pode encontrar esses três tipos na guia **[!UICONTROL Meus tokens]** na pasta programa ou campanha.

![Imagem dois](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

Mover programas e pastas também afeta os tokens. Sempre verifique se as referências não estão quebradas durante a mudança.

>[!NOTE]
>
>Se o e-mail enviado de um programa de envolvimento for um e-mail filho de um programa padrão (ou seja, não local para o programa de envolvimento), todos os Meus tokens usados no e-mail serão resolvidos do programa padrão no qual o e-mail filho reside.

## Uso de token

Selecione qualquer token e clique no ícone de uso no canto superior direito para ver uma lista de ativos que contêm esse token.

![Imagem Três](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![Imagem quatro](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**Mergulho profundo**

Saiba mais sobre cada um dos My Tokens:

* [CAMPANHA CRM](/help/sky/my-token-crm-campaign.md)
* [Data](/help/sky/my-token-date.md)
* [Arquivo de calendário](/help/sky/my-token-calendar-file.md)
* [Imagem](/help/sky/my-token-image.md)
* [Link](/help/sky/my-token-link.md)
* [Número](/help/sky/my-token-number.md)
* [Rich Text](/help/sky/my-token-rich-text.md)
* [Pontuação](/help/sky/my-token-score.md)
* [Script de email](/help/sky/my-token-email-script.md)
* [Texto](/help/sky/my-token-text.md)
