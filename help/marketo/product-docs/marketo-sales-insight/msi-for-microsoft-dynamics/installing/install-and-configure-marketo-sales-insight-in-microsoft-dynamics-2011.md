---
unique-page-id: 3571735
description: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2011 - Documentação do Marketo - Documentação do produto
title: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

O Marketo Sales Insight é uma ferramenta fantástica para sua equipe de vendas. Esta é a instrução passo a passo de como instalá-lo e configurá-lo no Microsoft Dynamics 2011 no local.

>[!PREREQUISITES]
>
>Conclua sua integração Marketo-Microsoft.
>
>[Baixe a solução correta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para a sua versão do Microsoft Dynamics CRM.

## Importar solução {#import-solution}

1. Entrar no Microsoft Dynamics CRM. Clique em **Configurações** no menu inferior esquerdo.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selecione **Soluções** na árvore.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Clique em **Importar** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Você já deve ter [instalado e configurado](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) a solução da Marketo antes de prosseguir.

1. Clique em **Procurar**. Selecione a solução Marketo Sales Insight que você [baixou](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Clique em **Avançar**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Verifique os detalhes da solução e clique em **Avançar**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Verifique se a opção de mensagem do SDK está marcada. Clique em **Avançar**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Agora aguarde a conclusão da importação.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Clique em **Fechar**.

   ![](assets/crmhand.png)

1. O Marketo Sales Insight será exibido na lista de soluções. Sim!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Selecione Marketo Sales Insight e clique em **Todas as personalizações do Publish** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Conecte o Marketo e o Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no Marketo e clique em **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Na seção **Sales Insight**, clique em **Editar configuração de API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie o **Host do Marketo**, a **URL da API** e a **ID de Usuário da API** para usar em uma etapa posterior. Insira uma **Chave secreta de API** de sua escolha e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) na sua chave secreta da API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Os seguintes campos devem ser sincronizados com o Marketo para que _o cliente potencial e o contato_ funcionem:
   >
   >* Prioridade
   >* Urgência
   >* Pontuação relativa
   >
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Volte para Dynamics, selecione **Configurações**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selecione **Configuração de API do Marketo** na árvore.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Clique em **Configuração Padrão**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Insira as informações que você obteve da Marketo anteriormente.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Clique em **Salvar**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Definir acesso do usuário {#set-user-access}

Configure as funções do usuário para conceder a usuários específicos acesso ao Sales Insight.

1. Selecione **Configurações**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Selecione **Administração** na árvore.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Clique em **Usuários**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Selecione os usuários aos quais deseja conceder acesso e clique em **Gerenciar Funções**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Selecione a função **Marketo Sales Insight** e clique em **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   E é isso! Todos os usuários com acesso agora poderão ver a seção sales insight na exibição detalhada de lead/contato.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Parabéns. Agora você está liberando todo o potencial do Marketo Sales Insight.

>[!MORELIKETHIS]
>
>[Configurando Estrelas e Chamas para Registros de Cliente Potencial/Contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
