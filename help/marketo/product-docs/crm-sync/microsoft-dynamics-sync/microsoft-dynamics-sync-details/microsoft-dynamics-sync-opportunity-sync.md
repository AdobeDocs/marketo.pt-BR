---
unique-page-id: 3571844
description: Microsoft Dynamics Sync - Sincronização de oportunidade - Documentação do Marketo - Documentação do produto
title: Microsoft Dynamics Sync - Sincronização de oportunidade
exl-id: dcb72f28-c980-4183-8473-a1e5ad0c8d3c
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Sincronização de [!DNL Microsoft Dynamics]: Sincronização de Oportunidade {#microsoft-dynamics-sync-opportunity-sync}

A sincronização do Marketo com o [!DNL Dynamics] é super poderosa. Aqui estão todos os detalhes da sincronização de oportunidade:

## Como os detalhes da oportunidade são mantidos em sincronia entre os dois sistemas? {#how-are-opportunity-details-kept-in-sync-between-the-two-systems}

A sincronização de oportunidade é unidirecional - [!DNL Dynamics] para o Marketo. Se você fizer alterações em uma oportunidade no [!DNL Dynamics], sua atualização será refletida no Marketo.

## Posso criar uma oportunidade no [!DNL Dynamics] usando o Marketo? {#can-i-create-an-opportunity-in-dynamics-using-marketo}

Não, você deve criar a oportunidade em [!DNL Dynamics] e ela será sincronizada automaticamente com o Marketo.

## Quais campos serão sincronizados com o Marketo? {#what-fields-will-sync-to-marketo}

Você pode [selecionar campos para sincronização](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} durante a instalação.

## Como uma Conta/Contato é associada a uma Oportunidade? {#how-is-an-account-contact-associated-with-an-opportunity}

O Contato/Conta pode ser associado à Oportunidade de duas maneiras:

* Ao criar uma oportunidade, o Contato (campo de pesquisa no formulário a ser contatado) e/ou a Conta (campo de pesquisa no formulário a ser contado) podem ser definidos. Em ambos os casos, esses valores são armazenados no campo Cliente em potencial (customerid) no Dynamics. Este campo não aparece no formulário de oportunidade, mas pode ser adicionado das configurações. Este campo pode conter apenas 1 valor, seja contato ou conta. A Marketo faz o seguinte:

   * Se o valor do contato for definido e a conta for deixada vazia, a Marketo criará um `opportunitycontactrole` e definirá a conta na oportunidade para a conta do contato. Se o contato não tiver uma conta, esse campo ficará vazio.
   * Se o valor da conta for definido e o contato for deixado em branco, a Marketo somente definirá a conta na oportunidade para essa conta.
   * Se ambos os valores forem definidos, o Dynamics escolherá a conta como o valor de customerid, para que o comportamento seja o mesmo acima.

* Por meio das partes interessadas: o Dynamics usa conexões para conectar a oportunidade ao contato por meio das partes interessadas da página de criação da oportunidade. Para isso, criaremos um registro `opportunitycontactrole` para cada nova parte interessada.
