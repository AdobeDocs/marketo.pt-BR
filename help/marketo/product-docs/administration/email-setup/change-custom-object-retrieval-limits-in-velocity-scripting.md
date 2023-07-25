---
description: "Alterar Limites de Recuperação de Objeto Personalizado em [!DNL Velocity Scripting] - Documentação do Marketo - Documentação do produto"
title: "Alterar Limites de Recuperação de Objeto Personalizado em [!DNL Velocity Scripting]"
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---

# Alterar limites de recuperação de objetos personalizados em [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Se você usar [!DNL Velocity Script] para exibir os dados do objeto personalizado em emails, esse recurso pode ser para você. Por padrão, você tem acesso a 10 objetos personalizados principais do Script do Velocity. Se precisar acessar mais, leia.

## O que é o [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) é um idioma baseado em [!DNL Java] projetado para modelos e scripts de conteúdo de HTML. O Marketo permite que ele seja usado no contexto de emails por meio do uso de [tokens de script](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Entre outras coisas, isso dá acesso aos dados armazenados em objetos personalizados.

Você pode fazer referência a objetos personalizados pai e filho que estão diretamente conectados ao cliente potencial ou ao contato, mas não a objetos personalizados de terceiro nível. Para cada objeto personalizado, os 10 registros atualizados mais recentemente por pessoa/contato estão disponíveis no tempo de execução e são ordenados da atualização mais recente (em 0) para a atualização mais antiga (em 9).

## Como alterar o limite {#how-to-change-the-limit}

1. Vá para a **[!UICONTROL Admin]** seção.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Clique em **[!UICONTROL E-mail]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. No [!UICONTROL Limites de Recuperação de Objeto Personalizado] , insira um novo [!UICONTROL Limite de Recuperação Pai] e clique em **[!UICONTROL Salvar alterações]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>A variável [!UICONTROL Limite de Recuperação Pai] O valor deve estar no intervalo de 10 a 100. A variável [!UICONTROL Limite de Recuperação Filho] O é definido automaticamente para você. Isso é feito dividindo 1000 pelo [!UICONTROL Limite de Recuperação Pai]. Por exemplo, se você definir o limite Pai como 50, o limite Filho se tornará 20 (1000 ÷ 50 = 20).

Legal! Agora você pode acessar mais objetos personalizados no [!DNL Velocity script].
