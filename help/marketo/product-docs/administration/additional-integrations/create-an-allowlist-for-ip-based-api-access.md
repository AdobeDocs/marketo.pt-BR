---
unique-page-id: 10098433
description: Criar um novo Incluo na lista de permissões para acesso à API com base em IP - Documentação do Marketo - Documentação do produto
title: Criar uma lista de permissões de acesso à API baseada em IP
exl-id: 1a2f2216-07ee-4d37-b883-458ea39fc452
feature: Administration
source-git-commit: 3595cdc76a0f92da10dc5ddaac64c4cf83056e88
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 10%

---

# Criar uma lista de permissões de acesso à API baseada em IP {#create-an-allowlist-for-ip-based-api-access}

Às vezes, você deseja conceder à API acesso somente a um endereço IP específico ou a um intervalo de endereços. Para fazer isso, primeiro habilite as restrições e, em seguida, especifique os endereços IP que podem usar as APIs.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>Este recurso opera independentemente das [restrições de logon baseadas em IP](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} do Marketo Engage, que estão sendo substituídas pelo [controle de acesso baseado em IP](https://helpx.adobe.com/br/enterprise/using/ip-based-access.html){target="_blank"} do Admin Console. Ele continuará funcionando como está após a migração do Adobe IMS.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-1.png)

1. Clique em **[!UICONTROL Serviços da Web]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-2.png)

1. Na área **[!UICONTROL Restrições de IP]**, clique em **[!UICONTROL Editar],** ou em **[!UICONTROL Editar Restrições de IP]** no canto superior esquerdo.

   ![](assets/create-an-allowlist-for-ip-based-api-access-3.png)

1. Incluir na lista de permissões Marque a caixa **[!UICONTROL Habilitar Restrições de IP]** e insira os endereços IP que deseja modificar.

   ![](assets/create-an-allowlist-for-ip-based-api-access-4.png)

   >[!NOTE]
   >
   >Você pode inserir um único endereço IP ou um intervalo deles, ou usar um curinga.

1. Clique em **[!UICONTROL Adicionar]** para abrir campos adicionais para inserir mais endereços IP.

   ![](assets/create-an-allowlist-for-ip-based-api-access-5.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/create-an-allowlist-for-ip-based-api-access-6.png)
