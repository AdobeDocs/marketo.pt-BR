---
unique-page-id: 11386358
description: Sandbox da Marketo - Documentos do Marketo - Documentação do produto
title: Sandbox da Marketo
exl-id: c040fac6-2290-4de5-b27d-2c7cb28f6e30
source-git-commit: 84a285974de3bbcdf33e24befae323d3d82ef239
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Sandbox da Marketo {#marketo-sandbox}

Uma sandbox Marketo é uma instância adicional usada para fins de teste antes da implementação no ambiente de produção.

>[!AVAILABILITY]
>
>Nem todos os clientes compraram esse recurso. Entre em contato com o Gerente de sucesso do cliente para obter detalhes.

Uma sandbox do Marketo não pode ser sincronizada com seu CRM comum se já estiver sincronizada com sua instância de produção. Use a sandbox do seu CRM para a sincronização e siga todas as mesmas etapas da sincronização original.

## O que você deve saber sobre sandboxes {#things-to-know-about-sandboxes}

* Depois que o Gerente de sucesso do cliente tiver sua sandbox configurada e enviar o convite a você, você deverá usar um endereço de email diferente para fazer logon da instância de produção do Marketo.
* Se quiser adicionar usuários, o processo será o mesmo que [adicionar usuários em produção](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md#create-users). Novamente, eles devem usar um endereço de email diferente se já tiverem um logon do Marketo.
* Sua sandbox do Marketo começará vazia, mas terá os mesmos recursos disponíveis que a instância de produção.
* Se você criar um programa na sandbox e quiser movê-lo para produção, poderá executar [program import](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md).
* As sandboxes são limitadas, de modo que as instâncias de produção não sejam afetadas negativamente pelos ambientes de teste. Você pode enviar até 20 emails por execução de campanha.

>[!CAUTION]
>
>No momento, não oferecemos suporte à atualização da caixa de proteção para a Sincronização do Marketo Dynamics. Se você precisar atualizar a caixa de proteção do Dynamics CRM, será necessária uma nova caixa de proteção do Marketo. Entre em contato com o Gerente de sucesso do cliente para obter mais detalhes.

## Cópia da instância {#instance-copy}

Você pode enviar um caso de suporte solicitando uma cópia de instância única para preencher a sandbox. No entanto, a cópia da instância não trará _tudo_. Consulte [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para obter detalhes.

>[!NOTE]
>
>* A cópia da instância é **não** suportada se a instância de origem for integrada ao Microsoft Dynamics.
>* Se você estiver alterando seu CRM nativo, uma nova instância do Marketo será necessária e uma cópia da instância para a nova instância do Marketo não será possível. Em vez disso, trabalhe com o Suporte da Marketo para explorar a funcionalidade do Programa de Importação.

