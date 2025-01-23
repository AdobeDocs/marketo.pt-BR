---
description: Torne uma campanha de marketing visível nas ações do Sales Insight - Documentação do Marketo - Documentação do produto
title: Tornar uma campanha de marketing visível nas ações de insights de vendas
exl-id: 223baca3-159e-4f0d-b26f-f4c924a39fc3
feature: Sales Insight Actions
source-git-commit: 696353c74fd14fe72699fb53a87cfed5e9c42d51
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Tornar uma campanha de marketing visível nas ações de insights de vendas {#make-a-marketing-campaign-visible-in-sales-insight-actions}

As campanhas só podem ser compartilhadas se estiverem visíveis.

Com as Ações de insights de vendas, os usuários terão acesso a um novo aplicativo de vendas chamado toutapp.com. Este aplicativo oferece a eles um novo conjunto de recursos de ação, mas também herda o recurso _Adicionar à Campanha de Marketing_, disponível na versão principal do Sales Insights. Isso é importante ter em mente, pois dependendo de onde você deseja que os usuários acessem o recurso Adicionar à campanha de marketing (toutapp.com ou a experiência do pacote MSI SFDC ), suas campanhas do Marketo precisarão ser configuradas de forma diferente. Consulte a nota na Etapa 4 para saber mais.

1. Selecione (ou crie) a Campanha que deseja compartilhar.

   ![](assets/make-a-marketing-campaign-visible-sia-1.png)

1. Clique na guia **Smart List**.

   ![](assets/make-a-marketing-campaign-visible-sia-2.png)

1. Adicione o acionador _Campanha solicitada_.

   ![](assets/make-a-marketing-campaign-visible-sia-3.png)

1. Para origem, escolha &quot;is&quot; **API de Serviço da Web**.

   ![](assets/make-a-marketing-campaign-visible-sia-4.png)

   >[!NOTE]
   >
   >Se você quiser mostrar a campanha de marketing para usuários que estão utilizando _Adicionar à Campanha de Marketing_ a partir do aplicativo Web toutapp.com (isso também inclui se você tiver o aplicativo Web incorporado ao CRM por meio do objeto Caixa de Saída de Vendas do Marketo), defina-o como &quot;API de Serviço da Web&quot;. Se desejar que a campanha de marketing seja exibida quando um usuário usar as ações no painel MSI no Salesforce nos botões de lead, contato, página da conta ou ação em massa nas exibições de lead e lista de contatos, atualize-a para &quot;Sales Insight&quot;

1. Clique na guia **Fluxo**.

   ![](assets/make-a-marketing-campaign-visible-sia-5.png)

1. Adicione a ação de fluxo _Momento interessante_.

   ![](assets/make-a-marketing-campaign-visible-sia-6.png)

1. Para Tipo, selecione **Web**.

   ![](assets/make-a-marketing-campaign-visible-sia-7.png)

1. Na caixa _Descrição_, escreva uma mensagem para a equipe de vendas. Neste exemplo, estamos usando tokens para especificar o formulário que foi preenchido.

   ![](assets/make-a-marketing-campaign-visible-sia-8.png)

1. Clique na guia **Agendar** e **Ativar** a campanha.

   ![](assets/make-a-marketing-campaign-visible-sia-9.png)
