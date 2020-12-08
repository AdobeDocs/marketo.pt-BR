---
unique-page-id: 7513865
description: Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics 2015 - Documentos do Marketing - Documentação do produto
title: Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics 2015
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics 2015 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

O Marketing Insight de vendas é uma ferramenta fantástica para dar à sua equipe de vendas uma &quot;janela&quot; sobre a riqueza de dados que a equipe de marketing tem. Veja como instalá-lo e configurá-lo no Microsoft Dynamics 2011

>[!NOTE]
>
>**Pré-requisitos**
>
>Conclua sua integração [com a](http://docs.marketo.com/x/ZwBd)Marketo-Microsoft.
>
>[Baixe a solução](http://docs.marketo.com/x/LoJo) correta para sua versão do Microsoft Dynamics CRM.

## Importar solução {#import-solution}

Ok, agora é hora de importar a solução Marketing to Sales Insight para o Microsoft Dynamics. Veja como:

1. Em Microsoft Dynamics CRM, clique em **Configurações**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Em CONFIGURAÇÕES, clique em **Personalizações**.

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. Clique em **Soluções**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Você já deve ter instalado e configurado a solução Marketo antes de avançar.

1. Clique em **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Na nova janela, clique em **Procurar**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Localize e selecione a solução que você baixou acima.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Clique em **Avançar**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. A solução será carregada. Você pode visualização o conteúdo do pacote, se desejar. Clique em **Avançar**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Certifique-se de deixar a caixa marcada e clique em **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sinta-se à vontade para baixar o arquivo de log e clique em **Fechar**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Incrível! Você deveria ver a solução agora. Se não estiver lá, atualize sua tela.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Marketing e insight de vendas do Connect {#connect-marketo-and-sales-insight}

Vinculemos sua instância de Marketo ao Sales Insight in Dynamics. Veja como:

>[!NOTE]
>
>Direitos de administrador necessários.

1. Faça logon no Marketo e vá para a seção **Admin **Admin.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Na seção Sales Insight (Informações de vendas), clique em **Edit API Configuration (Editar configuração** da API).

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie o Host **do** Marketo, o URL **da** API e a ID **do usuário da** API para uso em uma etapa posterior. Digite uma chave secreta da API de sua escolha e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Os campos a seguir devem ser sincronizados com o Marketing para que *tanto o Lead quanto o Contact* for Sales Insight funcionem:
   >
   >    
   >    
   >    * Prioridade
   >    * Urgência
   >    * Pontuação relativa

   >    
   >    
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De volta ao Microsoft Dynamics, vá para **Configurações**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Em **Configurações**, clique em Configuração **da API de** marketing.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Clique em **Novo**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Digite as informações que você tirou de Marketo anteriormente e clique em **Salvar**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Definir acesso do usuário {#set-user-access}

Por fim, é necessário conceder a usuários específicos acesso para usar o Marketing Insight de vendas.

1. Vá para **Configurações**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Vá para **Segurança**.

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. Clique em **Usuários**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Selecione os usuários aos quais deseja conceder acesso ao Sales Insight e clique em **Gerenciar funções**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Selecione a função Informações sobre vendas de marketing e clique em **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E você deveria estar pronto! Por fim, para testar, faça logon no Dynamics como um usuário que tem acesso ao Marketing to Sales Insight e observe uma oportunidade potencial ou contato.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Agora você desbloqueou o poder do Marketing Insight de Vendas para sua equipe de vendas.

>[!NOTE]
>
>**Artigos relacionados**
>
>[Configuração de estrelas e chamas para registros de cliente potencial/contato](http://docs.marketo.com/x/BICMAg)

