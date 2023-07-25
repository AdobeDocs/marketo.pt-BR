---
unique-page-id: 7513865
description: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2015 - Documentação do Marketo - Documentação do produto
title: Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2015
exl-id: 26c1f02c-c910-445d-8560-0b37961eadcb
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 2%

---

# Instalar e configurar o Marketo Sales Insight no Microsoft Dynamics 2015 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

O Marketo Sales Insight é uma ferramenta fantástica para fornecer à sua equipe de vendas uma &quot;janela&quot; para a riqueza de dados que a equipe de marketing possui. Veja como instalar e configurá-lo no Microsoft Dynamics 201

>[!PREREQUISITES]
>
>Conclua sua integração Marketo-Microsoft.
>
>[Baixar a solução correta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) para a sua versão do Microsoft Dynamics CRM.

## Importar solução {#import-solution}

OK, agora é hora de importar a solução Marketo Sales Insight para o Microsoft Dynamics. Veja como:

1. Em Microsoft Dynamics CRM, clique em **Configurações**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Em CONFIGURAÇÕES, clique em **Personalizações**.

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. Clique em **Soluções**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >É necessário que você já tenha instalado e configurado a solução Marketo antes de prosseguir.

1. Clique em **Importar**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Na nova janela, clique em **Procurar**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Localize e selecione a solução baixada acima.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Clique em **Próxima**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. A solução será carregada. Você pode visualizar o conteúdo do pacote se desejar. Clique em **Próxima**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Certifique-se de deixar a caixa marcada e clique em **Importar**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Você pode baixar o arquivo de log e clicar em **Fechar**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Ótimo! Você deve ver a solução agora. Se não estiver lá, atualize a tela.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Conecte o Marketo e o Sales Insight {#connect-marketo-and-sales-insight}

Vamos vincular sua instância do Marketo ao Sales Insight in Dynamics. Veja como:

>[!NOTE]
>
>É necessário ter direitos de administrador.

1. Faça logon no Marketo e acesse o **Admin** seção.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Na seção Sales Insight, clique em **Editar configuração da API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copie o **Host do Marketo**, **URL da API**, e **ID de usuário da API** para uso em uma etapa posterior. Insira uma chave secreta de API de sua escolha e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) na sua chave secreta da API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Os seguintes campos devem ser sincronizados com o Marketo para *Cliente Potencial e Contato* para que o Sales Insight funcione:
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

Por fim, é necessário conceder a usuários específicos acesso para usar o Marketo Sales Insight.

1. Ir para **Configurações**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Ir para **Segurança**.

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. Clique em **Usuários**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Selecione os usuários aos quais você deseja conceder acesso ao Sales Insight e clique em **Gerenciar Funções**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Selecione a função Marketo Sales Insight e clique em **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E você deveria estar pronto! Por fim, para testar, faça logon no Dynamics como um usuário com acesso ao Marketo Sales Insight e veja um cliente potencial ou contato.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Agora você desbloqueou o potencial do Marketo Sales Insight para sua equipe de vendas.

>[!MORELIKETHIS]
>
>[Configuração de Estrelas e Chamas para Registros de Cliente Potencial/Contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
