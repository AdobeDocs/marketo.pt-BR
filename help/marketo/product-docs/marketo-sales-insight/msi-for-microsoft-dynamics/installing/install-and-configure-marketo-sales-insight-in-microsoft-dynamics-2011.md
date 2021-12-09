---
unique-page-id: 3571735
description: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2011 - Documentos do Marketo - Documentação do produto
title: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 1%

---

# Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

O Marketo Sales Insight é uma ferramenta fantástica para sua equipe de vendas. Esta é a instrução passo a passo de como instalá-la e configurá-la no Microsoft Dynamics 2011 no local.

>[!PREREQUISITES]
>
>Conclua a integração Marketo-Microsoft.
>
>[Baixe a solução correta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para sua versão do Microsoft Dynamics CRM.

## Importar Solução {#import-solution}

1. Faça logon no Microsoft Dynamics CRM. Clique em **Configurações** no menu inferior esquerdo.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selecionar **Soluções** na árvore.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Clique em **Importar** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Você já deveria ter [instalado e configurado](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) a solução Marketo antes de seguir em frente.

1. Clique em **Procurar**. Selecione a solução Marketo Sales Insight que você [baixado](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Clique em **Próximo**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Verifique os detalhes da solução e clique em **Próximo**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Verifique se a opção SDK message está marcada. Clique em **Próximo**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Agora aguarde a conclusão da importação.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Clique em **Fechar**.

   ![](assets/crmhand.png)

1. O Marketo Sales Insight agora será exibido na lista de soluções. Sim!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Selecione Marketo Sales Insight e clique em **Publicar todas as personalizações** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Conectar o Marketo e o Insight de vendas  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no Marketo e clique em **Administrador**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Em **Insight de vendas** clique na seção **Editar configuração da API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie o **Host Marketo**, **URL da API** e **ID de usuário da API** para uso em uma etapa posterior. Insira um **Chave secreta da API** de sua escolha e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Os seguintes campos devem ser sincronizados com o Marketo para _Tanto o Cliente Potencial como o Contato_ para que o Sales Insight funcione:
   >
   >* Prioridade
   >* Urgência
   >* Pontuação relativa

   >
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Volte para Dynamics, selecione **Configurações**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selecionar **Configuração da API do Marketo** na árvore.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Clique em **Configuração padrão**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Insira as informações obtidas do Marketo anteriormente.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Clique em **Salvar**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Definir acesso do usuário {#set-user-access}

Configure as funções de usuário para conceder acesso ao Sales Insight a usuários específicos.

1. Selecionar **Configurações**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Selecionar **Administração** na árvore.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Clique em **Usuários**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Selecione os usuários aos quais deseja conceder acesso e clique em **Gerenciar funções**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Selecione o **Insight sobre vendas da Marketo** função e clique **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   E é isso! Todos os usuários agora terão acesso à seção sales insight na exibição de detalhes do cliente potencial/contato.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Parabéns. Agora você liberou o poder do Marketo Sales Insight.

>[!MORELIKETHIS]
>
>[Configuração de estrelas e chamas para registros de lead/contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
