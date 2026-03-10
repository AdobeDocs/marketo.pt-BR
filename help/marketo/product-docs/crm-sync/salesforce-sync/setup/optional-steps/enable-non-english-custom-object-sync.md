---
unique-page-id: 4719302
description: Saiba como habilitar a sincronização de objetos personalizados quando o usuário de sincronização do Marketo usa um idioma diferente do inglês. Defina o idioma de sincronização do usuário para inglês no Salesforce e atualize o esquema.
title: Habilitar a sincronização de objetos personalizados com idioma diferente do inglês
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 8%

---

# Habilitar a sincronização de objetos personalizados com idioma diferente do inglês {#enable-non-english-custom-object-sync}

Se o usuário de sincronização do Marketo estiver definido com um idioma diferente do inglês, talvez ocorra um erro ao tentar habilitar uma sincronização de objeto personalizado.

## O erro {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Contornando-Se {#getting-around-it}

1. Faça logon em [!DNL Salesforce] usando a marcação para sincronizar usuário.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. No nome de usuário, vá para **[!UICONTROL Instalação]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Em **[!UICONTROL Informações Pessoais]**, clique em **[!UICONTROL Minhas Informações Pessoais]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Altere o **[!UICONTROL Idioma]** para **[!UICONTROL Inglês]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. De volta ao Marketo, em **[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objetos]**, clique em **[!UICONTROL Atualizar Esquema]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Isso obterá a lista de objetos em inglês. Agora selecione o objeto de sua escolha e clique em **[!UICONTROL Habilitar Sincronização]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Observe que o objeto personalizado agora está habilitado e sincronizando.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Agora, volte para [!DNL Salesforce] e use as etapas acima para alterar o usuário de sincronização de volta para seu idioma preferido.

>[!NOTE]
>
>Não se esqueça de atualizar o esquema uma última vez para obter os objetos de volta no seu idioma.
