---
description: Visão geral do rastreamento de email - Documentação do Marketo - Documentação do produto
title: Visão geral do rastreamento de email
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Visão geral do rastreamento de email {#email-tracking-overview}

## Como funciona o rastreamento de resposta {#how-reply-tracking-works}

O rastreamento de resposta é feito observando uma ID de mensagem que está em todos os emails enviados. Cada email contém uma ID de mensagem exclusiva que nos permite ter um dos melhores controles de resposta disponíveis.

>[!PREREQUISITES]
>
>Conexão com o Servidor de email: o Sales Connect deve estar conectado à sua caixa de entrada para que saibamos quando uma nova resposta for recebida. Você precisará ter sua conta do Sales Connect conectada ao Gmail. Se você estiver usando o Outlook, precisaremos integrar com seu servidor Exchange.

Se o Sales Connect não puder acompanhar a resposta do seu cliente potencial ao email, ele não poderá interromper uma campanha com base na detecção de resposta ou registrar essa resposta ao Salesforce. O que significa que qualquer endereço de email pode responder?

Isso significa que se você enviar um email para flynn@flynnsarcade.com e ele responder com kevinf@flynnsarcade.com, poderemos rastrear a resposta. Além disso, se você enviar um email para flynn@flynnsarcade.com e CC alan@encom.com, e Alan enviar uma resposta, ele também detectará a resposta e encerrará a campanha.

## Como rastrear anexos de email {#how-to-track-your-email-attachments}

O Sales Connect oferece rastreamento nos seus anexos (.doc, .ppt, .pdf) para que você possa ver quando eles foram abertos/baixados e quais páginas seu destinatário está procurando. Permitiremos que você use nosso recurso de anexos rastreáveis do [aplicativo web](https://toutapp.com/login) e do Gmail (ou aplicativos Google).

>[!NOTE]
>
>O rastreamento de anexos está disponível apenas para os planos de nossa equipe (começando com nosso plano de inicialização g3).

**Como enviar seu primeiro anexo rastreável**

1. Componha um email ou edite um modelo e clique no botão **Conteúdo**.

1. Faça upload do anexo e envie-o. Oferecemos suporte a PDF, documentos do Word e apresentações do PowerPoint.

1. Selecione **Adicionar ao email**.

1. Clique em **Enviar** e acione o Feed Ativo. Você verá seus destinatários à medida que eles abrirem e navegarem pelos anexos.

>[!TIP]
>
>Se você não quiser rastrear um anexo, basta clicar em Anexar arquivos e esse anexo não será rastreado.

## Como funciona o rastreamento de exibição {#how-view-tracking-works}

Rastreamos aberturas de email colocando uma imagem invisível dentro dos emails enviados.

Se alguém responder ao seu email, mas o Sales Connect estiver dizendo que o recurso não foi visualizado, é provável que o recipient não tenha ativado imagens no cliente de email (ou seja, clique na mensagem &quot;clique aqui para baixar imagens&quot; no email).

Algumas dicas para obter melhores estatísticas de rastreamento nos emails:

* Inclua uma imagem em seus emails (como um logotipo) para que o recipient seja incentivado a habilitar imagens para ver sua mensagem.
* Incluir um link como chamada para ação no email.

## Email de teste não exibido como visualizado {#test-email-not-showed-as-viewed}

Mesmo que você tenha enviado sua mensagem para outro endereço de email, você não será registrado visualizando os emails enviados para si mesmo no Feed em tempo real. Nosso rastreamento é baseado em dispositivos; desde que você esteja usando um computador com o qual fez logon no Sales Connect, filtraremos essa atividade.

O motivo? O Sales Connect é inteligente e nossos usuários ativos nunca nos perdoariam se suas próprias informações aparecessem na atividade de Feed ao vivo toda vez que olhassem um email enviado.
