---
unique-page-id: 10092969
description: Filtro de sincronização do Microsoft Dynamics - Mesclar - Documentação do Marketo - Documentação do produto
title: Filtro de sincronização do Microsoft Dynamics - Mesclar
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Filtro de Sincronização do Microsoft Dynamics: Mesclar {#microsoft-dynamics-sync-filter-merge}

A mesclagem de clientes em potencial no Microsoft Dynamics usa o tipo Duas opções - Filtro de sincronização = Sim (TRUE) e Filtro de sincronização = Não (FALSE). Quando você mescla dois registros, o resultado varia, dependendo de qual registro é True e qual é False.

Os registros de lead tornam-se verdadeiros ou falsos com base nas regras de fluxo de trabalho definidas pelo administrador para determinar o vencedor. O filtro de sincronização do registro vencedor é o que determina se o registro do MS Dynamics é sincronizado com o Marketo.

É quando um registro é verdadeiro e outro é falso que ele fica complicado.

| Se o filtro de sincronização do registro perdido for: | e o filtro de sincronização do registro vencedor é: | Este é o resultado no Marketo |
|---|---|---|
| True | True | O registro vencedor continua a sincronização com o Marketo |
| Falso | Falso | O recorde de vitórias continua a _não_ sincronizar com o Marketo |
| Falso | True | O registro vencedor será sincronizado com o Marketo |
| True | Falso | O registro vencedor não será sincronizado com o Marketo |
