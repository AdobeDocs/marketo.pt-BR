---
description: Visão geral do rastreamento de email - Documentos do Marketo - Documentação do produto
title: Visão geral do rastreamento de email
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Visão geral do rastreamento de email {#email-tracking-overview}

## Como o rastreamento de resposta funciona {#how-reply-tracking-works}

O Rastreamento de resposta é feito observando uma ID de mensagem que está em cada email enviado. Cada email contém uma ID de mensagem exclusiva que nos permite ter um dos melhores rastreamentos de resposta.

>[!PREREQUISITES]
>
>Conexão com o Servidor de email: O Sales Connect deve estar conectado à sua caixa de entrada para que saibamos quando uma nova resposta chega. Você precisará ter sua conta do Sales Connect conectada ao Gmail. Se você estiver usando o Outlook, precisaremos fazer a integração com seu servidor do Exchange.

Se o Sales Connect não conseguir rastrear a resposta do seu prospecto ao seu email, ele não poderá parar uma campanha com base na detecção de resposta ou registrar a resposta ao Salesforce. O que queremos dizer com qualquer endereço de email que possa responder?

Isso significa que, se você enviar um email para flynn@flynnsarcade.com e ele responder com kevinf@flynnsarcade.com, poderemos rastrear a resposta. Além disso, se você enviar um email para flynn@flynnsarcade.com e CC alan@encom.com, e Alan escrever de volta, ele também detectará a resposta e encerrará a campanha.

## Como rastrear seus anexos de email {#how-to-track-your-email-attachments}

O Sales Connect oferece rastreamento em seus anexos (.doc, .ppt, .pdf) para que você possa ver quando eles foram abertos/baixados e ver quais páginas o destinatário está visualizando. Permitem usar nosso recurso de anexos rastreáveis de ambos os [aplicação web](https://toutapp.com/login) e Gmail (ou aplicativos Google).

>[!NOTE]
>
>O rastreamento de anexos só está disponível para nossos planos de equipe (começando com nosso plano de inicialização do g3t).

**Como enviar seu primeiro anexo rastreável**

1. Escreva um email ou edite um modelo e clique no botão **Conteúdo** botão.

1. Carregue seu anexo e envie-o. Oferecemos suporte a apresentações do PDF, Word e Powerpoint.

1. Selecionar **Adicionar ao Email**.

1. Clique em **Enviar** e acione seu Feed ao vivo. Você verá seus recipients à medida que eles forem abertos e navegará pelos anexos.

>[!TIP]
>
>Se não quiser rastrear um anexo, clique em Anexar arquivos e esse anexo não será rastreado.

## Como o rastreamento de visualização funciona {#how-view-tracking-works}

Rastreamos aberturas de email ao colocar uma imagem invisível dentro dos emails enviados.

Se alguém responder ao seu email, mas o Sales Connect disser que não foi visualizado, as chances são de que o recipient não tenha ativado imagens em seu cliente de email (ou seja, clique na mensagem &quot;clique aqui para baixar imagens&quot; no email).

Algumas dicas para obter estatísticas de rastreamento melhores em seus emails:

* Inclua uma imagem em seus emails (como um logotipo) para que o recipient seja incentivado a permitir que as imagens vejam sua mensagem.
* Inclua um link como uma chamada para a ação no email.

## Teste de email não exibido como visualizado {#test-email-not-showed-as-viewed}

Mesmo que você tenha enviado sua mensagem para outro endereço de email, não registraremos você visualizando nenhum email enviado para você mesmo no Feed ativo. Nosso rastreamento é baseado em dispositivos; contanto que você esteja usando um computador com o qual fez logon no Sales Connect, nós filtraremos essa atividade.

O motivo? O Sales Connect é inteligente e nossos usuários ativos nunca nos perdoariam se suas próprias informações aparecessem na Atividade do Feed ao vivo toda vez que olhassem para um email enviado.
