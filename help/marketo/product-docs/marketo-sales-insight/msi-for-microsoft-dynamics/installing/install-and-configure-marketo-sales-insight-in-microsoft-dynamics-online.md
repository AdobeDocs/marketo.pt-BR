---
unique-page-id: 37355602
description: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics Online - Documentação do Marketo - Documentação do produto
title: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 1%

---

# Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

O Marketo Sales Insight é uma ferramenta fantástica para fornecer à sua equipe de vendas uma &quot;janela&quot; para a riqueza de dados que a equipe de marketing possui. Veja como instalá-lo e configurá-lo no Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Conclua sua integração Marketo-Microsoft.
>
>[Baixe a solução correta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para a sua versão do Microsoft Dynamics CRM.

## Importar solução {#import-solution}

>[!NOTE]
>
>Se você estiver usando a Interface Unificada, antes da Etapa 1 abaixo, clique no ícone Configurações no canto superior direito e selecione **Configurações Avançadas**.

1. Em Microsoft Dynamics CRM, clique em **Configurações**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Em Configurações, clique em **Personalizações**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Clique em **Soluções**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >É necessário que você já tenha instalado e configurado a solução Marketo antes de prosseguir.

1. Clique em **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Na nova janela, clique em **Procurar**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. No computador, localize e instale a solução que você acabou de baixar.

1. Clique em **Avançar**.

   ![](assets/seven.png)

1. A solução será carregada. Você pode visualizar o conteúdo do pacote se desejar. Clique em **Avançar**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Certifique-se de deixar a caixa marcada e clique em **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Você pode baixar o arquivo de log e clicar em **Fechar**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Fantástico! Você deve ver a solução agora. Se não estiver lá, atualize a tela.

   ![](assets/eleven.png)

1. Clique em **Personalização do Publish**.

   >[!NOTE]
   >
   >Habilite a sincronização Global do MS Dynamics.

## Conecte o Marketo e o Sales Insight {#connect-marketo-and-sales-insight}

Vamos vincular sua instância do Marketo ao Sales Insight in Dynamics. Veja como:

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no Marketo e vá para a seção **Administrador**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Na seção Insight de vendas, clique em **Editar configuração de API**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copie o **Host do Marketo**, a **URL da API** e a **ID de Usuário da API** para usar em uma etapa posterior. Insira uma Chave secreta de API de sua escolha e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) na sua chave secreta da API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Os seguintes campos devem ser sincronizados com o Marketo para que _o cliente potencial e o contato_ funcionem:
   >
   >* Prioridade
   >* Urgência
   >* Pontuação relativa
   >
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De volta ao Microsoft Dynamics, vá para **Configurações**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Em **Configurações**, clique em **Configuração da API do Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Clique em **Novo**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Insira as informações que você obteve do Marketo anteriormente e clique em **Salvar**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Ativar sincronização {#enable-sync}

1. No Marketo, clique em **Admin**.

   ![](assets/enable-one.png)

1. Em Integração, selecione **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Clique em **Habilitar sincronização**.

   ![](assets/enable-three.png)

1. Clique em **Editar** ao lado de Detalhes da sincronização de campo.

   ![](assets/enable-four.png)

1. Isso _automaticamente_ selecionará campos MSI que foram desabilitados anteriormente (Urgência, Pontuação relativa e Prioridade). Basta clicar em **Salvar** em para começar a sincronizar dados.

   ![](assets/enable-five.png)

## Definir acesso do usuário {#set-user-access}

Por fim, é necessário conceder a usuários específicos acesso para usar o Marketo Sales Insight.

1. Vá para **Configurações**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Vá para **Segurança**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Clique em **Usuários**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Selecione os usuários aos quais você deseja conceder acesso ao Sales Insight e clique em **Gerenciar funções**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Selecione a função Marketo Sales Insight e clique em **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   E você deveria estar pronto! Por fim, para testar, faça logon no Dynamics como um usuário com acesso ao Marketo Sales Insight e veja um cliente potencial ou contato.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Configurando Estrelas e Chamas para Registros de Cliente Potencial/Contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
