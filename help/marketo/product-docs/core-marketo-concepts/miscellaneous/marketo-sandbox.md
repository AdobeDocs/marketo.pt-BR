---
unique-page-id: 11386358
description: Saiba mais sobre a sandbox da Marketo Engage para testes antes da produção. Use uma instância de sandbox para testar sem afetar a produção.
title: Sandbox do Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 8bb13497a5173f355563e2badf867a5f847be488
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 3%

---

# Sandbox do Marketo {#marketo-sandbox}

Uma sandbox da Marketo Engage é uma instância adicional usada para fins de teste antes da implementação no ambiente de produção.

>[!AVAILABILITY]
>
>Nem todos compraram este recurso. Entre em contato com a equipe de conta da Adobe (seu gerente de conta) para obter mais detalhes.

Uma sandbox da Marketo não pode ser sincronizada com o CRM normal se já estiver sincronizada com a instância de produção. Use a sandbox do CRM para a sincronização e siga as mesmas etapas da sincronização original.

## O que você deve saber sobre sandboxes {#things-to-know-about-sandboxes}

* Se quiser adicionar usuários, o processo é o mesmo que [adicionar usuários na produção](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md#add-a-user). Novamente, eles devem usar um endereço de email diferente se já tiverem um logon no Marketo.
* A sandbox da Marketo começará vazia, mas terá os mesmos recursos disponíveis que a instância de produção.
* Se você criar um programa em sua sandbox e quiser movê-lo para a produção, poderá executar uma [importação de programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* As sandboxes são limitadas para que as instâncias de produção não sejam afetadas negativamente pelos ambientes de teste. Você pode enviar até 20 emails por execução de campanha.

>[!CAUTION]
>
>A atualização da sandbox para a sincronização do Salesforce do Marketo Dynamics _or_ não é suportada no momento. Se você precisar atualizar sua sandbox do CRM, será necessária uma nova sandbox da Marketo. Entre em contato com a equipe de conta da Adobe (seu gerente de conta) para obter mais detalhes.

## Cópia da instância {#instance-copy}

É possível enviar um caso de suporte solicitando uma cópia de instância única para preencher sua sandbox. No entanto, a cópia da instância não trará _tudo_. Entre em contato com o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para obter detalhes.

>[!NOTE]
>
>Se você estiver alterando o CRM nativo, será necessária uma nova instância do Marketo e não será possível fazer uma cópia da instância para a nova instância do Marketo. Em vez disso, trabalhe com o Suporte da Marketo para explorar a funcionalidade do Programa de importação.
