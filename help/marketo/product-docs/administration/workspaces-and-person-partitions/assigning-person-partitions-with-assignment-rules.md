---
unique-page-id: 2360327
description: Como configurar regras de atribuição para rotear pessoas do seu CRM para as partições de pessoas corretas.
title: Atribuição de partições de pessoa com regras de atribuição
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
TQID: 'https://experienceleague.adobe.com/7e7A0wXFiKVttSm7BXEJYtVBnSW6qAah1ygNqO4qdr0'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b4e49ca2-9149-5443-90e6-11978bb87c2f
    internal-label: Partitions
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 10%
---
# Atribuição de partições de pessoa com regras de atribuição {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**Permissões de administrador são necessárias**

>[!PREREQUISITES]
>
>[Criar uma Partição de Pessoa](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

Ao usar partições de pessoa, configure regras de atribuição para rotear as pessoas criadas pelo seu CRM para suas respectivas partições.

>[!NOTE]
>
>Somente as pessoas criadas no Marketo pelo seu CRM e pela API do SOAP terão regras de atribuição aplicadas a elas.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. Clique em **[!UICONTROL Espaços de trabalho e partições]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. Na guia **[!UICONTROL Partições de pessoa]**, clique em **[!UICONTROL Regras de atribuição]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. Clique em **[!UICONTROL Adicionar opção]** para adicionar condições para rotear pessoas para partições de pessoas.

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. Selecione o campo no qual a condição deve ser criada.

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. Escolha o operador e insira um valor.

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. Selecione a Partição de Pessoas na qual você deseja que as pessoas que atendem às condições se encaixem.

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >Você pode adicionar quantas escolhas desejar.

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

As regras de atribuição para suas partições de pessoa foram configuradas.

>[!NOTE]
>
>A opção padrão será aplicada se nenhuma das condições anteriores for atendida.
