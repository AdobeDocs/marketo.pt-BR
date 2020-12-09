---
unique-page-id: 3571735
description: Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics 2011 - Documentos do Marketing - Documentação do produto
title: Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics 2011
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---


# Instalar e configurar o Marketingto Sales Insight no Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

O Marketing to Sales Insight é uma ferramenta fantástica para sua equipe de vendas. Esta é a instrução passo a passo de como instalá-la e configurá-la no Microsoft Dynamics 2011 On-Premise.

>[!PREREQUISITES]
>
>Conclua sua integração [com a](http://docs.marketo.com/x/DoA2)Marketo-Microsoft.
>
>[Baixe a solução](http://docs.marketo.com/x/LoJo) correta para sua versão do Microsoft Dynamics CRM.

## Importar solução {#import-solution}

1. Faça logon no Microsoft Dynamics CRM. Clique em **Configurações** no menu inferior esquerdo.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selecione **Soluções** na árvore.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Clique em **Importar** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >
   >Você já deve ter [instalado e configurado](install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) a solução Marketo antes de avançar.

1. Clique em **Procurar**. Selecione a solução Marketing to Sales Insight que você [baixou](download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Clique em **Avançar**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Verifique os detalhes da solução e clique em **Avançar**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Verifique se a opção de mensagem do SDK está marcada. Clique em **Avançar**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Agora espere a importação terminar.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Clique em **Fechar**.

   ![](assets/crmhand.png)

1. O Marketing to Sales Insight agora será exibido na lista da solução. Sim!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Selecione Marketing to Sales Insight e clique em **Publicar todas as personalizações** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Marketing e insight de vendas do Connect  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no Marketo e clique em **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Na seção **Sales Insight **clique em **Editar configuração** da API.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie o Host **do** Marketo, o URL **da** API e a ID **do usuário da** API para uso em uma etapa posterior. Digite uma chave **secreta da** API de sua escolha e clique em **SALVAR**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

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

1. Volte para Dinâmicas e selecione **Configurações**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selecione **Marketo API Config** na árvore.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Clique em Configuração **** padrão.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Insira as informações que você tirou do Marketo anteriormente.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Clique em **Salvar.**

   ** ![](assets/image2015-5-4-11-3a28-3a13.png)

   **

## Definir acesso do usuário {#set-user-access}

Configure funções de usuário para conceder acesso a usuários específicos ao Sales Insight.

1. Selecione **Configurações**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Selecione **Administração** na árvore.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Clique em **Usuários**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Selecione os usuários aos quais deseja conceder acesso e clique em **Gerenciar funções**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Selecione a função **Marketing** Sales Insight e clique em **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   E é isso! Todos os usuários têm acesso agora poderão ver a seção de informações de vendas na visualização de detalhes do cliente potencial/contato.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Parabéns. Você agora liberou o poder do Marketing Sales Insight.

>[!NOTE]
>
>**Artigos relacionados**
>
>[Configuração de estrelas e chamas para registros de cliente potencial/contato](http://docs.marketo.com/x/BICMAg)

