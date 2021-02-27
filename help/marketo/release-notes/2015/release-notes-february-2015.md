---
unique-page-id: 6094890
description: Notas de versão - fevereiro de 2015 - Documentos do Marketo - Documentação do produto
title: Notas de versão - fevereiro de 2015
translation-type: tm+mt
source-git-commit: 029d8b419ba5078980b4fde9890bdb35194bf264
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Notas de versão: Fevereiro de 2015 {#release-notes-february}

Os seguintes recursos foram incluídos na versão de fevereiro de 2015. Verifique a disponibilidade de recursos do Marketing Edition. Após o lançamento, volte a encontrar links para artigos detalhados para cada recurso. Rolo de tambor...

## Aprimoramentos da Marketing Automation {#marketing-automation-enhancements}

**[Mover Campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Alegre-se! Agora você pode mover campanhas inteligentes para dentro e para fora de programas usando o recurso arrastar e soltar ou o recurso Mover na árvore.

**[Dynamics 2015 (Online)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)**  - compatível!

**Alterações no certificado HTTPS**

Para proteger a confidencialidade e a integridade dos dados do cliente e dos serviços SaaS, o Marketo segue as práticas recomendadas do setor SaaS

e substituirá os protocolos de segurança usados no momento (SHA-1 e SSL) por versões mais seguras (SHA-2 (também conhecido como SHA-256) e TLS) para os seguintes domínios:

* [marketo.net](https://marketo.net) (tráfego Munchkin criptografado)

* [marketo.com](https://marketo.com) (principais aplicativos SaaS)

Isso acontecerá pouco depois desta versão. O protocolo SHA-1 será temporariamente suportado no domínio [mktoapi.com](https://mktoapi.com) até dezembro de 2015 para permitir que os proprietários de sistemas e aplicativos herdados atualizem seus sistemas com compatibilidade com SHA-2.

**Munchkin seguro**

Estamos removendo nosso suporte para SSL3. Mantivemos o SSL3 até agora para manter o suporte a navegadores da Web antigos, mas em 2015 não estamos mais vendo tráfego significativo da Web desses navegadores. Isso só afetaria Munchkin quando usado em páginas seguras, e será lançado lentamente após o lançamento de fevereiro.

## Aprimoramentos de personalização em tempo real {#real-time-personalization-enhancements}

**[URL do público alvo para Campanha](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Selecione as páginas que deseja que sua campanha em tempo real seja exibida usando &#39;Adicionar um URL de Público alvo&#39;. Esse recurso funciona com todos os tipos de campanha (Diálogo, Em zona, Widgets), mas é especialmente valioso para campanhas na zona, onde uma campanha será renderizada na ID da zona somente para o URL do público alvo selecionado. Ele oferece suporte à adição de vários URLs a públicos alvos de páginas da Web diferentes.

![](assets/image2015-2-19-11-3a0-3a30.png)

**País e estado adicionados à definição de metas baseada em conta**

O país e o estado podem ser adicionados às Listas de conta nomeada. Prospectos de conta da chave do público alvo de locais específicos.
