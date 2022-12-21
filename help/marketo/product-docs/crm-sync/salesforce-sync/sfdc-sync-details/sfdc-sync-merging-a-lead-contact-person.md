---
unique-page-id: 7515133
description: Sincronização SFDC - Mesclar um cliente potencial/contato/pessoa - Documentos da Marketo - Documentação do produto
title: Sincronização SFDC - Mesclando um Lead/Contato/Pessoa
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# Sincronização SFDC: Mesclar um lead/contato/pessoa {#sfdc-sync-merging-a-lead-contact-person}

Às vezes é melhor listar as regras. Aqui vamos nós:

* Quando você mescla dois leads em **Salesforce**, a sincronização normal informa ao Marketo e os leads são mesclados automaticamente como pessoas no Marketo.
* Mesclar duas pessoas em **Marketo** Na verdade, chama o mesmo processo que mesclá-los como leads no Salesforce. Ele ainda funciona automaticamente.
* Mesclar um **cliente potencial (pessoa) em um contato** funciona da mesma maneira. Você acaba com um único contato de ambos os lados.
* Ao mesclar, a pontuação padrão é somada.

>[!NOTE]
>
>Mesclar 3 leads (pessoas) com pontuações de 10 cada um produzirá um resultado de 1 lead (pessoa) com uma pontuação de 30.

* Valores de campo conflitantes são retirados do &quot;registro vencedor&quot;. (Registro = o cliente potencial ou contato resultante)
* Se o &quot;registro perdedora&quot; (aquele que está desaparecendo) tivesse um valor e o registro vencedor não tiver, manteremos o registro perdedora. Em outras palavras, &quot;Algum valor é melhor do que nenhum valor&quot;.
* Todos os itens do log de atividades são mesclados.

>[!NOTE]
>
>Detalhe para obter mais informações sobre [mesclagem de pessoas no Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
