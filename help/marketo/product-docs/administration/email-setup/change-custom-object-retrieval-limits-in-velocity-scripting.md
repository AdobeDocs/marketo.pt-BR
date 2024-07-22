---
description: "Alterar Limites de Recuperação de Objeto Personalizado em [!DNL Velocity Scripting] - Documentação do Marketo - Documentação do Produto"
title: "Alterar Limites de Recuperação de Objeto Personalizado em  [!DNL Velocity Scripting]"
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---

# Alterar Limites de Recuperação de Objeto Personalizado em [!DNL Velocity Scripting] {#change-custom-object-retrieval-limits-in-velocity-scripting}

Se você usa o [!DNL Velocity Script] para exibir dados de Objeto Personalizado em emails, esse recurso pode ser para você. Por padrão, você tem acesso a 10 objetos personalizados principais do Script do Velocity. Se precisar acessar mais, leia.

## O que é [!DNL Velocity] {#what-is-velocity}

[[!DNL Apache Velocity]](https://velocity.apache.org/) é uma linguagem criada em [!DNL Java] projetada para modelos e scripts de conteúdo de HTML. O Marketo permite que ele seja usado no contexto de Emails por meio do uso de [tokens de script](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Entre outras coisas, isso dá acesso aos dados armazenados em objetos personalizados.

Você pode fazer referência a objetos personalizados pai e filho que estão diretamente conectados ao cliente potencial ou ao contato, mas não a objetos personalizados de terceiro nível. Para cada objeto personalizado, os 10 registros atualizados mais recentemente por pessoa/contato estão disponíveis no tempo de execução e são ordenados da atualização mais recente (em 0) para a atualização mais antiga (em 9).

## Como alterar o limite {#how-to-change-the-limit}

1. Vá para a seção **[!UICONTROL Admin]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Clique em **[!UICONTROL Email]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Na tabela [!UICONTROL Limites de Recuperação de Objeto Personalizados], insira um novo [!UICONTROL Limite de Recuperação Pai] e clique em **[!UICONTROL Salvar Alterações]**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>O valor de [!UICONTROL Limite de Recuperação Pai] deve estar no intervalo de 10 a 100. O [!UICONTROL Limite de Recuperação de Filho] é definido automaticamente para você. Isso é feito dividindo 1000 pelo [!UICONTROL Limite de Recuperação Pai]. Por exemplo, se você definir o limite Pai como 50, o limite Filho se tornará 20 (1000 ÷ 50 = 20).

Legal! Agora você pode acessar mais objetos personalizados em [!DNL Velocity script].
