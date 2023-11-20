---
unique-page-id: 7515133
description: Sincronização de SFDC - Mesclando um lead/contato/pessoa - Documentação da Marketo - Documentação do produto
title: Sincronização do SFDC - Intercalando um cliente em potencial/contato/pessoa
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Sincronização do SFDC: Intercalando um lead/contato/pessoa {#sfdc-sync-merging-a-lead-contact-person}

Às vezes é melhor apenas listar as regras. Aqui vamos nós:

* Ao mesclar dois leads em **Salesforce**, a sincronização normal informa ao Marketo Engage e os leads são mesclados automaticamente como pessoas no Marketo.
* Mesclar duas pessoas em **Marketo** na verdade, invoca o mesmo processo que mesclá-los como leads no Salesforce. Ele ainda funciona automaticamente.
* Mesclar um **lead (pessoa) em um contato** funciona da mesma maneira. Você acaba com um único contato de ambos os lados.
* Ao mesclar, a pontuação padrão é somada.

>[!NOTE]
>
>Mesclar 3 leads (pessoas) com pontuações de 10 cada um produzirá um resultado de 1 lead (pessoa) com uma pontuação de 30.

* Valores de campo conflitantes são retirados do &quot;registro vencedor&quot;. (Registro = o lead ou contato resultante)
* Se o &quot;registro perdedor&quot; (aquele que está desaparecendo) tivesse um valor e o registro vencedor não tivesse nenhum, nós manteremos o registro perdedor. Em outras palavras, &quot;algum valor é melhor do que nenhum valor&quot;.
* Todos os itens do log de atividades são mesclados.

>[!NOTE]
>
>Detalhes para obter mais informações sobre [mesclar pessoas no Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}.
