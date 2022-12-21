---
unique-page-id: 1147066
description: Substituir restrições de pessoa em uma campanha inteligente - Documentos do Marketo - Documentação do produto
title: Substituir restrições de pessoa em uma campanha inteligente
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Substituir restrições de pessoa em uma campanha inteligente {#override-person-restrictions-in-a-smart-campaign}

O Marketo permite definir o número máximo de pessoas que podem se qualificar para uma campanha inteligente; isso ajuda a evitar o envio acidental de todo o banco de dados. Se desejar _override_ este limite, veja como.

>[!PREREQUISITES]
>
>Certifique-se de [ativar restrições de pessoa para campanhas inteligentes](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) no Marketo Admin.

1. Em Atividades de marketing, acesse sua campanha inteligente e clique em **Agendar**.

   ![](assets/one.png)

1. Nas Configurações da campanha inteligente, clique em **Editar**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >O limite padrão é aquele definido em Admin.

1. Insira um novo limite e clique em **Salvar.**

   ![](assets/three.png)

   A campanha inteligente não será executada se o número de pessoas que se qualificam exceder o limite definido.

   >[!CAUTION]
   >
   >Tenha cuidado com esse recurso para não incluir acidentalmente muitas pessoas.
