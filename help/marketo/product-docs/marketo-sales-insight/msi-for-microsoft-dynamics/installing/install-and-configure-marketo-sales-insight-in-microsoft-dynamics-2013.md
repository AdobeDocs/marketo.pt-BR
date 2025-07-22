---
unique-page-id: 3571737
description: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2013 - Documentação do Marketo - Documentação do produto
title: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 2%

---

# Instalar e Configurar o [!DNL Marketo Sales Insight] no [!DNL Microsoft Dynamics 2013] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

O [!DNL Marketo Sales Insight] é uma ferramenta fantástica para fornecer à sua equipe de vendas uma &quot;janela&quot; para a riqueza de dados que a equipe de marketing possui. Veja como instalá-lo e configurá-lo.

>[!PREREQUISITES]
>
>Conclua sua integração Marketo-Microsoft.
>
>[Baixe a solução correta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para a sua versão do CRM [!DNL Microsoft Dynamics].

## Importar solução {#import-solution}

OK, agora é hora de importar a solução [!DNL Marketo Sales Insight] para o [!DNL Microsoft Dynamics].

1. Em **[!UICONTROL Microsoft Dynamics CRM]**, clique em **[!UICONTROL Configurações]**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Personalizações]**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Clique em **[!UICONTROL Soluções]**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Você já deve ter instalado e configurado o Marketo antes de prosseguir

1. Clique em **[!UICONTROL Importar]**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Na nova janela, clique em **[!UICONTROL Procurar]**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Localize e selecione a solução baixada acima.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. A solução será carregada. Você pode visualizar o conteúdo do pacote se desejar. Clique em **[!UICONTROL Avançar]**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Certifique-se de deixar a caixa marcada e clique em **[!UICONTROL Importar]**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sinta-se à vontade para baixar o arquivo de log. Clique em **[!UICONTROL Fechar]**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantástico! Você deve ver a solução agora. Se não estiver lá, atualize a tela.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Conecte o Marketo e o Sales Insight {#connect-marketo-and-sales-insight}

Vamos vincular sua instância do Marketo a [!DNL Sales Insight] em [!DNL Dynamics].

>[!NOTE]
>
>É necessário ter direitos de administrador.

1. Faça logon no Marketo e vá para a seção **[!UICONTROL Administrador]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Na seção **[!UICONTROL Sales Insight]**, clique em **[!UICONTROL Editar configuração de API]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie o **[!UICONTROL Host do Marketo]**, a **[!UICONTROL URL da API]** e a **[!UICONTROL ID de Usuário da API]** para usar em uma etapa posterior. Insira uma **[!UICONTROL Chave secreta de API]** de sua escolha e clique em **[!UICONTROL Salvar]**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) na sua chave secreta da API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Os seguintes campos devem ser sincronizados com o Marketo Insight para que _o cliente potencial e o contato_ funcionem:
   >
   >* Prioridade
   >* Urgência
   >* Pontuação relativa
   >
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De volta a [!DNL Microsoft Dynamics], vá para **[!UICONTROL Configurações]**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Configuração da API do Marketo]**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Insira as informações que você obteve do Marketo anteriormente e clique em **[!UICONTROL Salvar]**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Definir acesso do usuário {#set-user-access}

Finalmente, você pode conceder a usuários específicos acesso ao [!DNL Marketo Sales Insight].

1. Vá para **[!UICONTROL Configurações]**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Clique em **[!UICONTROL Usuários]**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Selecione os usuários aos quais você deseja conceder acesso ao Sales Insight e clique em **[!UICONTROL Gerenciar funções]**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Selecione a função **[!UICONTROL Marketo Sales Insight]** e clique em **[!UICONTROL OK]**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E você deveria estar pronto! Finalmente, para testar, faça login no [!DNL Dynamics] como um usuário que tem acesso ao [!DNL Marketo Sales Insight] e olhe um cliente em potencial ou contato.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Você desbloqueou a força do [!DNL Marketo Sales Insight] para sua equipe de vendas.

>[!MORELIKETHIS]
>
>[Configurando Estrelas e Chamas para Registros de Cliente Potencial/Contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
