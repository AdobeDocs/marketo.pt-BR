---
description: Como configurar o rastreamento de domínio personalizado - Documentos do Marketo - Documentação do produto
title: Como configurar o rastreamento de domínio personalizado
hide: true
hidefromtoc: true
source-git-commit: ec78e047c9dc126553fe8a4b6a4c21b0d11aea5c
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Como configurar o rastreamento de domínio personalizado {#how-to-set-up-custom-domain-tracking}

O Rastreamento de domínio personalizado permite que sua equipe use seu próprio nome de empresa em todos os links rastreáveis adicionados aos emails de vendas. Depois de configurar,  qualquer link que você tenha no seu email para que apareça como go.suaempresa.com, de modo que quando alguém passar o mouse sobre um link, ele lerá go.suaempresa.com em vez de go.toutapp.com.

Você precisará da assistência da sua equipe de TI para configurar um registro CNAME para o seu domínio que aponte para go.toutapp.com. Esse CNAME será o que aparece em todos os links de rastreamento (por exemplo, go.yourcompany.com).

Depois de confirmar com sua equipe de TI que o CNAME está configurado corretamente, você pode adicioná-lo à página Rastreamento de domínio personalizado em Ações.

>[!NOTE]
>
>Se o CNAME não estiver configurado corretamente e você ativá-lo como o domínio personalizado em Ações, ele poderá quebrar os links e pixels de rastreamento.

## Ativar o rastreamento de domínio personalizado {#enable-custom-domain-tracking}

>[!NOTE]
>
>**Privilégios de administrador necessários.**

1. Clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/how-to-set-up-custom-domain-tracking-1.png)

1. Em Configurações de administração, selecione **Rastreamento**.

   ![](assets/how-to-set-up-custom-domain-tracking-2.png)

1. Na guia Rastreamento de domínio personalizado , digite seu CNAME e clique em **Connect**.

   ![](assets/how-to-set-up-custom-domain-tracking-3.png)
