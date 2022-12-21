---
unique-page-id: 3571737
description: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2013 - Documentos do Marketo - Documentação do produto
title: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 2%

---

# Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

O Marketo Sales Insight é uma ferramenta fantástica para dar à sua equipe de vendas uma &quot;janela&quot; sobre a riqueza de dados que a equipe de marketing tem. Veja como instalá-lo e configurá-lo.

>[!PREREQUISITES]
>
>Conclua a integração Marketo-Microsoft.
>
>[Baixe a solução correta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para sua versão do Microsoft Dynamics CRM.

## Importar Solução {#import-solution}

Ok, agora é hora de importar a solução Marketo Sales Insight para o Microsoft Dynamics.

1. Em **Microsoft Dynamics CRM** click **Configurações**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Em **Configurações**, clique em **Personalizações**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Clique em **Soluções**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Você já deve ter instalado e configurado o Marketo antes de seguir em frente

1. Clique em **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Na nova janela, clique em **Procurar**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Encontre e selecione a solução que você baixou acima.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Clique em **Próximo**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. A solução será carregada. Você pode exibir o conteúdo do pacote, se desejar. Clique em **Próximo**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Certifique-se de deixar a caixa marcada e clique em **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Você pode baixar o arquivo de log. Clique em **Fechar**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Ótimo! Você deve ver a solução agora. Se não estiver lá, atualize a tela.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Conectar o Marketo e o Insight de vendas {#connect-marketo-and-sales-insight}

Vamos vincular sua instância do Marketo ao Sales Insight no Dynamics.

>[!NOTE]
>
>É necessário ter direitos de administrador.

1. Faça logon no Marketo e acesse o **Administrador** seção.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Em **Insight de vendas** clique na seção **Editar configuração da API**.

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
   >* Prioridade
   >* Urgência
   >* Pontuação relativa

   >
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De volta ao Microsoft Dynamics, acesse **Configurações**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Em **Configurações**, clique em **Configuração da API do Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Clique em **Novo**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Insira as informações obtidas do Marketo anteriormente e clique em **Salvar**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Definir acesso do usuário {#set-user-access}

Por fim, você pode conceder acesso a usuários específicos ao Marketo Sales Insight.

1. Ir para **Configurações**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Clique em **Usuários**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Selecione os usuários aos quais deseja conceder acesso ao Sales Insight e clique **Gerenciar funções**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Selecione o **Insight sobre vendas da Marketo** função e clique **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E você deveria estar pronto! Por fim, para testar, faça logon no Dynamics como um usuário que tem acesso ao Marketo Sales Insight e olhe um cliente potencial ou contato.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Agora você desbloqueou o poder do Marketo Sales Insight para sua equipe de vendas.

>[!MORELIKETHIS]
>
>[Configuração de estrelas e chamas para registros de lead/contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
