---
unique-page-id: 7515133
description: Sincronização SFDC - Mesclando um cliente potencial/contato/pessoa - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Mesclando um cliente potencial/contato/pessoa
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---


# Sincronização SFDC: Mesclando um cliente potencial/contato/pessoa {#sfdc-sync-merging-a-lead-contact-person}

Às vezes é melhor simplesmente lista as regras. Aqui vamos nós:

* Quando você mescla dois clientes potenciais em **Salesforce**, a sincronização normal informa ao Marketo e os clientes potenciais são mesclados automaticamente como pessoas no Marketo.
* A mesclagem de duas pessoas em **Marketo** chama o mesmo processo que mesclá-las como clientes potenciais no Salesforce. Ainda funciona automaticamente.
* Mesclar um **cliente potencial (pessoa) em um contato** funciona da mesma maneira. Você acaba com um único contato de ambos os lados.
* Ao mesclar, a pontuação padrão é resumida.

>[!NOTE]
>
>A mesclagem de 3 clientes potenciais (pessoas) com pontuações de 10 cada, resultará em um resultado de 1 cliente potencial (pessoa) com uma pontuação de 30.

* Valores de campo conflitantes são extraídos do &quot;registro vencedor&quot;. (Registro = o cliente potencial ou contato resultante)
* Se o &quot;recorde perdedor&quot; (aquele que está desaparecendo) tiver um valor e o recorde vencedor não tiver, manteremos o registro perdedor. Em outras palavras, &quot;Algum valor é melhor que nenhum valor.&quot;
* Todos os itens do registro de atividades são unidos.

>[!NOTE]
>
>Mergulhe fundo para obter mais informações sobre a união de [pessoas no Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
