---
description: Configuração de visualizações do MSI - Documentação do Marketo - Documentação do produto
title: Configuração de exibições do MSI
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 4%

---

# Configuração de exibições do MSI {#setting-up-msi-views}

Instalar o plug-in [!DNL Sales Insight] no Dynamics adiciona automaticamente o [!DNL Best Bets] e os painéis relacionados no Mapa do Site. Se, por algum motivo, os painéis não forem adicionados, veja como adicioná-los manualmente.

1. No Dynamics, clique no ícone de engrenagem e selecione **[!UICONTROL Configurações avançadas]** no menu suspenso.

1. No canto superior esquerdo da tela, clique em **[!UICONTROL Configurações]**. Em Personalização, escolha **[!UICONTROL Personalizações]**.

1. Clique em **[!UICONTROL Personalizar o sistema]**.

1. Na árvore à esquerda, clique em **[!UICONTROL Extensões de Cliente]** e clique duas vezes em **[!UICONTROL Mapa de Sites]**.

1. Clique na seta direita para ir para a próxima página. Em Vendas, você deve ver Marketo. Caso contrário, certifique-se de ter importado o pacote corretamente.

   >[!NOTE]
   >
   >No Marketo, você deve ter: Melhores opções, Meu email, Atividade da Web e Atividade anônima da Web. Se algum desses painéis estiver ausente, clique no sinal + acima de Vendas e adicione-os como uma Subárea.

1. Clique em um painel para selecioná-lo. Na coluna à direita, insira as respectivas informações abaixo para cada uma. Você pode ignorar quaisquer categorias não listadas.

   **Melhores Opções**</br>
URL: MainviewBestbets.html</br>
Ícone: /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID: marketo_bestbets</br>
Título: Melhores Opções

   **Meu Email**</br>
URL: mkt_/MainViewMyEmail.html</br>
Ícone: /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID: marketo_myemail</br>
Título: Meu email

   **Atividade da Web**</br>
URL: mkt_/MainViewWebActivity.html</br>
Ícone: /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID: marketo_webactivity</br>
Título: Atividade da Web

   **Atividade da Web Anônima**</br>
URL: mkt_/MainViewWebActivity.html</br>
Ícone: /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID: marketo_anonymous_webactivity</br>
Title: Atividade Anônima Na Web

1. Clique em **[!UICONTROL Salvar]** quando terminar.
