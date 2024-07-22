---
description: Como configurar o rastreamento de domínio personalizado - Documentação do Marketo - Documentação do produto
title: Como configurar o rastreamento de domínio personalizado
exl-id: 6dea7f3d-d44d-4f67-af44-a8963c95c378
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Como configurar o rastreamento de domínio personalizado {#how-to-set-up-custom-domain-tracking}

O Rastreamento de domínio personalizado permite que sua equipe use o nome da própria empresa em todos os links rastreáveis adicionados aos emails de vendas. Depois de configurar isso, incluiremos na lista de permissões qualquer link que você tiver no seu e-mail para aparecer como go.yourcompany.com, para que, quando alguém passar o mouse sobre um link, ele leia go.yourcompany.com em vez de go.toutapp.com.

Você precisará da assistência da sua equipe de TI para configurar um registro CNAME para o seu domínio que aponte para go.toutapp.com. Esse CNAME será o que aparece em todos os links de rastreamento (por exemplo, go.yourcompany.com).

Depois de confirmar com sua equipe de TI que o CNAME está configurado corretamente, você pode adicioná-lo à página Rastreamento de domínio personalizado em Ações.

>[!NOTE]
>
>Se o CNAME não estiver configurado corretamente e você ativá-lo como seu domínio personalizado em Ações, ele poderá quebrar os links e pixels de rastreamento.

## Habilitar o rastreamento de domínio personalizado {#enable-custom-domain-tracking}

>[!NOTE]
>
>**Privilégios de administrador necessários.**

1. Clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. Em Configurações do administrador, selecione **Acompanhamento**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. Na guia Custom Domain Tracking, digite seu CNAME e clique em **Conectar**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
