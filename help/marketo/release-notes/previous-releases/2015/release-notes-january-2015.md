---
unique-page-id: 4720758
description: Notas de versão - Janeiro de 2015 - Documentação da Marketo - Documentação do produto
title: Notas de versão - Janeiro de 2015
exl-id: f312ff87-6ac1-4167-be98-76600bb4b3cd
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 4%

---

# Notas de versão: Janeiro de 2015 {#release-notes-january}

Os seguintes recursos estão incluídos na versão de janeiro de 2015. Verifique sua Marketo Edition para ver a disponibilidade dos recursos. Após o lançamento, volte para encontrar links para artigos detalhados de cada recurso!

## Atualizações da automação de marketing {#marketing-automation-updates}

**Páginas de aterrissagem para dispositivos móveis**

Agora você pode [criar visualizações móveis para landing pages](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) no editor de landing page. Entregue sua mensagem de maneira eficaz, independentemente do dispositivo, e aumente o engajamento, adaptando seu conteúdo para facilitar o consumo em qualquer lugar. Esse recurso será implantado gradualmente durante a semana seguinte ao lançamento.

[-Vídeo de apresentação da página de aterrissagem-](https://youtu.be/aPQHlG2X6c0)

**Novas chamadas à API Rest**

Três novas chamadas para a API ReST de lead &amp; atividade:

* Excluir lead
* Obter leads por ID de programa
* Obter leads excluídos

Além disso, há uma nova opção para Sincronizar lead, para gravar a alteração de lead de forma assíncrona para uma chamada de API mais rápida. Os detalhes completos estarão disponíveis após o lançamento em [developers.marketo.com](https://developers.marketo.com)

**Suporte a objeto personalizado de script de e-mail**

Agora acesse objetos personalizados associados ao objeto Conta a partir de scripts de email!

## Personalização em tempo real {#real-time-personalization}

**Remarketing personalizado para Google e Facebook**

O remarketing mostra anúncios para pessoas que visitaram seu site. Agora você pode personalizar suas campanhas de remarketing em [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) e [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) uso de dados da personalização em tempo real. Compre para públicos-alvo de diferentes setores, listas de conta nomeadas, tamanhos de empresa ou quaisquer dados de leads conhecidos.

[Módulo de lista de contas nomeado](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

Os aprimoramentos no módulo Contas nomeadas melhorarão as taxas de correspondência e as validações para os usuários. As adições incluem:

* Organizações correspondentes da sua lista Conta nomeada usando o endereço de email do Cliente potencial (também para clientes somente RTP)
* Suporte para até 100 mil registros por conta
* Modelo de arquivo CSV para exibir e baixar

![](assets/image2015-1-14-11-3a12-3a16.png)

**Opções de tag RTP atualizadas**

As opções de Tag RTP em Configurações da conta foram atualizadas para incluir:

1. CDN e assíncrono (tag recomendada)
1. CDN e síncrono (alta velocidade)
1. Tag assíncrona sem CDN
1. Tag síncrona sem CDN

Para melhor desempenho, é recomendável colocar a tag na parte superior do cabeçalho da página da Web após `<head>`. Todas as tags permitem o uso da variável [API RTP](https://developers.marketo.com/documentation/websites/rtp-js-api/). Para obter informações sobre como implantar a Tag RTP, consulte [here](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
