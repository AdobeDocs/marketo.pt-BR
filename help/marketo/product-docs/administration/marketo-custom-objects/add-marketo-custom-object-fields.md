---
unique-page-id: 10093688
description: Adicionar campos de objeto personalizados de marketing - Documentos de marketing - Documentação do produto
title: Adicionar campos de objeto personalizados de marketing
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Adicionar campos de objeto personalizados de marketing {#add-marketo-custom-object-fields}

Depois de criar um objeto personalizado, é necessário adicionar campos a ele para atender às suas necessidades comerciais.

Os campos definem as informações específicas usadas por um objeto personalizado. Campos de link têm um trabalho especial, para conectar objetos personalizados, e são abordados em um [artigo separado](add-marketo-custom-object-link-fields.md).

1. Clique em **Admin** e, em **Gerenciamento de banco de dados**, selecione **Objetos personalizados de marketing**.

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. Selecione o objeto ao qual deseja adicionar o campo à direita.

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. Na guia **Campos **, clique em **Novo campo**.

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >Os três campos mostrados acima são criados automaticamente pelo Marketo quando você cria um objeto personalizado. O Marketo gerencia esses campos automaticamente e você não pode editá-los ou excluí-los.

1. Insira um nome de exibição e uma descrição.

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >O nome da API pode ser editado somente até que seja aprovado.

1. Agora, escolha um tipo de dados apropriado na lista.

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. Puxe o controle deslizante Dedupe para cima se quiser usar o novo campo como um identificador exclusivo. Clique em **Salvar **para concluir.

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >Ao criar um campo de desduplicação, você pode usá-lo para remover campos de duplicado no banco de dados.

1. Adicione quaisquer outros campos de que você precise.

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Se estiver criando uma estrutura um para muitos, é necessário adicionar um campo Link ao objeto personalizado. Para uma estrutura muitas para muitas, você não precisa de um campo de link no objeto personalizado, mas precisa adicionar dois campos de link no objeto intermediário. Consulte [Adicionar campos de link de objeto personalizado de marketing](add-marketo-custom-object-link-fields.md) para criar os campos de link e [Entendendo objetos personalizados de marketing](understanding-marketo-custom-objects.md) para obter mais informações sobre tipos de objetos personalizados.

>[!MORELIKETHIS]
>
>* [Adicionar campos de link de objeto personalizado de marketing](add-marketo-custom-object-link-fields.md)
>* [Editar e excluir um objeto personalizado de marketing](edit-and-delete-a-marketo-custom-object.md)
>* [Como entender objetos personalizados de marketing](understanding-marketo-custom-objects.md)
>* [Editar e excluir campos de objetos personalizados de marketing](edit-and-delete-marketo-custom-object-fields.md)

>



