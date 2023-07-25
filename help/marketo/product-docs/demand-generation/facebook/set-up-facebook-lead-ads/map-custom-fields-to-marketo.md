---
unique-page-id: 12983101
description: Mapear campos personalizados para o Marketo - Documentação do Marketo - Documentação do produto
title: Mapear campos personalizados para o Marketo
exl-id: c52c9bcb-6448-4ebe-b87f-9e3a48e3d27d
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Mapear campos personalizados para o Marketo {#map-custom-fields-to-marketo}

Você pode coletar mais do que as informações padrão que a Facebook armazena por padrão, como a frequência com que alguém usa seu serviço de delivery online. Você pode fazer isso ao [criação de perguntas personalizadas](https://www.facebook.com/business/help/774623835981457?helpref=uf_permalink) nos seus anúncios de clientes potenciais do Facebook.

No entanto, **O Marketo não iniciará automaticamente a coleta desses dados**. Para que o Marketo comece a capturar valores de campos personalizados, você **deve** mapeie esses campos personalizados para um campo no Marketo.

Veja como configurar isso na área LaunchPoint do Administrador.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Vá para a área Admin e clique em **LaunchPoint**. Em Serviços Instalados, localize e edite **Anúncios de clientes potenciais do facebook**.

   ![](assets/image2017-10-24-9-3a32-3a16.png)

1. Clique em **Próxima**.

   ![](assets/image2017-10-24-14-3a55-3a13.png)

1. Deixar a conta autorizada como está — fazer **não** fazer alterações. Clique em **Próxima**.

   ![](assets/image2017-10-24-14-3a56-3a48.png)

1. Como antes, deixe as páginas selecionadas como estão — faça **não** fazer alterações. Clique em **Próxima**.

   ![](assets/image2017-10-24-15-3a0-3a54.png)

1. É aqui que você mapeia o campo personalizado do Facebook para o campo do Marketo. Clique em **Adicionar.**

   ![](assets/image2017-10-24-9-3a33-3a49.png)

1. Na nova linha, digite o nome do campo personalizado do Facebook.

   ![](assets/image2017-10-24-9-3a37-3a3.png)

   >[!NOTE]
   >
   >Somente os campos que foram salvos em modelos de formulário do Facebook aparecerão como opções aqui.

1. Clique em **Campo do Marketo** coluna. Digite para procurar o campo para o qual deseja mapear. Depois de selecionar um campo, clique em **Salvar**.

   ![](assets/image2017-10-24-11-3a16-3a42.png)

   >[!NOTE]
   >
   >Se você ainda não tiver um campo no Marketo para mapear o campo do Facebook, saiba como [criar campos personalizados](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md).

>[!CAUTION]
>
>Você **deve** passe por esse processo para qualquer novo campo do Facebook para que o Marketo colete os dados.
