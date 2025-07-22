---
description: Visão geral do rastreamento de email - Documentação do Marketo - Documentação do produto
title: Visão geral do rastreamento de email
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Visão geral do rastreamento de email {#email-tracking-overview}

## Como funciona o rastreamento de resposta {#how-reply-tracking-works}

O rastreamento de resposta é feito observando uma ID de mensagem que está em todos os emails enviados. Cada email contém uma ID de mensagem exclusiva que nos permite ter um dos melhores controles de resposta disponíveis.

>[!PREREQUISITES]
>
>Conexão com o Servidor de Email: o [!DNL Sales Connect] deve estar conectado à sua caixa de entrada para que saibamos quando uma nova resposta será recebida. Você precisará ter sua conta [!DNL Sales Connect] conectada ao Gmail. Se você estiver usando o Outlook, precisaremos integrar com seu servidor Exchange.

Se [!DNL Sales Connect] não puder acompanhar a resposta do seu cliente potencial ao email, ele não poderá interromper uma campanha com base na detecção de resposta ou registrar essa resposta à Salesforce. O que significa que qualquer endereço de email pode responder?

Isso significa que se você enviar um email para flynn@flynnsarcade.com e ele responder com kevinf@flynnsarcade.com, poderemos rastrear a resposta. Além disso, se você enviar um email para flynn@flynnsarcade.com e CC alan@encom.com, e Alan enviar uma resposta, ele também detectará a resposta e encerrará a campanha.

## Como rastrear anexos de email {#how-to-track-your-email-attachments}

O [!DNL Sales Connect] oferece o rastreamento dos seus anexos (.doc, .ppt, .pdf) para que você possa ver quando eles foram abertos/baixados e quais páginas o destinatário está procurando. Permitiremos que você use nosso recurso de anexos rastreáveis do [aplicativo web](https://toutapp.com/login) e do Gmail (ou aplicativos Google).

>[!NOTE]
>
>O rastreamento de anexos está disponível apenas para os planos de nossa equipe (começando com nosso plano de inicialização g3).

**Como enviar seu primeiro anexo rastreável**

1. Componha um email ou edite um modelo e clique no botão **[!UICONTROL Conteúdo]**.

1. Faça upload do anexo e envie-o. Oferecemos suporte a PDFs, [!DNL Word] documentos e [!DNL Powerpoint] apresentações.

1. Selecione **[!UICONTROL Adicionar ao email]**.

1. Clique em **[!UICONTROL Enviar]** e acione o Feed Ativo. Você verá seus destinatários à medida que eles abrirem e navegarem pelos anexos.

>[!TIP]
>
>Se você não quiser rastrear um anexo, basta clicar em Anexar arquivos e esse anexo não será rastreado.

## Como funciona o rastreamento de exibição {#how-view-tracking-works}

Rastreamos aberturas de email colocando uma imagem invisível dentro dos emails enviados.

Se alguém responder ao seu email, mas [!DNL Sales Connect] estiver dizendo que ele não foi visualizado, provavelmente o destinatário não habilitou imagens no cliente de email (ou seja, clique na mensagem &quot;clique aqui para baixar imagens&quot; no email).

Algumas dicas para obter melhores estatísticas de rastreamento nos emails:

* Inclua uma imagem em seus emails (como um logotipo) para que o recipient seja incentivado a habilitar imagens para ver sua mensagem.
* Incluir um link como call to action no email.

## Email de teste não exibido como visualizado {#test-email-not-showed-as-viewed}

Mesmo que você tenha enviado sua mensagem para outro endereço de email, você não será registrado visualizando os emails enviados para si mesmo no Feed em tempo real. Nosso rastreamento é baseado em dispositivos; desde que você esteja usando um computador com o qual fez logon [!DNL Sales Connect], vamos filtrar essa atividade.

O motivo? [!DNL Sales Connect] é inteligente, e nossos usuários ativos nunca nos perdoariam se suas próprias informações aparecessem na Atividade de Feed ao vivo toda vez que olhassem um email que enviavam.
