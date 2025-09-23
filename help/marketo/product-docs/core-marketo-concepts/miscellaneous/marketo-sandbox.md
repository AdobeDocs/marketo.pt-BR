---
unique-page-id: 11386358
description: Marketo Sandbox — Documentação do Marketo — Documentação do produto
title: Sandbox do Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Sandbox do Marketo {#marketo-sandbox}

Uma sandbox da Marketo Engage é uma instância adicional usada para fins de teste antes da implementação no ambiente de produção.

>[!AVAILABILITY]
>
>Nem todos compraram este recurso. Entre em contato com a equipe de conta da Adobe (seu gerente de conta) para obter mais detalhes.

Uma sandbox da Marketo não pode ser sincronizada com o seu CRM normal se já estiver sincronizada com a sua instância de produção. Use a sandbox do CRM para a sincronização e siga as mesmas etapas da sincronização original.

## O que você deve saber sobre sandboxes {#things-to-know-about-sandboxes}

* Se quiser adicionar usuários, o processo é o mesmo que [adicionar usuários na produção](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). Novamente, eles devem usar um endereço de email diferente se já tiverem um logon no Marketo.
* A sandbox da Marketo começará vazia, mas terá os mesmos recursos disponíveis que a instância de produção.
* Se você criar um programa em sua sandbox e quiser movê-lo para a produção, poderá executar uma [importação de programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* As sandboxes são limitadas para que as instâncias de produção não sejam afetadas negativamente pelos ambientes de teste. Você pode enviar até 20 emails por execução de campanha.

>[!CAUTION]
>
>No momento, não há suporte para a atualização da sandbox da sincronização do Salesforce do Marketo Dynamics _ou_. Se você precisar atualizar sua sandbox do CRM, será necessária uma nova sandbox da Marketo. Entre em contato com a equipe de conta da Adobe (seu gerente de conta) para obter mais detalhes.

## Cópia da instância {#instance-copy}

É possível enviar um caso de suporte solicitando uma cópia de instância única para preencher sua sandbox. No entanto, a cópia da instância não trará _tudo_. Consulte o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para obter detalhes.

>[!NOTE]
>
>Se você estiver alterando seu CRM nativo, será necessária uma nova instância do Marketo e não será possível fazer uma cópia da instância para a nova instância do Marketo. Em vez disso, trabalhe com o Suporte da Marketo para explorar a funcionalidade do Programa de importação.
