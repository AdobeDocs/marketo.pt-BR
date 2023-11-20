---
unique-page-id: 4719302
description: Habilitar Sincronização De Objeto Personalizado Em Outro Idioma - Documentação Do Marketo - Documentação Do Produto
title: Habilitar a sincronização de objetos personalizados em outros idiomas
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 1%

---

# Habilitar a sincronização de objetos personalizados em outros idiomas {#enable-non-english-custom-object-sync}

Se o usuário de sincronização do Marketo estiver definido com um idioma diferente do inglês, talvez ocorra um erro ao tentar habilitar uma sincronização de objeto personalizado.

## O erro {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Contornando-Se {#getting-around-it}

1. Efetue logon no [!DNL Salesforce] usando o usuário markto sync.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. No nome de usuário, acesse **[!UICONTROL Configuração]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Em **[!UICONTROL Informações pessoais]**, clique em **[!UICONTROL Minhas informações pessoais]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Altere o **[!UICONTROL Idioma]** para **[!UICONTROL Inglês]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. De volta ao Marketo, em **[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objetos]**, clique em **[!UICONTROL Atualizar esquema]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Isso obterá a lista de objetos em inglês. Agora, selecione o objeto de sua escolha e clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Observe que o objeto personalizado agora está habilitado e sincronizando.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Agora retorne ao Salesforce e use as etapas acima para alterar o usuário de sincronização de volta para seu idioma preferido.

>[!NOTE]
>
>Não se esqueça de atualizar o esquema uma última vez para obter os objetos de volta no seu idioma.
