---
unique-page-id: 3571739
description: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 365 - Marketo Docs - Documentação do produto
title: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 365
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 1%

---

# Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

O Marketo Sales Insight é uma ferramenta fantástica para fornecer à sua equipe de vendas uma &quot;janela&quot; para a riqueza de dados que a equipe de marketing possui. Veja como instalar e configurar.

>[!PREREQUISITES]
>
>Conclua sua integração Marketo-Microsoft.
>
>[Baixe a solução correta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para a sua versão do Microsoft Dynamics CRM.

## Importar solução {#import-solution}

1. Faça logon no [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Clique no menu ![—](assets/image2015-3-16-16-1-13.png) e selecione **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Clique no menu ![—](assets/image2015-5-13-10-5-8.png). Na lista suspensa, selecione **Configurações** e, em seguida, **Soluções**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >Você já deve ter o [instalado e configurado a solução da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) antes de prosseguir.

1. Clique em **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Na nova janela, clique em **Procurar**. Escolha a solução [Marketo Sales Insight baixada na etapa 1](#msi). Clique em **Avançar**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. A solução será carregada. Você pode visualizar o conteúdo do pacote se desejar. Clique em **Avançar**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Certifique-se de deixar a caixa **marcada** e clique em **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sinta-se à vontade para baixar o arquivo de log. Clique em **Fechar**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantástico! Você deve ver a solução agora. Se não estiver lá, atualize a tela.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Clique em **Todas as personalizações do Publish**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Conecte o Marketo e o Sales Insight {#connect-marketo-and-sales-insight}

Vamos vincular sua instância do Marketo ao Sales Insight in Dynamics. Veja como:

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Faça logon no Marketo e vá para a seção **Administrador**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Na seção **Sales Insight**, clique em **Editar configuração de API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie o **Host do Marketo**, a **URL da API** e a **ID de Usuário da API** para usar em uma etapa posterior. Insira uma **Chave secreta de API** de sua escolha e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) na sua chave secreta da API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Os seguintes campos devem ser sincronizados com o Marketo para que _o cliente potencial e o contato_ funcionem:
   >
   > * Prioridade
   > * Urgência
   > * Pontuação relativa
   >
   >Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, execute [este procedimento](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. De volta ao Microsoft Dynamics, clique no ícone ![](assets/image2015-5-13-15-3a49-3a19.png) ao lado de Configurações e selecione **Configuração de API do Marketo** na lista suspensa.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Clique em **Configuração Padrão**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Insira as informações que você copiou do Marketo anteriormente.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Clique no ícone ![](assets/image2015-5-13-16-3a8-3a51.png) no canto inferior direito para salvar as alterações.

## Definir acesso do usuário {#set-user-access}

Você precisa conceder permissões aos usuários para usar o Sales Insight.

1. Clique no menu ![](assets/image2015-5-13-10-3a5-3a8.png). No menu suspenso, selecione **Configurações** e **Segurança**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Clique em **Usuários**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Selecione os usuários aos quais você deseja conceder acesso ao Sales Insight e clique em **Gerenciar funções**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Selecione a função **Marketo Sales Insight** e clique em **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E você deveria estar pronto! Por fim, para testar, faça logon no Dynamics como um usuário com acesso ao Marketo Sales Insight e veja um cliente potencial ou contato.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Agora você desbloqueou o potencial do Marketo Sales Insight para sua equipe de vendas.

>[!MORELIKETHIS]
>
>[Configurando Estrelas e Chamas para Registros de Cliente Potencial/Contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
