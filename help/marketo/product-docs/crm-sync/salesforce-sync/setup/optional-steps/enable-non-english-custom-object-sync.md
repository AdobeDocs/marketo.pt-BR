---
unique-page-id: 4719302
description: Habilitar sincronização de objetos personalizados não em inglês - Documentos do marketing - Documentação do produto
title: Ativar sincronização de objetos personalizados que não sejam em inglês
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Ativar sincronização de objetos personalizados que não sejam em inglês {#enable-non-english-custom-object-sync}

Se o usuário de sincronização do Marketo estiver definido para um idioma diferente do inglês, você poderá encontrar um erro ao tentar ativar a sincronização de objetos personalizados.

## O erro {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Conheça {#getting-around-it}

1. Faça logon no Salesforce usando o marcador para sincronizar o usuário.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. No nome do usuário, vá para **Configuração**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Em Informações **** pessoais, clique em **Minhas informações** pessoais.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Clique em **Editar**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Mude o **idioma** para o **inglês**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Clique em **Salvar**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. De volta ao Marketo, em **Admin > Salesforce > Objetos** , clique em **Atualizar Schema**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Isso vai puxar a lista dos objetos em inglês. Agora selecione o objeto de sua escolha e clique em **Ativar sincronização**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Observe que seu objeto personalizado agora está ativado e sendo sincronizado.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Agora, volte para o Salesforce e use as etapas acima para alterar o usuário de sincronização de volta para seu idioma preferido.

>[!NOTE]
>
>**Lembrete**
>
>Não se esqueça de atualizar o Schema uma última vez para puxar os objetos de volta para o seu idioma.

