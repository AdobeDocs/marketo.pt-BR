---
unique-page-id: 2360354
description: "Adicionar [!DNL Munchkin] Código de rastreamento do seu site - Documentação do Marketo - Documentação do produto"
title: "Adicionar [!DNL Munchkin] Código de rastreamento do seu site"
exl-id: a03a7f11-8d5e-4325-b975-8fc350711da0
feature: Administration, Munchkin Tracking Code
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

# Adicionar [!DNL Munchkin] Código de rastreamento para seu site {#add-munchkin-tracking-code-to-your-website}

O código de rastreamento JavaScript personalizado do Marketo, chamado de [!DNL Munchkin]O rastreia todas as pessoas que visitam seu site para que você possa reagir às visitas com campanhas de marketing automatizadas. Até mesmo visitantes anônimos são rastreados junto com seus endereços IP e outras informações. **Sem esse código de rastreamento, você não poderá rastrear visitas ou outras atividades no seu site**!

>[!PREREQUISITES]
>
>Certifique-se de ter acesso a um desenvolvedor de JavaScript experiente. O Suporte técnico da Marketo não está configurado para ajudar na solução de problemas do JavaScript personalizado.

## Adicionar código de rastreamento ao seu site {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Os usuários do Adobe Experience Cloud também podem usar [Integração do Marketo no Adobe Launch](https://exchange.adobe.com/apps/ec/100223/adobe-launch-core-extension){target="_blank"} para incluir [!DNL Munchkin] em suas páginas da Web. Se você usar o Adobe Launch, _o [!DNL Munchkin] o script é adicionado automaticamente_, portanto, não é necessário adicioná-lo você mesmo.

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/add-munchkin-tracking-code-to-your-website-1.png)

1. Clique em **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-2.png)

1. Selecionar **[!UICONTROL Assíncrono]** para **[!UICONTROL Tipo de código de rastreamento]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-3.png)

   >[!NOTE]
   >
   >Em quase todos os casos, você deve usar o código assíncrono. [Saiba mais](#types-of-munchkin-tracking-codes).

1. Clique em e copie o código de rastreamento do Javascript para colocar em seu site.

   ![](assets/add-munchkin-tracking-code-to-your-website-4.png)

   >[!CAUTION]
   >
   >Não use o código mostrado nesta captura de tela - você deve usar o código exclusivo que aparece em sua conta!

   >[!TIP]
   >
   >Coloque o código de rastreamento nas páginas da Web que deseja rastrear. Pode ser cada página de sites menores ou somente as páginas principais de sites com muitas páginas da Web geradas dinamicamente, fóruns de usuários etc.

   Para obter melhores resultados, use o [!DNL Munchkin] e coloque-o dentro da variável `<head>` elementos de suas páginas. Se estiver usando o código simples (não recomendado), ele será exibido antes da variável `</body>` tag.

   ![](assets/add-munchkin-tracking-code-to-your-website-5.png)

   >[!TIP]
   >
   >Para sites que visualizam um alto volume de tráfego (ou seja, centenas de milhares de visitas por mês), recomendamos que você opte por não rastrear pessoas anônimas. [Saiba mais](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking/){target="_blank"}.

## Adicionar código de rastreamento ao usar vários espaços de trabalho {#add-tracking-code-when-using-multiple-workspaces}

Se estiver usando espaços de trabalho na sua conta do Marketo, provavelmente você também terá presenças da Web separadas que correspondem aos espaços de trabalho. Nesse caso, você pode usar a variável [!DNL Munchkin] Javascript de rastreamento para atribuir suas pessoas anônimas ao espaço de trabalho e partição corretos.

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/add-munchkin-tracking-code-to-your-website-6.png)

1. Clique em **[!UICONTROL Munchkin]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-7.png)

1. Selecione o espaço de trabalho apropriado para as páginas da Web que deseja rastrear.

   ![](assets/add-munchkin-tracking-code-to-your-website-8.png)

   >[!NOTE]
   >
   >Se você não usar o espaço de trabalho especial [!DNL Munchkin] , as pessoas serão atribuídas à partição padrão criada quando sua conta foi configurada. Ele se chama &quot;[!UICONTROL Padrão]&quot; inicialmente, mas você pode ter alterado isso em sua própria conta da Marketo.

1. Selecionar **[!UICONTROL Assíncrono]** para **[!UICONTROL Tipo de código de rastreamento]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-9.png)

1. Clique em e copie o código de rastreamento JavaScript para colocar em seu site.

   ![](assets/add-munchkin-tracking-code-to-your-website-10.png)

   >[!CAUTION]
   >
   >Não use o código mostrado nesta captura de tela - você deve usar o código exclusivo que aparece em sua conta!

1. Coloque o código de rastreamento em suas páginas da Web no `<head>` elemento. As novas pessoas que visitarem esta página serão atribuídas a esta partição.

   ![](assets/add-munchkin-tracking-code-to-your-website-11.png)

   >[!CAUTION]
   >
   >Você só pode usar um [!DNL Munchkin] script de rastreamento para uma única partição e espaço de trabalho em uma página. Não inclua scripts de rastreamento para várias partições/espaços de trabalho em seu site.

   >[!NOTE]
   >
   >As landing pages criadas no Marketo contêm automaticamente um código de rastreamento, portanto, não é necessário colocar esse código nelas.

## Tipos de [!DNL Munchkin] Códigos de rastreamento {#types-of-munchkin-tracking-codes}

Existem três tipos de [!DNL Munchkin] códigos de rastreamento que você pode escolher. Cada uma afeta o tempo de carregamento da página da Web de forma diferente.

1. **[!UICONTROL Simples]**: tem o menor número de linhas de código, mas não otimiza o tempo de carregamento da página da Web. Este código carrega a biblioteca jQuery sempre que uma página da Web é carregada.
1. **[!UICONTROL Assíncrono]**: reduz o tempo de carregamento da página da Web.
1. **[!UICONTROL jQuery assíncrono]**: reduz o tempo de carregamento da página da Web e também melhora o desempenho do sistema. Esse código pressupõe que você já tenha o jQuery e não verifica se deve carregá-lo.

## Teste se seu [!DNL Munchkin] O código está funcionando {#test-if-your-munchkin-code-is-working}

Para verificar se o seu [!DNL Munchkin] o código está funcionando depois de ter sido adicionado:

1. Visite sua página da Web.

1. No seu [!DNL My Marketo], clique no link **[!UICONTROL Analytics]** bloco.

   ![](assets/add-munchkin-tracking-code-to-your-website-12.png)

1. Clique em **[!UICONTROL Atividade da página da Web]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-13.png)

1. Clique em **[!UICONTROL Configuração]** clique duas vezes **[!UICONTROL Origem da atividade]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-14.png)

1. Altere o [!UICONTROL Origem da atividade] para **[!UICONTROL Visitantes anônimos (incluindo ISPs)]** e clique em **[!UICONTROL Aplicar]**.

   ![](assets/add-munchkin-tracking-code-to-your-website-15.png)

1. Clique em **[!UICONTROL Relatório]** guia.

   ![](assets/add-munchkin-tracking-code-to-your-website-16.png)

   >[!NOTE]
   >
   >Se você não visualizar nenhum dado, aguarde alguns minutos e clique no ícone de atualização na parte inferior.
