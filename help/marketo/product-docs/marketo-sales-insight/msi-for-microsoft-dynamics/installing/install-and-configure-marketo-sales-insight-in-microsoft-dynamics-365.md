---
unique-page-id: 3571739
description: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 365 - Documentos do Marketo - Documentação do produto
title: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 365
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 1%

---

# Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

O Marketo Sales Insight é uma ferramenta fantástica para dar à sua equipe de vendas uma &quot;janela&quot; sobre a riqueza de dados que a equipe de marketing tem. Veja como instalar e configurar.

>[!PREREQUISITES]
>
>Conclua a integração Marketo-Microsoft.
>
>[Baixe a solução correta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para sua versão do Microsoft Dynamics CRM.

## Importar Solução {#import-solution}

1. Faça logon em [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Clique no botão ![—](assets/image2015-3-16-16-1-13.png) e selecione **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Clique no botão ![—](assets/image2015-5-13-10-5-8.png) menu. No menu suspenso , selecione **Configurações**, em seguida selecione **Soluções**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >Você já deveria ter [instalada e configurada a solução Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) antes de avançar.

1. Clique em **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Na nova janela, clique em **Procurar**. Escolha a [Solução Marketo Sales Insight que você baixou na etapa 1](#msi). Clique em **Próximo**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. A solução será carregada. Você pode exibir o conteúdo do pacote, se desejar. Clique em **Próximo**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Certifique-se de deixar a caixa **verificado** e clique em **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Você pode baixar o arquivo de log. Clique em **Fechar**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Ótimo! Você deve ver a solução agora. Se não estiver lá, atualize a tela.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Clique em **Publicar todas as personalizações**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Conectar o Marketo e o Insight de vendas {#connect-marketo-and-sales-insight}

Vamos vincular sua instância do Marketo ao Sales Insight no Dynamics. Veja como:

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no Marketo e acesse o **Administrador** seção.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Em **Insight de vendas** seção , clique em **Editar configuração da API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie o **Host Marketo**, **URL da API** e **ID de usuário da API** para uso em uma etapa posterior. Insira um **Chave secreta da API** de sua escolha e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Os seguintes campos devem ser sincronizados com o Marketo para _Tanto o Cliente Potencial como o Contato_ para que o Sales Insight funcione:
   >
   > * Prioridade
   > * Urgência
   > * Pontuação relativa

   >
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De volta ao Microsoft Dynamics, clique no botão ![](assets/image2015-5-13-15-3a49-3a19.png) ícone ao lado de Configurações e selecione **Configuração da API do Marketo** na lista suspensa.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Clique em **Configuração padrão**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Insira as informações copiadas do Marketo anteriormente.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Clique no botão ![](assets/image2015-5-13-16-3a8-3a51.png) no canto inferior direito para salvar as alterações.

## Definir acesso do usuário {#set-user-access}

Você precisa conceder aos usuários permissões para usar o Sales Insight.

1. Clique no botão ![](assets/image2015-5-13-10-3a5-3a8.png) menu. No menu suspenso , selecione **Configurações**, em seguida selecione **Segurança**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Clique em **Usuários**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Selecione os usuários aos quais deseja conceder acesso ao Sales Insight e clique **Gerenciar funções**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Selecione o **Insight sobre vendas da Marketo** função e clique **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E você deveria estar pronto! Por fim, para testar, faça logon no Dynamics como um usuário que tem acesso ao Marketo Sales Insight e olhe um cliente potencial ou contato.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Agora você desbloqueou o poder do Marketo Sales Insight para sua equipe de vendas.

>[!MORELIKETHIS]
>
>[Configuração de estrelas e chamas para registros de lead/contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
