---
unique-page-id: 4719306
description: Ocultar um campo do Salesforce da sincronização de marketing - Documentos do marketing - Documentação do produto
title: Ocultar um campo do Salesforce da sincronização de marketing para
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 0%

---


# Ocultar um campo do Salesforce da sincronização de marketing {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Nem todos os campos no Salesforce são úteis para Marketing. Você pode otimizar o desempenho da sincronização incluindo apenas os campos de que precisa. É assim que se pode ocultar um campo de Marketo.

1. Clique no menu de nome e selecione **Configuração**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Digite **perfis** na barra de pesquisa e clique em **Perfis** em **Gerenciar usuários**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Clique no perfil do usuário de sincronização.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Na seção **Field-Level Security**, clique em **Visualização** ao lado do objeto que contém o campo público alvo.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Clique em **Editar**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Desmarque a caixa de seleção **Visível** ao lado do campo que você deseja ocultar. Clique em **Salvar**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Se o campo que você oculta no Salesforce já tiver sido sincronizado com o Marketo, você precisará ocultá-lo no Marketo, também se não quiser usá-lo.

   É isso! Esse campo não será mais exibido no Marketo depois que a próxima sincronização for concluída.

   >[!MORELIKETHIS]
   >
   >[Ocultar e mostrar um campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md)
