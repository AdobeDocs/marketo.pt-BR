---
unique-page-id: 3571830
description: Etapa 3 de 3 - Conectar o Microsoft Dynamics com o Marketing (Online) - Documentos do Marketing - Documentação do produto
title: Etapa 3 de 3 - Conectar o Microsoft Dynamics com o Marketing (Online)
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---


# Etapa 3 de 3: Conectar o Microsoft Dynamics com o Marketing (Online) {#step-of-connect-microsoft-dynamics-with-marketo-online}

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Esta é a última etapa da sincronização. Estamos quase lá!

>[!NOTE]
>
>**Pré-requisitos**
>
>* [Etapa 1 de 3: Instalar a solução Marketing (Online)](step-1-of-3-install.md)
   >
   >
* [Etapa 2 de 3: Configurar usuário de sincronização de marketing no Dynamics](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**Permissões de administrador necessárias**

## Digite as informações do usuário do Dynamics Sync {#enter-dynamics-sync-user-information}

1. Faça logon no Marketo e clique em **Admin**.

   ![](assets/login-admin.png)

1. Clique em **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Selecione **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Clique em **Editar** na **Etapa 1: Insira credenciais**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Verifique se suas credenciais estão corretas, pois não é possível reverter as alterações subsequentes no schema após o envio. Se as credenciais incorretas forem salvas, será necessário obter uma nova subscrição de marketing.

1. Digite o **Nome** de usuário, a **Senha** e o **URL** do Microsoft Dynamics (a ID do cliente e o Segredo do cliente são opcionais). Clique em **Salvar** quando concluído.

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >O Nome de usuário no Marketo deve corresponder ao Nome de usuário para o usuário de sincronização no CRM. O formato pode ser [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#bcc9cfd9cefcd8d3d1ddd5d292dfd3d1) DOMAIN\user.

## Selecionar campos a serem sincronizados {#select-fields-to-sync}

1. Clique em **Editar** na **Etapa 2: Selecione Campos para sincronização**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Selecione os campos que deseja sincronizar com o Marketo, de modo que eles sejam pré-selecionados. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

## Sincronizar campos para um filtro personalizado {#sync-fields-for-a-custom-filter}

Se você criou um filtro personalizado, certifique-se de entrar e selecionar os novos campos a serem sincronizados com o Marketo.

1. Vá para Admin e selecione **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e verifique-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer coisa. Clique em **Salvar**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Ativar sincronização {#enable-sync}

1. Clique em **Editar** na **Etapa 3: Ative Sincronizar**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >O Marketo não eliminará a duplicação automaticamente em relação a uma sincronização do Microsoft Dynamics ou quando você inserir pessoas ou clientes em potencial manualmente.

1. Leia tudo no pop-up, digite seu endereço de email e clique em Sincronização **de** Start.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. A primeira sincronização pode levar algumas horas. Quando terminar, você receberá uma notificação por email.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Excelente trabalho!
