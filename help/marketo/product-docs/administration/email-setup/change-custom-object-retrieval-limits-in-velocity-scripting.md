---
description: Alterar limites de recuperação de objeto personalizado no script do Velocity - Documentos do Marketo - Documentação do produto
title: Alterar limites de recuperação de objeto personalizado no script do Velocity
exl-id: ef45205e-421d-4d1d-8c9d-7d627326a90c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Alterar limites de recuperação de objeto personalizado no script do Velocity {#change-custom-object-retrieval-limits-in-velocity-scripting}

Se você usa o script do Velocity para exibir dados de Objeto personalizado em emails, esse recurso pode ser para você. Por padrão, você tem acesso a 10 objetos personalizados principais do Script do Velocity. Se precisar acessar mais, leia.

## O que é o Velocity {#what-is-velocity}

[O Apache Velocity](https://velocity.apache.org/) é uma linguagem incorporada ao Java, projetada para modelar e criar scripts de conteúdo HTML. O Marketo permite que ele seja usado no contexto de Emails por meio do uso de [tokens de script](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md). Dentre outras coisas, isso dá acesso aos dados armazenados em objetos personalizados.

Você pode fazer referência a objetos personalizados pai e filho que estejam diretamente conectados ao Lead ou Contato, mas não a objetos personalizados de terceiros. Para cada objeto personalizado, os 10 registros atualizados mais recentemente por pessoa/contato estão disponíveis em tempo de execução e são ordenados da atualização mais recente (em 0) para a atualização mais antiga (em 9).

## Como alterar o limite {#how-to-change-the-limit}

1. Vá para a seção **Admin**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-1.png)

1. Clique em **Email**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-2.png)

1. Na tabela Limites de Recuperação de Objeto Personalizado, insira um novo Limite de Recuperação de Pai e clique em **Salvar Alterações**.

   ![](assets/change-custom-object-retrieval-limits-in-velocity-scripting-3.png)

>[!NOTE]
>
>O valor do Limite de Recuperação Pai deve estar no intervalo de 10 - 100. O Limite de Recuperação de Filho é definido automaticamente para você. Isso é feito dividindo 1000 pelo Limite de Recuperação do Pai. Por exemplo, se você definir o limite Pai como 50, o limite Filho se tornará 20 (1000 ÷ 50 = 20).

Doce! Agora é possível acessar mais objetos personalizados do script do Velocity.
