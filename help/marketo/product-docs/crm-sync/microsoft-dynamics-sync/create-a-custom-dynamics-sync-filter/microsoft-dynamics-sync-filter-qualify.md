---
unique-page-id: 10092977
description: Filtro de Sincronização do Microsoft Dynamics - Qualificar - Documentos do Marketing - Documentação do Produto
title: Filtro de Sincronização do Microsoft Dynamics - Qualificado
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Filtro de Sincronização do Microsoft Dynamics: Qualificar {#microsoft-dynamics-sync-filter-qualify}

Quando quiser converter um cliente potencial para um contato no Microsoft Dynamics, certifique-se de usar este processo padrão de Qualificação. Em seguida, sincronize-o com o Marketo.

## O processo de conversão {#the-conversion-process}

Veja como os filtros funcionam durante o processo de conversão.

| Se o filtro de sincronização de cliente potencial for: | e o filtro de sincronização de contato é: | Este é o resultado de Marketo |
|---|---|---|
| Falso | Falso | Nada é sincronizado no Marketo |
| True | True | O contato é sincronizado no Marketo |
| Falso | True | Novo registro de contato é criado no Marketo |
| True | Falso | O MS Dynamics atualiza informações de cliente potencial no Marketo, mas o registro de contato não é sincronizado |

>[!CAUTION]
>
>Nós só oferecemos suporte ao processo de conversão qualificado e pronto.
