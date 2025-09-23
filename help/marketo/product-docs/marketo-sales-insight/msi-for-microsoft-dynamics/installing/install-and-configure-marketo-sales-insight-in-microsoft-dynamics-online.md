---
unique-page-id: 37355602
description: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics Online - Documentação do Marketo - Documentação do produto
title: Instalar e configurar o Insight de vendas do Marketo no Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 3%

---

# Instalar e Configurar o [!DNL Marketo Sales Insight] no [!DNL Microsoft Dynamics Online] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

O [!DNL Marketo Sales Insight] é uma ferramenta fantástica para fornecer à sua equipe de vendas uma &quot;janela&quot; para a riqueza de dados que a equipe de marketing possui. Veja como instalá-lo e configurá-lo no [!DNL Microsoft Dynamics Online].

>[!PREREQUISITES]
>
>Conclua sua integração Marketo-Microsoft.
>
>[Baixe a solução correta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para a sua versão do [!DNL Microsoft Dynamics CRM].

## Importar solução {#import-solution}

>[!NOTE]
>
>Se você estiver usando a Interface Unificada, antes da Etapa 1 abaixo, clique no ícone Configurações no canto superior direito e selecione **[!UICONTROL Configurações Avançadas]**.

1. Em Microsoft Dynamics CRM, clique em **[!UICONTROL Configurações]**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Em Configurações, clique em **[!UICONTROL Personalizações]**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Clique em **[!UICONTROL Soluções]**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >É necessário que você já tenha instalado e configurado a solução Marketo antes de prosseguir.

1. Clique em **[!UICONTROL Importar]**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Na nova janela, clique em **[!UICONTROL Procurar]**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. No computador, localize e instale a solução que você acabou de baixar.

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/seven.png)

1. A solução será carregada. Você pode visualizar o conteúdo do pacote se desejar. Clique em **[!UICONTROL Avançar]**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Certifique-se de deixar a caixa marcada e clique em **[!UICONTROL Importar]**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Você pode baixar o arquivo de log e clicar em **[!UICONTROL Fechar]**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Fantástico! Você deve ver a solução agora. Se não estiver lá, atualize a tela.

   ![](assets/eleven.png)

1. Clique em **[!UICONTROL Personalização de publicação]**.

   >[!NOTE]
   >
   >Habilite a sincronização Global [!DNL MS Dynamics].

## Conectar o Marketo e o [!DNL Sales Insight] {#connect-marketo-and-sales-insight}

Vamos vincular sua instância do Marketo a [!DNL Sales Insight] em [!DNL Dynamics]. Veja como:

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no Marketo e vá para a seção **[!UICONTROL Administrador]**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Na seção [!UICONTROL Sales Insight], clique em **[!UICONTROL Editar configuração de API]**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copie o **[!UICONTROL Host do Marketo]**, a **[!UICONTROL URL da API]** e a **[!UICONTROL ID de Usuário da API]** para usar em uma etapa posterior. Insira uma Chave secreta de API de sua escolha e clique em **[!UICONTROL Salvar]**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) na sua chave secreta da API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Os campos a seguir devem ser sincronizados com o Marketo para que _o Cliente Potencial e o Contato_ funcionem:[!DNL Sales Insight]
   >
   >* Prioridade
   >* Urgência
   >* Pontuação relativa
   >
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De volta a [!DNL Microsoft Dynamics], vá para **[!UICONTROL Configurações]**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Configuração da API do Marketo]**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Insira as informações que você obteve do Marketo anteriormente e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Ativar sincronização {#enable-sync}

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/enable-one.png)

1. Em Integração, selecione **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/enable-two.png)

1. Clique em **[!UICONTROL Habilitar sincronização]**.

   ![](assets/enable-three.png)

1. Clique em **[!UICONTROL Editar]** ao lado de [!UICONTROL Detalhes da sincronização de campo].

   ![](assets/enable-four.png)

1. Isso _automaticamente_ selecionará campos MSI que foram desabilitados anteriormente ([!UICONTROL Urgência], [!UICONTROL Pontuação relativa] e [!UICONTROL Prioridade]). Basta clicar em **[!UICONTROL Salvar]** em para começar a sincronizar dados.

   ![](assets/enable-five.png)

## Definir acesso do usuário {#set-user-access}

Por fim, você precisa conceder a usuários específicos acesso para usar o [!DNL Marketo Sales Insight].

1. Vá para **[!UICONTROL Configurações]**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Vá para **[!UICONTROL Segurança]**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Clique em **[!UICONTROL Usuários]**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Selecione os usuários aos quais você deseja conceder acesso a [!DNL Sales Insight] e clique em **[!UICONTROL Gerenciar Funções]**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Selecione a função [!DNL Marketo Sales Insight] e clique em **[!UICONTROL OK]**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   E você deveria estar pronto! Finalmente, para testar, faça login no [!DNL Dynamics] como um usuário que tem acesso ao [!DNL Marketo Sales Insight] e olhe um cliente em potencial ou contato.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Configurando Estrelas e Chamas para Registros de Cliente Potencial/Contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
