---
unique-page-id: 37355602
description: Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics Online - Documentos do Marketing - Documentação do produto
title: Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics Online
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---


# Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

O Marketing Insight de vendas é uma ferramenta fantástica para dar à sua equipe de vendas uma &quot;janela&quot; sobre a riqueza de dados que a equipe de marketing tem. Veja como instalá-lo e configurá-lo no Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Conclua sua [integração com a Microsoft do Marketing](http://docs.marketo.com/x/E4A2).
>
>[Baixe a ](http://docs.marketo.com/x/LoJo) solução correta para a sua versão do Microsoft Dynamics CRM.

## Importar solução {#import-solution}

>[!NOTE]
>
>Se estiver usando a Interface Unificada, antes da Etapa 1 abaixo, clique no ícone Configurações no canto superior direito e selecione **Configurações avançadas**.

1. Em Microsoft Dynamics CRM, clique em **Configurações**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Em CONFIGURAÇÕES, clique em **Personalizações**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Clique em **Soluções**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Você já deve ter instalado e configurado a solução Marketo antes de avançar.

1. Clique em **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Na nova janela, clique em **Procurar**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. No computador, encontre e instale a solução que acabou de baixar.
1. Clique em **Próximo**.

   ![](assets/seven.png)

1. A solução será carregada. Você pode visualização o conteúdo do pacote, se desejar. Clique em **Próximo**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Certifique-se de deixar a caixa marcada e clique em **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Sinta-se à vontade para baixar o arquivo de log e clique em **Fechar**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Incrível! Você deveria ver a solução agora. Se não estiver lá, atualize sua tela.

   ![](assets/eleven.png)

1. Clique em **Publicar personalização**.

   >[!NOTE]
   >
   >Certifique-se de ativar a sincronização Global do MS Dynamics.

## Connect Marketing e insights de vendas {#connect-marketo-and-sales-insight}

Vinculemos sua instância de Marketo ao Sales Insight in Dynamics. Veja como:

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no Marketo e vá para a seção **Admin **Admin.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Na seção Sales Insight, clique em **Editar configuração da API**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copie as **ID de usuário da API**, **URL da API** e **ID de usuário da API** para uso em uma etapa posterior. Digite uma chave secreta da API de sua escolha e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Os campos a seguir devem ser sincronizados com o Marketo para *lead e Contact* para que o Sales Insight funcione:
   >
   >    
   >    
   >    * Prioridade
   >    * Urgência
   >    * Pontuação relativa

   >    
   >    
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De volta ao Microsoft Dynamics, vá para **Settings**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Em **Configurações**, clique em **Configuração da API do Marketing**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Clique em **Novo**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Digite as informações que você tirou do Marketo anteriormente e clique em **Salvar**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Ativar sincronização {#enable-sync}

1. Em Marketo, clique em **Admin**.

   ![](assets/enable-one.png)

1. Em Integração, selecione **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Clique em **Ativar sincronização**.

   ![](assets/enable-three.png)

1. Clique em **Editar** ao lado de Detalhes de sincronização de campo.

   ![](assets/enable-four.png)

1. Isso *selecionará automaticamente* os campos MSI que foram desativados anteriormente (Urgência, Pontuação relativa e Prioridade). Basta clicar em **Salvar** para que o start sincronize os dados.

   ![](assets/enable-five.png)

## Definir acesso do usuário {#set-user-access}

Por fim, é necessário conceder a usuários específicos acesso para usar o Marketing Insight de vendas.

1. Vá para **Configurações**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Vá para **Security**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Clique em **Usuários**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Selecione os usuários aos quais deseja conceder acesso ao Sales Insight e clique em **Gerenciar funções**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Selecione a função Informações de vendas de marketing e clique em **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   E você deveria estar pronto! Por fim, para testar, faça logon no Dynamics como um usuário que tem acesso ao Marketing to Sales Insight e observe uma oportunidade potencial ou contato.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Configuração de estrelas e chamas para registros de cliente potencial/contato](http://docs.marketo.com/x/BICMAg)

