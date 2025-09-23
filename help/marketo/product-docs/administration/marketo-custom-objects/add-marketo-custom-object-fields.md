---
unique-page-id: 10093688
description: Adicionar campos de objeto personalizados do Marketo - Documentação do Marketo - Documentação do produto
title: Adicionar campos de objeto personalizados do Marketo
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 3%

---

# Adicionar campos de objeto personalizados do Marketo {#add-marketo-custom-object-fields}

Após criar um objeto personalizado, é necessário adicionar campos a ele para atender às suas necessidades comerciais.

Os campos definem as informações específicas usadas por um objeto personalizado. Os campos de link têm um trabalho especial, para conectar objetos personalizados, e são abordados em um [artigo separado](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/add-marketo-custom-object-fields-1.png)

1. Clique em **[!UICONTROL Objetos personalizados do Marketo]**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. Selecione o objeto ao qual deseja adicionar o campo à direita.

   ![](assets/add-marketo-custom-object-fields-3.png)

1. Clique na guia **[!UICONTROL Campos]** e depois em **[!UICONTROL Novo Campo]**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >Os três campos mostrados acima são criados automaticamente pelo Marketo quando você cria um objeto personalizado. O Marketo gerencia esses campos automaticamente e não é possível editá-los ou excluí-los.

1. Insira um [!UICONTROL Nome para Exibição] e (opcional) [!UICONTROL Descrição].

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >O [!UICONTROL Nome da API] pode ser editado somente até ser aprovado.

1. Agora, escolha um [!UICONTROL Tipo de Dados] apropriado na lista.

   ![](assets/add-marketo-custom-object-fields-6.png)

1. Puxe o controle deslizante [!UICONTROL Dedupe] se desejar usar o novo campo como um identificador exclusivo. Clique em **[!UICONTROL Salvar]** para concluir.

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >Os campos de desduplicação podem ser usados para recuperar, atualizar ou excluir objetos personalizados. Cada definição de objeto personalizado deve conter pelo menos um (e não mais de três) campos de desduplicação.

1. Adicione outros campos necessários.

   >[!NOTE]
   >
   >Se você estiver criando uma estrutura de um para muitos, será necessário adicionar um campo Link ao seu objeto personalizado. Para uma estrutura muitos para muitos, você não precisa de um campo de link no objeto personalizado, mas deve adicionar dois campos de link no objeto intermediário. Consulte [Adicionar campos de link de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) para criar os campos de link e [Noções básicas sobre objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) para obter mais informações sobre tipos de objetos personalizados.

>[!MORELIKETHIS]
>
>* [Adicionar campos de link de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Editar e excluir um objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Editar e excluir campos de objeto personalizado do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Noções básicas sobre objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
