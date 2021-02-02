---
unique-page-id: 10092969
description: Filtro de Sincronização do Microsoft Dynamics - Mesclar - Documentos do Marketing - Documentação do Produto
title: Filtro de Sincronização do Microsoft Dynamics - Mesclar
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Filtro de Sincronização do Microsoft Dynamics: Mesclar {#microsoft-dynamics-sync-filter-merge}

A mesclagem de clientes em potencial no Microsoft Dynamics usa o tipo Duas Opções - Filtro de sincronização = Sim (TRUE) e o filtro de sincronização = Não (FALSE). Quando você mescla dois registros, o resultado varia, dependendo de qual registro é Verdadeiro e qual é Falso.

Os registros de cliente potencial se tornam verdadeiros ou falsos com base nas regras de fluxo de trabalho definidas pelo administrador para determinar o vencedor. O filtro de sincronização para o registro vencedor é o que determina se o registro do MS Dynamics sincroniza com o Marketo.

É quando um registro é verdadeiro e um é falso que fica complicado.

| Se o filtro de sincronização para o registro de perda for: | e o filtro de sincronização para o registro vencedor é: | Este é o resultado de Marketo |
|---|---|---|
| True | True | O registro vencedor continua sincronizando com o Marketo |
| Falso | Falso | O registro vencedor continua a **não** sincronizar com o Marketo |
| Falso | True | O registro vencedor será sincronizado com o Marketo |
| True | Falso | O registro vencedor não será sincronizado com o Marketo |
