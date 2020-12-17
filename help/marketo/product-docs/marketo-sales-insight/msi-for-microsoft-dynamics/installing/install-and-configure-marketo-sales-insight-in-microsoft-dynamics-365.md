---
unique-page-id: 3571739
description: Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics 365 - Documentos do Marketing - Documentação do produto
title: Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics 365
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 0%

---


# Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

O Marketing Insight de vendas é uma ferramenta fantástica para dar à sua equipe de vendas uma &quot;janela&quot; sobre a riqueza de dados que a equipe de marketing tem. Veja como instalar e configurar.

>[!PREREQUISITES]
>
>Conclua sua [integração com a Microsoft do Marketing](http://docs.marketo.com/x/E4A2).
>
>[Baixe a ](http://docs.marketo.com/x/LoJo) solução correta para a sua versão do Microsoft Dynamics CRM.

## Importar solução {#import-solution}

1. Faça logon em [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Clique no menu ![—](assets/image2015-3-16-16-1-13.png) e selecione **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Clique no menu ![—](assets/image2015-5-13-10-5-8.png). Na lista suspensa, selecione **Settings** e, em seguida, selecione **Solutions**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Você já deve ter [instalado e configurado a solução Marketo](../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) antes de avançar.

   Clique em Importar.
   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Na nova janela, clique em **Procurar**. Escolha a [solução Marketing Insight de vendas que você baixou na etapa 1](#msi). Clique em **Próximo**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. A solução será carregada. Você pode visualização o conteúdo do pacote, se desejar. Clique em **Próximo**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Certifique-se de deixar a caixa **marcada** e clique em **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sinta-se à vontade para baixar o arquivo de log. Clique em **Fechar**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Incrível! Você deveria ver a solução agora. Se não estiver lá, atualize sua tela.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Clique em **Publicar todas as personalizações**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connect Marketing e insights de vendas {#connect-marketo-and-sales-insight}

Vinculemos sua instância de Marketo ao Sales Insight in Dynamics. Veja como:

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no Marketo e vá para a seção **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Na seção **Sales Insight**, clique em **Editar configuração da API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie as **ID do usuário da API**, **URL da API** e **ID do usuário da API** para uso em uma etapa posterior. Digite uma **chave secreta da API** de sua escolha e clique em **SALVAR**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Os campos a seguir devem ser sincronizados com o Marketo para *lead e Contact* para que o Sales Insight funcione:
   >
   > * Prioridade
   > * Urgência
   > * Pontuação relativa

   >
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De volta ao Microsoft Dynamics, clique no ícone ![](assets/image2015-5-13-15-3a49-3a19.png) ao lado de Configurações e selecione **Configuração da API do Marketing** no menu suspenso.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Clique em **Configuração Padrão**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Insira as informações que você copiou do Marketo anteriormente.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Clique no ícone ![](assets/image2015-5-13-16-3a8-3a51.png) no canto inferior direito para salvar as alterações.

## Definir acesso do usuário {#set-user-access}

É necessário conceder aos usuários permissões para usar o Sales Insight.

1. Clique no menu ![](assets/image2015-5-13-10-3a5-3a8.png). No menu suspenso, selecione **Settings** e, em seguida, selecione **Security**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Clique em **Usuários**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Selecione os usuários aos quais você deseja conceder acesso ao Sales Insight e clique em **Gerenciar funções**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Selecione a função **Marketing to Sales Insight** e clique em **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E você deveria estar pronto! Por fim, para testar, faça logon no Dynamics como um usuário que tem acesso ao Marketing to Sales Insight e observe uma oportunidade potencial ou contato.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Agora você desbloqueou o poder do Marketing Insight de Vendas para sua equipe de vendas.

>[!NOTE]
>
>**Artigos relacionados**
>
>[Configuração de estrelas e chamas para registros de cliente potencial/contato](http://docs.marketo.com/x/BICMAg)