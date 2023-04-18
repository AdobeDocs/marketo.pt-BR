---
unique-page-id: 9437991
description: Triggers e filtros para campanhas inteligentes de dispositivos móveis - Documentos do Marketo - Documentação do produto
title: Acionadores e filtros para campanhas inteligentes móveis
exl-id: 76fc7a74-b27d-4898-a8ca-85c9c2828a28
source-git-commit: a90f752b291e6d34c920a94795011a8c9efa6d5b
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 1%

---

# Acionadores e filtros para campanhas inteligentes móveis {#triggers-and-filters-for-mobile-smart-campaigns}

Você pode configurar acionadores e filtros para uma campanha inteligente de aplicativo móvel.

Para a maioria das atividades, há um acionador, um filtro e um filtro de inatividade. Use filtros de inatividade para rastrear uma ação, como tocar em uma notificação por push, que *did&#39;t* aconteça.

* O Aplicativo Móvel Está/Foi Instalado
* O Aplicativo Móvel Foi/Foi Aberto
* Possui/teve atividade de aplicativo móvel
* Tem/Teve Sessão de Aplicativo Móvel
* Toque/toque em notificação por push móvel

Há apenas filtros para esta atividade:

* Notificação por push enviada - filtro e filtro de inatividade

Procurar por **aplicativo móvel** no painel direito para listar todos os acionadores e filtros do aplicativo móvel.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-1.png)

## Restrições {#constraints}

Use restrições com acionadores e filtros para classificar ainda mais os dados.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-2.png)

Todos os acionadores e filtros, exceto para Notificação por push de envio, contêm essas duas restrições padrão:

* Tipo de dispositivo - iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, Android smartphone, Android tablet, Desconhecido (esta é uma lista predefinida)

* Plataforma - iPhone ou Android

Alguns acionadores e filtros oferecem restrições adicionais, como:

* Versão do aplicativo - Uma maneira de direcionar pessoas que não estão na versão mais recente. Por exemplo, se a versão mais recente do aplicativo for 2.0, você poderá usá-la para encontrar pessoas que NÃO estão no aplicativo versão 2.0

* Fonte de instalação - Atualmente, a única opção é a API

* Localidade - A configuração no dispositivo

* Aplicativo móvel - O nome do aplicativo específico. Útil para especificar se você tem mais de um

* Versão da plataforma - A versão do sistema operacional

* Duração da sessão (segundos) - Hora da sessão em que o aplicativo está em primeiro plano

* Está habilitado para push - **Verdadeiro** significa que as notificações por push podem ser enviadas. **Falso** significa que não podem; por exemplo, a pessoa pode ter optado por não receber notificações por push

## Triggers e filtros {#triggers-and-filters}

**Tem aplicativo móvel**

Use este filtro para descobrir todas as pessoas que já tiveram seu aplicativo instalado. Isso está disponível somente como filtro.

>[!NOTE]
>
>O filtro encontrará instalações atuais e anteriores, pois o Marketo não rastreia as desinstalações do aplicativo.

**Restrições** - Tipo de dispositivo, plataforma, aplicativo móvel, versão do aplicativo móvel, tipo de dispositivo, fonte de instalação, está habilitado para push e localidade

![](assets/triggers-and-filters-for-mobile-smart-campaigns-3.png)

>[!TIP]
>
>É uma prática recomendada especificar Tem aplicativo móvel = true e É ativado por push = true, bem como o nome do aplicativo móvel ao definir a lista inteligente de quem deve receber uma notificação por push.

O Aplicativo Móvel Está/Foi Instalado

* Aplicativo móvel instalado - acionador

* Aplicativo móvel instalado - filtro

* O aplicativo móvel NÃO foi instalado - filtro de inatividade

**Restrições** - Tipo de dispositivo, plataforma, versão do aplicativo, local e fonte de instalação

![](assets/triggers-and-filters-for-mobile-smart-campaigns-4.png)

O Aplicativo Móvel Foi/Foi Aberto

* Aplicativo móvel aberto - acionador

* Aplicativo móvel aberto - filtro

* NÃO Aplicativo móvel foi aberto - filtro de inatividade

**Restrições** - Tipo de dispositivo e plataforma

![](assets/triggers-and-filters-for-mobile-smart-campaigns-5.png)

Possui/teve atividade de aplicativo móvel

Eles fornecem uma maneira poderosa de rastrear atividades móveis personalizadas. Você precisará trabalhar com o desenvolvedor para configurar o rastreamento [para Android](https://developers.marketo.com/documentation/mobile/installation-instructions-on-android) e [para iOS](https://developers.marketo.com/documentation/mobile/installation-instructions-on-ios).

* Possui atividade de aplicativo móvel - acionador

* Atividade do aplicativo móvel - filtro

* NOT Had Mobile App Activity - filtro de inatividade

**Restrições** - Tipo de dispositivo, plataforma, versão do aplicativo móvel, localidade, versão da plataforma, mais cinco outros:

* Ação - Atividade móvel personalizada

* Tipo de ação - (opcional) Campo de texto usado para categorizar várias ações

* Detalhes da ação - (opcional) Campo de texto que fornece informações adicionais sobre uma ação

* Métrica de ação - (opcional) Campo numérico que fornece informações adicionais sobre uma ação (por exemplo, preço)

* Duração da ação (segundos) - (opcional) Campo numérico que pode ser usado para capturar quanto tempo um usuário levou para concluir uma ação

As restrições de Ação permitem usar o acionador e os filtros para rastrear a atividade móvel de perto.

>[!NOTE]
>
>**Exemplo**
>
>Sob o tipo de ação de *Compras*, aqui está uma ação muito específica, com as outras restrições definindo-a:
>
>* Comprou uma camisa
   >   * Era vermelho
   >   * Custou US$ 30
   >   * Demorou 20 segundos para comprar


Veja como o filtro aparece no Marketo:

![](assets/triggers-and-filters-for-mobile-smart-campaigns-6.png)

>[!NOTE]
>
>**Exemplo**
>
>É possível ter várias ações no mesmo tipo de ação. Na verdade, sua experiência de compra normal pode envolver várias colunas em Compras! Que tal umas meias para ir com isso?
>
>| Tipo de ação | Compras | Compras |
>|---|---|---|
>| Ação | Camiseta comprada | Calças compradas |
>| Detalhes da ação | Cor | Cor |
>| Métrica da ação | Preço | Preço |


**Tem/Teve Sessão de Aplicativo Móvel**

* Possui sessão de aplicativo móvel - acionador

* Sessão de aplicativo móvel - filtro

* NOT Had Mobile App Session - filtro de inatividade

**Restrições** - Tipo de dispositivo, plataforma e duração da sessão (segundos)

![](assets/triggers-and-filters-for-mobile-smart-campaigns-7.png)

Notificações por push com toques/toques

* Toque em Notificação por push - acionador

* Notificação por push com toque - filtro

* NÃO Toque em Notificação por push - Filtro de inatividade

**Restrições** - Tipo de dispositivo, plataforma, versão do aplicativo móvel, notificação por push e versão da plataforma

![](assets/triggers-and-filters-for-mobile-smart-campaigns-8.png)

>[!TIP]
>
>Use o filtro de inatividade Notificação por push não mapeada para encontrar pessoas que não tocaram em uma notificação por push enviada recentemente para elas, para que você possa acompanhar por email.

**Foi Enviada Notificação Por Push** Essa atividade está disponível somente como filtro.

* Notificação por push enviada - filtro

* NÃO Foi Enviado Notificação por push - Filtro de inatividade

**Restrições** - Notificação por push e aplicativo móvel

![](assets/triggers-and-filters-for-mobile-smart-campaigns-9.png)

>[!MORELIKETHIS]
>
>* [Adicionar uma restrição a um filtro de lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)
>* [Usar filtros de inatividade em uma Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

