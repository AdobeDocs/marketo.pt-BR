---
unique-page-id: 10092969
description: Filtro de Sincronização do Microsoft Dynamics - Mesclar - Documentos do Marketo - Documentação do produto
title: Filtro de Sincronização do Microsoft Dynamics - Mesclar
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Filtro de Sincronização do Microsoft Dynamics: Mesclar {#microsoft-dynamics-sync-filter-merge}

A mesclagem de leads no Microsoft Dynamics usa o tipo Duas Opções - Filtro de sincronização = Sim (TRUE) e Filtro de sincronização = Não (FALSE). Quando você mescla dois registros, o resultado varia, dependendo de qual registro é Verdadeiro e qual é Falso.

Os registros de lead se tornam verdadeiros ou falsos com base nas regras de fluxo de trabalho definidas pelo administrador para determinar o vencedor. O filtro de sincronização para o registro vencedor é o que determina, em última análise, se o registro do MS Dynamics sincroniza com o Marketo.

É quando um registro é verdadeiro e um é falso que fica complicado.

| Se o filtro de sincronização para o registro perdedora for: | e o filtro de sincronização para o registro vencedor é: | Esse é o resultado no Marketo |
|---|---|---|
| Verdadeiro | Verdadeiro | O registro vencedor continua sincronizando com o Marketo |
| Falso | Falso | O registro vencedor continua a **não** sincronizar com o Marketo |
| Falso | Verdadeiro | O registro vencedor será sincronizado com o Marketo |
| Verdadeiro | Falso | O registro vencedor não será sincronizado com o Marketo |
