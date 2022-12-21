---
unique-page-id: 10092977
description: Filtro de sincronização do Microsoft Dynamics - Qualificar - Documentos do Marketo - Documentação do produto
title: Filtro de Sincronização do Microsoft Dynamics - Qualificar
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Filtro de sincronização do Microsoft Dynamics: Qualificar {#microsoft-dynamics-sync-filter-qualify}

Quando quiser converter um lead para um contato no Microsoft Dynamics, certifique-se de usar esse processo padrão de qualificação. Em seguida, sincronize-a com o Marketo.

## O processo de conversão {#the-conversion-process}

Veja como os filtros funcionam durante o processo de conversão.

| Se o filtro de sincronização de leads for: | e o filtro de sincronização de contatos é: | Esse é o resultado no Marketo |
|---|---|---|
| False | False | Nada é sincronizado no Marketo |
| True | True | O contato é sincronizado no Marketo |
| False | True | Novo registro de contato é criado no Marketo |
| True | False | O MS Dynamics atualiza informações privilegiadas no Marketo, mas o registro de contato não é sincronizado |

>[!CAUTION]
>
>Só oferecemos suporte ao processo de conversão qualificado pronto para uso.
