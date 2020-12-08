---
unique-page-id: 4720758
description: Notas de versão - janeiro de 2015 - Documentos do Marketo - Documentação do produto
title: Notas de versão - janeiro de 2015
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Notas de versão: Janeiro de 2015 {#release-notes-january}

Os seguintes recursos estão incluídos na versão de janeiro de 2015. Verifique a disponibilidade de recursos do Marketing Edition. Após o lançamento, volte a encontrar links para artigos detalhados para cada recurso!

## Atualizações da automação de marketing {#marketing-automation-updates}

**Novas fotos de Rick DeCosta!**

Rick é um cliente do Marketo do SmartBear e tem uma coleção [inacreditável de fotos](https://www.flickr.com/photos/rickdecosta). Dê uma olhada!

## Landings page amigáveis para dispositivos móveis {#mobile-friendly-landing-pages}

Agora você pode [criar visualizações móveis para landing page](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/add-a-mobile-view-for-your-free-form-landing-page.md) no editor de landings page. Forneça sua mensagem de forma eficiente, independentemente do dispositivo, e aumente o envolvimento, adaptando seu conteúdo para fácil consumo em qualquer lugar. Esse recurso será lançado gradualmente durante a semana seguinte ao lançamento.

`<iframe width="420" height="315" src="//www.youtube-nocookie.com/embed/aPQHlG2X6c0" frameborder="0" allowfullscreen></iframe>`

**Novas chamadas da API ReST**

Três novas chamadas para a API ReST de cliente potencial e Atividade:

* Excluir cliente potencial
* Obter clientes em potencial por ID de Programa
* Obter Clientes Potenciais Excluídos

Além disso, há uma nova opção para Sincronizar cliente potencial, para gravar a mudança de cliente potencial de forma assíncrona para uma chamada de API mais rápida. Os detalhes completos estarão disponíveis após o lançamento em [developers.marketo.com](http://developers.marketo.com)

**Suporte a objetos personalizados de script de email**

Agora, acesse objetos personalizados associados ao objeto Conta a partir de scripts de e-mail!

## Personalização em tempo real {#real-time-personalization}

**Comentários personalizados para Google e Facebook**

O remarketing mostra anúncios às pessoas que visitaram seu site. Agora você pode personalizar suas campanhas de remarketing no [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md) e [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md) usando dados da Personalização em tempo real. Compartilhe para audiências de diferentes setores, listas de conta nomeadas, tamanhos de empresa ou quaisquer dados de clientes potenciais conhecidos.

[Módulo de Lista de conta nomeado](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-new-account-list.md)

As melhorias no módulo Contas nomeadas melhorarão as taxas de correspondência e as validações para os usuários. As adições incluem:

* Correspondência de organizações da sua lista Conta Nomeada usando o endereço de email do Cliente Potencial (também para clientes somente RTP)
* Suporte para até 100 mil registros por conta
* Modelo de arquivo CSV para visualização e download

![](assets/image2015-1-14-11-3a12-3a16.png)

Opções de tag RTP atualizadas

[As opções de etiqueta](http://docs.marketo.com/display/docs/rtp+tag+implementation) RTP em Configurações da conta foram atualizadas para incluir:

1. CDN e assíncrono (tag recomendada)
1. CDN e síncrono (alta velocidade)
1. Tag assíncrona sem CDN
1. Tag síncrona sem CDN

Para obter o melhor desempenho, é recomendável colocar a tag na parte superior do cabeçalho na sua página da Web após `<head>`. Todas as tags permitem o uso da API [](http://developers.marketo.com/documentation/websites/rtp-js-api/)RTP. Para obter informações sobre como implantar a tag RTP, consulte [aqui](/help/marketo/product-docs/web-personalization/rtp-tag-implementation/deploy-the-rtp-javascript.md).

![](assets/image2015-1-15-13-3a30-3a45.png)
