---
unique-page-id: 4719306
description: Ocultar um campo do Salesforce na sincronização do Marketo - Documentação do Marketo - Documentação do produto
title: Ocultar um campo do Salesforce da sincronização com o Marketo
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 1%

---

# Ocultar um campo do Salesforce da sincronização com o Marketo {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Permissões de administrador necessárias**

Nem todos os campos no Salesforce são úteis para Marketing. Você pode otimizar o desempenho da sincronização incluindo apenas os campos necessários. Veja como ocultar um campo do Marketo Engage.

1. Clique no menu do seu nome e selecione **[!UICONTROL Instalação]**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Insira &quot;perfis&quot; na barra de pesquisa e clique em **[!UICONTROL Perfis]** em **[!UICONTROL Gerenciar usuários]**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Clique em sincronizar perfil do usuário.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Na seção **[!UICONTROL Segurança em Nível de Campo]**, clique em **[!UICONTROL Exibir]** ao lado do objeto que contém o campo de destino.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Clique em **[!UICONTROL Editar]**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Desmarque a caixa de seleção **[!UICONTROL Visível]** ao lado do campo que você deseja ocultar. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Se o campo ocultado no Salesforce já tiver sido sincronizado com o Marketo, será necessário ocultá-lo no Marketo, também se você não quiser usá-lo.

   Pronto! Você não verá mais esse campo no Marketo após a conclusão da próxima sincronização.

   >[!MORELIKETHIS]
   >
   >[Ocultar e Reexibir um Campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
