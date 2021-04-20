---
title: noções básicas sobre os meus tokens
description: Noções básicas sobre meus tokens
exl-id: d56748e2-d742-45dd-96a8-dd80e30d9d8b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 5%

---

# Noções básicas sobre meus tokens

<br> 

Meus tokens são variáveis personalizadas que podem ser criadas e usadas em programas ou pastas de campanha. Eles se parecem com isto: `{{_my.Name of Token_}}`

## Exemplos

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

Para acessar e criar Meus tokens, selecione o programa ou a pasta da campanha e vá para a guia [!UICONTROL Meus tokens]. Arraste e solte qualquer token em sua tela [!UICONTROL Tokens locais].

![Imagem Um](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>Os nomes de Meus Tokens não podem ser alterados depois de terem sido salvos, portanto, escolha cuidadosamente.

>[!NOTE]
>
>Meus tokens não serão resolvidos ao enviar um email do Sales Insight no Microsoft Dynamics ou no Salesforce; somente os tokens padrão serão preenchidos (lead, empresa etc.). No entanto, os valores padrão para tokens funcionarão.

>[!NOTE]
>
>Os tokens de link não funcionarão em emails somente texto.

## Aninhamento de tokens

Quando você faz um novo token, ele pode ser referenciado por outros objetos na árvore. É possível substituir variáveis globais em níveis inferiores na árvore. Existe uma estrutura de nomenclatura para a qual o token foi criado para facilitar o gerenciamento.

* **Token local:** o token foi criado diretamente nesse programa ou pasta.
* **[Token substituído:](/help/sky/override-an-inherited-my-token.md)** o token foi herdado, mas foi feita uma exceção neste programa ou pasta.
* **Token herdado:** o token foi criado acima da árvore em algum lugar em um programa ou pasta de nível superior.

Você pode encontrar esses três tipos na guia **[!UICONTROL Meus tokens]** em seu programa ou pasta da campanha.

![Imagem dois](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

Mover programas e pastas afeta tokens também. Sempre verifique se as referências não estão quebradas durante a movimentação.

>[!NOTE]
>
>Se o e-mail enviado de um programa de envolvimento for um e-mail filho de um programa padrão (ou seja, não local para seu programa de envolvimento), todos os Meus tokens usados no e-mail serão resolvidos do programa padrão em que o e-mail filho reside.

## Utilização do token

Selecione qualquer token e clique no ícone de uso no canto superior direito para ver uma lista de ativos que contêm esse token.

![Imagem Três](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![Imagem quatro](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**Aprofundamento**

Saiba mais sobre cada um dos Meus tokens:

* [Campanha do CRM](/help/sky/my-token-crm-campaign.md)
* [Data](/help/sky/my-token-date.md)
* [Arquivo de calendário](/help/sky/my-token-calendar-file.md)
* [Imagem](/help/sky/my-token-image.md)
* [Link](/help/sky/my-token-link.md)
* [Número](/help/sky/my-token-number.md)
* [Texto formatado](/help/sky/my-token-rich-text.md)
* [Pontuação](/help/sky/my-token-score.md)
* [Script de e-mail](/help/sky/my-token-email-script.md)
* [Texto](/help/sky/my-token-text.md)
