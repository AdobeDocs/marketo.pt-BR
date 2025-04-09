---
description: Adicionar SSL às suas páginas de aterrissagem - Documentação do Marketo - Documentação do produto
title: Adicionar SSL às suas landing pages
hide: true
hidefromtoc: true
feature: Landing Pages
exl-id: 00ec2d91-3d4f-4671-af9d-9750c1642d40
source-git-commit: 1112af01c08835876f4a2385f304a33e2ddd48ff
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Adicionar SSL às suas landing pages {#add-ssl-to-your-landing-pages}

A criptografia SSL (Secure Socket Layer) permite proteger todas as suas Landing Pages para uma instância do Marketo Engage.

Ao preencher um formulário da Web ou visitar uma landing page hospedada pelo Marketo Engage, por padrão as informações são enviadas por protocolo não seguro (HTTP). De acordo com a política da empresa, talvez você queira proteger as informações enviadas à Marketo no (HTTPS). Por exemplo, quando você visitar `http://info.mydomain.com/`, agora será `https://info.mydomain.com/`.

O Marketo Engage rastreia &quot;Página da Web visitada&quot; e &quot;Clique no link na página da Web&quot; por padrão por protocolo HTTP não seguro. Para ter os links de rastreamento protegidos com seu próprio certificado, o Marketo precisa criar um servidor não compartilhado separado para habilitá-lo. Proteger todos os aspectos da interação de um contato com você normalmente significa proteger tanto as páginas de aterrissagem quanto os links de rastreamento.

CAPTURA DE TELA

## Habilitar certificação SSL {#enable-ssl-certification}

Adicione SSL automaticamente para todos os aliases de domínio criados como parte das regras de página inicial.

1. Vá para a área **Administrador**.

   CAPTURA DE TELA

1. Selecione **Páginas de aterrissagem** na árvore. Na guia **Regras**, clique no menu suspenso **Novo** e selecione **Novo Alias de Domínio**.

   CAPTURA DE TELA

1. Marque a caixa de seleção **Gerar certificado SSL**.

   CAPTURA DE TELA

Isso adiciona automaticamente um certificado SSL a esse domínio.

CAPTURA DE TELA

## Habilitar SSL para o domínio padrão {#enable-ssl-default-domain}

CAPTURA DE TELA

>[!NOTE]
>
>* A coluna Certificado SSL na lista mostra o status de certificado de todos os aliases de domínio criados após o lançamento desse recurso (DATE). Se o SSL estiver habilitado para um domínio por meio do Suporte da Marketo, o certificado continuará a existir, mas não aparecerá na tabela. Essa tabela reflete somente os certificados SSL para domínios adicionados usando as etapas deste artigo.
>
>* Pode levar até três minutos para que o SSL esteja no estado PRONTO. Você deve atualizar a página para que as alterações sejam exibidas.
