---
unique-page-id: 3571844
description: Microsoft Dynamics Sync — Sincronização De Oportunidades — Documentação Do Marketo — Documentação Do Produto
title: Microsoft Dynamics Sync - Sincronização De Oportunidades
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 9a130e0b2ec84b638adf37188b65b565b090fe1b
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Sincronização De Oportunidades {#microsoft-dynamics-sync-opportunity-sync}

A sincronização do Marketo Engage para o Dynamics é superpoderosa. Aqui estão todos os detalhes da sincronização de oportunidades.

## Como os detalhes da oportunidade são mantidos em sincronia entre os dois sistemas? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

A sincronização de oportunidades é uma via - Dinâmica para o Marketo. Se você fizer alterações em uma oportunidade no Dynamics, sua atualização será refletida no Marketo.

## Posso criar uma oportunidade no Dynamics usando o Marketo? {#can-i-create-an-opportunity-in-dynamics-using-marketo}

Não, você deve criar a oportunidade no Dynamics e ela será sincronizada automaticamente com o Marketo.

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante a configuração.

## Como uma Conta/Contato é associada a uma Oportunidade? {#how-is-an-account-contact-associated-with-an-opportunity}

O Contato/Conta pode ser associado à Oportunidade de duas maneiras:

* Ao criar uma oportunidade, o Contato (campo de pesquisa no formulário a ser contatado) e/ou a Conta (campo de pesquisa no formulário a ser contado) podem ser definidos. Em ambos os casos, esses valores são armazenados no campo Cliente em potencial (customerid) no Dynamics. Este campo não aparece no formulário de oportunidade, mas pode ser adicionado das configurações. Este campo pode conter apenas 1 valor, seja contato ou conta. A Marketo faz o seguinte:

   * Se o valor de contato estiver definido e a conta ficar vazia, o Marketo cria uma `opportunitycontactrole` e define a conta na oportunidade para a conta do contato. Se o contato não tiver uma conta, esse campo ficará vazio.
   * Se o valor da conta for definido e o contato for deixado em branco, a Marketo somente definirá a conta na oportunidade para essa conta.
   * Se ambos os valores forem definidos, o Dynamics escolherá a conta como o valor de customerid, para que o comportamento seja o mesmo acima.


* Por meio das partes interessadas: o Dynamics usa conexões para conectar a oportunidade ao contato por meio das partes interessadas da página de criação da oportunidade. Para isso, criaremos um `opportunitycontactrole` registro para cada nova parte interessada.
