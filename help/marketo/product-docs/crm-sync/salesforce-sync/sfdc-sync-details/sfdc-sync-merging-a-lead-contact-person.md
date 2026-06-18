---
unique-page-id: 7515133
description: Entenda como a mesclagem de clientes potenciais, contatos e pessoas no Salesforce e no Marketo funciona. Saiba mais sobre regras de mesclagem para pontuações, valores de campo e logs de atividades.
title: Sincronização da SFDC - Intercalando um cliente em potencial/contato/pessoa
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/alPa6YMG0tgo08ruZAZlWhujV54iVcUMAAejXJbEQFw
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: 18ccc13ddd9cfb998015bb581373a7ca7c064d59
workflow-type: tm+mt
source-wordcount: 268
ht-degree: 2%

---

# Sincronização do SFDC: mesclar um lead, contato ou pessoa {#sfdc-sync-merging-a-lead-contact-person}

Às vezes, é melhor apenas listar as regras. Aqui vamos nós:

* Quando você mescla dois clientes em potencial no **[!DNL Salesforce]**, a sincronização normal informa ao Marketo e os clientes em potencial são mesclados automaticamente como pessoas no Marketo.
* Mesclar duas pessoas no **Marketo** invoca o mesmo processo que mesclá-las como clientes em potencial no [!DNL Salesforce]. Ele ainda funciona automaticamente.
* Mesclar um **lead (pessoa) em um contato** funciona da mesma maneira. Você acaba com um único contato de ambos os lados.
* Ao mesclar, a pontuação padrão é somada.

>[!NOTE]
>
>Mesclar 3 leads (pessoas) com pontuações de 10 cada um produzirá um resultado de 1 lead (pessoa) com uma pontuação de 30.

* Valores de campo conflitantes são retirados do &quot;registro vencedor&quot;. (Registro = o lead ou contato resultante)
* Se o &quot;registro perdedor&quot; (aquele que está desaparecendo) tiver um valor e o registro vencedor não tiver nenhum (ou for nulo), manteremos o registro perdedor. Em outras palavras, &quot;algum valor é melhor do que nenhum valor&quot;.
* Todos os itens do log de atividades são mesclados.

>[!NOTE]
>
>O comportamento dos campos booleanos em uma mesclagem de API mudou na versão de março de 2026. Agora, um valor Falso é tratado corretamente como tendo um valor para esse campo. Somente um valor nulo é tratado como &quot;vazio&quot; ao avaliar campos conflitantes. Consulte [esta publicação da comunidade](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/api-merge-functionality-for-boolean-fields-251219?profile.language=pt){target="_blank"} para obter mais detalhes.

>[!MORELIKETHIS]
>
>Aprofundamento para obter mais informações sobre [mesclando pessoas no Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
