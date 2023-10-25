---
unique-page-id: 10092977
description: Filtro de sincronização do Microsoft Dynamics - Qualificar - Documentação do Marketo - Documentação do produto
title: Filtro de sincronização do Microsoft Dynamics - Qualificar
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 6%

---

# Filtro de Sincronização do Microsoft Dynamics: Qualificar {#microsoft-dynamics-sync-filter-qualify}

Quando quiser converter um cliente potencial em um contato no Microsoft Dynamics, certifique-se de usar esse processo de qualificação padrão. Em seguida, sincronize-o com o Marketo Engage.

## O processo de conversão {#the-conversion-process}

Veja como os filtros funcionam durante o processo de conversão.

| Se o filtro de sincronização de leads for: | e o filtro de sincronização de contatos é: | Este é o resultado no Marketo |
|---|---|---|
| Falso | Falso | Nada é sincronizado no Marketo |
| True | True | O contato é sincronizado no Marketo |
| Falso | True | O novo registro de contato é criado no Marketo |
| True | Falso | O MS Dynamics atualiza as informações dos clientes potenciais no Marketo, mas o registro de contato não está sincronizado |

>[!CAUTION]
>
>Oferecemos suporte apenas ao processo de conversão Qualify pronto para uso.
