---
unique-page-id: 11386358
description: Saiba mais sobre a sandbox da Marketo Engage para testes antes da produção. Use uma instância de sandbox para testar sem afetar a produção.
title: Sandbox do Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
TQID: https://experienceleague.adobe.com/Cb1H0PKG-G0c4FkIcjI-erNzR0dwRtj7TwfqtwhFFMI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e2290edd-b061-4880-9d79-dee306cf5aa9
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 306
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
