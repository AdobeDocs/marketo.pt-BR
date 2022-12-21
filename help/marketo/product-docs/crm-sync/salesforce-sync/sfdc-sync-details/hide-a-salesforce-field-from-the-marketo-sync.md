---
unique-page-id: 4719306
description: Ocultar um campo do Salesforce a partir da sincronização do Marketo - Documentos do Marketo - Documentação do produto
title: Ocultar um campo do Salesforce na sincronização do Marketo
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---

# Ocultar um campo do Salesforce na sincronização do Marketo {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Nem todos os campos no Salesforce são úteis para Marketing. Você pode otimizar o desempenho da sincronização incluindo apenas os campos necessários. Veja como ocultar um campo do Marketo.

1. Clique no menu de nome e selecione **Configuração**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Enter **perfis** na barra de pesquisa e clique em **Perfis** under **Gerenciar usuários**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Clique no perfil do usuário de sincronização.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Em **Segurança no nível do campo** seção , clique em **Exibir** ao lado do objeto que contém o campo target .

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Clique em **Editar**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Desmarque a opção **Visível** caixa de seleção ao lado do campo que deseja ocultar. Clique em **Salvar**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Se o campo oculto no Salesforce já tiver sido sincronizado com o Marketo, você também precisará ocultá-lo no Marketo se não quiser usá-lo.

   Pronto! Esse campo não será mais exibido no Marketo após a conclusão da próxima sincronização.

   >[!MORELIKETHIS]
   >
   >[Ocultar e mostrar um campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
