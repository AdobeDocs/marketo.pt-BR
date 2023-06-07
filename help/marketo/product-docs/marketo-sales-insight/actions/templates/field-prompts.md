---
description: Avisos de campo - Documentação do Marketo - Documentação do produto
title: Prompts de campo
source-git-commit: b4773137bf21eccc58a6d975d50748e8ff2a57db
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Prompts de campo {#field-prompts}

Os prompts de campo permitem que você adicione uma string de texto aos emails que precisam ser removidos ou substituídos antes que o email possa ser enviado. Essa é uma ótima maneira de lembrar os usuários de adicionar mais personalização.

Para adicionar um prompt de campo, digite o texto desejado. Coloque um ponto de exclamação como prefixo e coloque-o entre chaves (veja abaixo).

**Exemplos:**

`{{! Introduce yourself}}`

`{{! Insert name of Account Executive}}`

`{{! Add sentence that references their industry and role}}`

<p>Os usuários precisarão substituir esse texto por sua própria personalização antes que o email possa ser enviado.

>[!NOTE]
>
>Ao usar prompts com campanhas de vendas, é melhor usá-los com etapas de email manuais. Essas etapas atribuirão ao usuário uma tarefa de lembrete para enviar o email, dando a ele a oportunidade de substituir os prompts por texto personalizado. As etapas automáticas de email das Campanhas de vendas tentarão enviar automaticamente, sem permitir que o usuário substitua os prompts. Os prompts que não forem substituídos farão com que os emails não sejam enviados.
