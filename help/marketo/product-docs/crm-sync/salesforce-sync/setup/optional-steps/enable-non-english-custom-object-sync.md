---
unique-page-id: 4719302
description: Habilitar sincronização de objetos personalizados em outros idiomas - Documentos do Marketo - Documentação do produto
title: Habilitar sincronização de objetos personalizados em outros idiomas
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Habilitar sincronização de objetos personalizados em outros idiomas {#enable-non-english-custom-object-sync}

Se o usuário de sincronização do Marketo estiver definido em um idioma diferente do inglês, você poderá encontrar um erro ao tentar ativar a sincronização de objetos personalizados.

## O erro {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Conheça {#getting-around-it}

1. Faça logon no Salesforce usando o usuário de sincronização do marketo.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Em nome do usuário, acesse **Configuração**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Em **Informações pessoais**, clique em **Minhas informações pessoais**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Clique em **Editar**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Altere o **Idioma** para **Inglês**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Clique em **Salvar**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. De volta ao Marketo, em **Admin > Salesforce > Objetos** click **Atualizar esquema**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Essa ação extrairá a lista de objetos em inglês. Em seguida, selecione o objeto de sua escolha e clique em **Ativar Sincronização**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Observe que seu objeto personalizado agora está ativado e sincronizado.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Agora volte para o Salesforce e use as etapas acima para alterar o usuário de sincronização de volta para seu idioma preferencial.

>[!NOTE]
>
>Não se esqueça de atualizar o esquema uma última vez para puxar os objetos de volta no seu idioma.
