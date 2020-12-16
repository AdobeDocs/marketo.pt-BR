---
unique-page-id: 7515133
description: Sincronização SFDC - Mesclando um cliente potencial/contato/pessoa - Documentos do Marketing - Documentação do produto
title: Sincronização SFDC - Mesclando um cliente potencial/contato/pessoa
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Sincronização SFDC: Mesclando um cliente potencial/contato/pessoa {#sfdc-sync-merging-a-lead-contact-person}

Às vezes é melhor simplesmente lista as regras. Aqui vamos nós:

* Quando você mescla dois clientes potenciais no **Salesforce**, a sincronização normal informa ao Marketo e os clientes potenciais são mesclados automaticamente como pessoas no Marketo.
* A fusão de duas pessoas no **Marketo** na verdade chama o mesmo processo de mesclagem que as lideranças no Salesforce. Ainda funciona automaticamente.
* Mesclar um **cliente potencial (pessoa) em um contato** funciona da mesma maneira. Você acaba com um único contato de ambos os lados.
* Ao mesclar, a pontuação padrão é resumida.

>[!NOTE]
>
>**Exemplo**
>
>A mesclagem de 3 clientes potenciais (pessoas) com pontuações de 10 cada, resultará em um resultado de 1 cliente potencial (pessoa) com uma pontuação de 30.

* Valores de campo conflitantes são extraídos do &quot;registro vencedor&quot;. (Registro = o cliente potencial ou contato resultante)
* Se o &quot;recorde perdedor&quot; (aquele que está desaparecendo) tiver um valor e o recorde vencedor não tiver, manteremos o registro perdedor. Em outras palavras, &quot;Algum valor é melhor que nenhum valor.&quot;
* Todos os itens do registro de atividades são unidos.

>[!NOTE]
>
>**Mergulho profundo**
>
>Mergulhe fundo para obter mais informações sobre como [unir pessoas no Marketo](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).

