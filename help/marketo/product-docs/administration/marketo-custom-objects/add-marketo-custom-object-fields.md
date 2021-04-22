---
unique-page-id: 10093688
description: Adicionar campos de objeto personalizados do Marketo - Documentos do Marketo - Documentação do produto
title: Adicionar campos de objeto personalizados do Marketo
translation-type: tm+mt
source-git-commit: 65182770291dc14fbe915a40403fc09b433aae86
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# Adicionar campos de objeto personalizados do Marketo {#add-marketo-custom-object-fields}

Depois de criar um objeto personalizado, é necessário adicionar campos para atender às suas necessidades comerciais.

Os campos definem as informações específicas usadas por um objeto personalizado. Os campos de link têm um trabalho especial, para conectar objetos personalizados, e são cobertos em um [artigo separado](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Clique em **Admin** e, em **Gerenciamento de Banco de Dados**, selecione **Marketo Custom Objects**.

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. Selecione o objeto ao qual deseja adicionar o campo à direita.

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. Na guia **Fields**, clique em **New Field**.

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >Os três campos mostrados acima são criados automaticamente pelo Marketo quando você cria um objeto personalizado. O Marketo gerencia esses campos automaticamente e você não pode editá-los ou excluí-los.

1. Insira um nome de exibição e uma descrição.

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >O nome da API só pode ser editado até ser aprovado.

1. Agora, escolha um tipo de dados apropriado na lista.

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. Puxe o controle deslizante Dedupe para cima se desejar usar o novo campo como um identificador exclusivo. Clique em **Save** para concluir.

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >Campos de exclusão podem ser usados para recuperar, atualizar ou excluir objetos personalizados. Cada definição de objeto personalizado deve conter pelo menos um (e não mais de três) campo de dedupe.

1. Adicione quaisquer outros campos necessários.

   >[!NOTE]
   >
   >Se estiver criando uma estrutura one-to-many, será necessário adicionar um campo Link ao objeto personalizado. Para uma estrutura de muitas para muitas, você não precisa de um campo de link no objeto personalizado, mas deve adicionar dois campos de link no objeto intermediário. Consulte [Adicionar campos de link de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) para criar os campos de link e [Compreender objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obter mais informações sobre tipos de objetos personalizados.

>[!MORELIKETHIS]
>
>* [Adicionar campos de link de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Editar e excluir um objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Editar e excluir campos de objeto personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Como entender objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

