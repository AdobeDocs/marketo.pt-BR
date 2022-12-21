---
unique-page-id: 37355602
description: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics Online - Documentos do Marketo - Documentação do produto
title: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 1%

---

# Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

O Marketo Sales Insight é uma ferramenta fantástica para dar à sua equipe de vendas uma &quot;janela&quot; sobre a riqueza de dados que a equipe de marketing tem. Veja como instalá-lo e configurá-lo no Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Conclua a integração Marketo-Microsoft.
>
>[Baixe a solução correta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para sua versão do Microsoft Dynamics CRM.

## Importar Solução {#import-solution}

>[!NOTE]
>
>Se estiver usando a Interface Unificada, antes da Etapa 1 abaixo, clique no ícone Configurações no canto superior direito e selecione **Configurações avançadas**.

1. Em Microsoft Dynamics CRM, clique em **Configurações**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. Em Configurações, clique em **Personalizações**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Clique em **Soluções**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Você já deve ter instalado e configurado a solução da Marketo antes de seguir em frente.

1. Clique em **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Na nova janela, clique em **Procurar**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. No computador, encontre e instale a solução que acabou de baixar.

1. Clique em **Próximo**.

   ![](assets/seven.png)

1. A solução será carregada. Você pode exibir o conteúdo do pacote, se desejar. Clique em **Próximo**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Certifique-se de deixar a caixa marcada e clique em **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Você pode baixar o arquivo de log e, em seguida, clicar em **Fechar**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Ótimo! Você deve ver a solução agora. Se não estiver lá, atualize a tela.

   ![](assets/eleven.png)

1. Clique em **Publicar personalização**.

   >[!NOTE]
   >
   >Certifique-se de ativar a sincronização do Global MS Dynamics.

## Conectar o Marketo e o Insight de vendas {#connect-marketo-and-sales-insight}

Vamos vincular sua instância do Marketo ao Sales Insight no Dynamics. Veja como:

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no Marketo e acesse o **Administrador** seção.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Na seção Informações de vendas , clique em **Editar configuração da API**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copie o **Host Marketo**, **URL da API** e **ID de usuário da API** para uso em uma etapa posterior. Insira uma chave secreta de API de sua escolha e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Os seguintes campos devem ser sincronizados com o Marketo para _Tanto o Cliente Potencial como o Contato_ para que o Sales Insight funcione:
   >
   >* Prioridade
   >* Urgência
   >* Pontuação relativa

   >
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De volta ao Microsoft Dynamics, acesse **Configurações**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Em **Configurações**, clique em **Configuração da API do Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Clique em **Novo**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Insira as informações obtidas do Marketo anteriormente e clique em **Salvar**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Ativar sincronização {#enable-sync}

1. No Marketo, clique em **Administrador**.

   ![](assets/enable-one.png)

1. Em Integração, selecione **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Clique em **Ativar Sincronização**.

   ![](assets/enable-three.png)

1. Clique em **Editar** ao lado de Detalhes de sincronização de campo.

   ![](assets/enable-four.png)

1. Esse _automaticamente_ selecione os campos MSI que foram desabilitados anteriormente (Urgência, Pontuação relativa e Prioridade). Basta clicar em **Salvar** para iniciar a sincronização de dados.

   ![](assets/enable-five.png)

## Definir acesso do usuário {#set-user-access}

Por fim, é necessário conceder acesso a usuários específicos para usar o Marketo Sales Insight.

1. Ir para **Configurações**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Ir para **Segurança**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Clique em **Usuários**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Selecione os usuários aos quais deseja conceder acesso ao Sales Insight e clique em **Gerenciar funções**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Selecione a função Marketo Sales Insight e clique em **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   E você deveria estar pronto! Por fim, para testar, faça logon no Dynamics como um usuário que tem acesso ao Marketo Sales Insight e olhe um cliente potencial ou contato.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Configuração de estrelas e chamas para registros de lead/contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
