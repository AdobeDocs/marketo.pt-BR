---
unique-page-id: 12983101
description: Mapear campos personalizados para o Marketo - Documentos do Marketo - Documentação do produto
title: Mapear campos personalizados para o Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Mapear campos personalizados para o Marketo {#map-custom-fields-to-marketo}

Você pode desejar coletar mais do que as informações padrão que a Facebook armazena por padrão, como com que frequência alguém usa seu serviço de entrega online. Você pode fazer isso ao [criação de perguntas personalizadas](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) nos seus anúncios de lead da Facebook.

No entanto, **O Marketo não iniciará automaticamente a coleta desses dados**. Para que o Marketo comece a capturar valores de campos personalizados, você **must** mapeie esses campos personalizados para um campo no Marketo.

Veja como configurar isso na área LaunchPoint de Admin.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para a área Admin e clique em **LaunchPoint**. Em Serviços instalados, localize e edite **Anúncios de lead da facebook**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Clique em **Próximo**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Deixe a conta autorizada como está—do **not** faça qualquer alteração. Clique em **Próximo**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Como antes, deixe as páginas selecionadas como estão—do **not** faça qualquer alteração. Clique em **Próximo**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. Aqui é onde você mapeia o campo Facebook personalizado para o campo Marketo . Clique em **Adicionar.**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Na nova linha, digite o nome do campo personalizado do Facebook.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Somente os campos que foram salvos em modelos de formulário Facebook serão exibidos como opções aqui.

1. Clique no botão **Campo Marketo** coluna. Digite para pesquisar o campo para o qual deseja mapear. Depois de selecionar um campo, clique em **Salvar**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Se ainda não tiver um campo no Marketo para mapear o campo Facebook para o, saiba como [criar campos personalizados](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Você **must** passe por esse processo para qualquer novo campo do Facebook para que o Marketo colete os dados.
