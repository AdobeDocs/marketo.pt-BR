---
description: Configuração de exibições MSI - Documentos do Marketo - Documentação do produto
title: Configuração de exibições MSI
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Configuração de exibições MSI {#setting-up-msi-views}

Instalar o plug-in Sales Insight no Dynamics adiciona automaticamente as Melhores Melhores Propostas e painéis relacionados no Mapa do Site. Se, por algum motivo, os painéis não forem adicionados, veja a seguir como adicioná-los manualmente.

1. Em Dinâmicas, clique no ícone de engrenagem e selecione **Configurações avançadas** no menu suspenso .

1. No canto superior esquerdo da tela, clique em **Configurações**. Em Personalização, escolha **Personalizações**.

1. Clique em **Personalizar o sistema**.

1. Na árvore à esquerda, clique em **Extensões de cliente** e clique duas vezes **Mapa do site**.

1. Clique na seta para a direita para ir para a próxima página. Em Vendas, você deve ver a Marketo. Caso contrário, certifique-se de ter importado o pacote corretamente.

   >[!NOTE]
   >
   >Em Marketo, você deve ter: Melhores vantagens, Meu email, Atividade da Web e Atividade Anônima da Web. Se algum desses painéis estiver ausente, clique no sinal + acima de Vendas e adicione-o como uma Subárea.

1. Clique em um painel para selecioná-lo. Na coluna à direita, insira as respectivas informações abaixo para cada uma. É possível ignorar qualquer categoria não listada.

   **Melhores Propostas**</br>
URL: MainviewBestbets.html</br>
Ícone: /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID: marketo_bestbets</br>
Título: Melhores Propostas

   **Meu Email**</br>
URL: mkt_/MainViewMyEmail.html</br>
Ícone: /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID: marketo_myemail</br>
Título: Meu Email

   **Atividade da Web**</br>
URL: mkt_/MainViewWebActivity.html</br>
Ícone: /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID: marketo_webactivity</br>
Título: Atividade da Web

   **Atividade Anônima da Web**</br>
URL: mkt_/MainViewWebActivity.html</br>
Ícone: /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID: marketo_anonymous_webactivity</br>
Título: Atividade Anônima da Web

1. Clique em **Salvar** quando concluído.
