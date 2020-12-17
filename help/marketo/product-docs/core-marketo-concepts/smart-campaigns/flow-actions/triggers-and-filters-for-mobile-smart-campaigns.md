---
unique-page-id: 9437991
description: Acionadores e Filtros para Campanhas inteligentes móveis - Documentos do Marketing - Documentação do produto
title: Acionadores e Filtros para Campanhas inteligentes móveis
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---


# Acionadores e Filtros para Campanhas inteligentes móveis {#triggers-and-filters-for-mobile-smart-campaigns}

Você pode configurar acionadores e filtros para uma campanha inteligente do aplicativo móvel.

Para a maioria das atividades, há um acionador, um filtro e um filtro de inatividade. Use filtros de inatividade para rastrear uma ação, como tocar em uma notificação por push, que *não* ocorreu.

* O aplicativo móvel está/foi instalado
* O aplicativo móvel é/foi aberto
* Tem/Teve Atividade de aplicativo móvel
* Tem/Teve Sessão de Aplicativo Móvel
* Notificação por push móvel tocada/tocada

Há apenas filtros para esta atividade:

* Notificação por push enviada - filtro e filtro de inatividade

Procure **aplicativo móvel** no painel direito para lista de todos os filtros e acionadores do aplicativo móvel.

![](assets/image2015-8-12-17-3a25-3a18.png)

## Restrições {#constraints}

Use restrições com acionadores e filtros para classificar ainda mais os dados.

![](assets/image2015-8-17-12-3a6-3a33.png)

Todos os acionadores e filtros, exceto para Notificação por push enviada, contêm estas duas restrições padrão:

* Tipo de dispositivo - iPod, iPhone, iPhone 6 Plus, iPad mini, iPad, Android smartphone, Android tablet, Unknown (esta é uma lista predefinida)

* Plataforma - iPhone ou Android

Alguns acionadores e filtros oferta restrições adicionais, como:

* Versão do aplicativo - uma forma de público alvo para pessoas que não estão na versão mais recente. Por exemplo, se a versão mais recente do aplicativo for 2.0, você pode usá-la para encontrar pessoas que NÃO estão no App versão 2.0

* Fonte de instalação - Atualmente, a única opção é a API

* Localidade - A configuração no dispositivo

* Aplicativo móvel - o nome do aplicativo específico. Útil para especificar se você tem mais de um

* Versão da plataforma - A versão do SO

* Duração da sessão (segundos) - Tempo da sessão quando o aplicativo está em primeiro plano

* Está ativado para push - **Verdadeiro** significa que notificações por push podem ser enviadas. **Os** Falsemeanos que não podem; por exemplo, a pessoa pode ter opt out de receber notificações por push

## Acionadores e Filtros {#triggers-and-filters}

**Possui aplicativo móvel**

Use este filtro para descobrir todas as pessoas que já tiveram seu aplicativo instalado. Isso está disponível somente como filtro.

>[!NOTE]
>
>O filtro encontrará instalações atuais e anteriores, pois o Marketo não rastreia as desinstalações do aplicativo.

**Restrições**: Tipo de dispositivo, Plataforma, Aplicativo móvel, Versão do aplicativo móvel, Tipo de dispositivo, Fonte de instalação, Está habilitado para push e Localidade

![](assets/image2015-8-21-13-3a33-3a54.png)

>[!TIP]
>
>É uma prática recomendada especificar Has Mobile App = true e Is Push Enabled = true, bem como o nome do aplicativo móvel ao definir a lista inteligente de quem deve receber uma notificação por push.

O aplicativo móvel está/foi instalado

* Aplicativo móvel instalado - acionador

* Aplicativo móvel instalado - filtro

* NÃO Aplicativo móvel instalado - filtro de inatividade

**Restrições**: Tipo de dispositivo, Plataforma, Versão do aplicativo, Local e Origem da instalação

![](assets/image2015-8-17-13-3a11-3a3.png)

O aplicativo móvel é/foi aberto

* Aplicativo móvel aberto - acionador

* Aplicativo móvel aberto - filtro

* O aplicativo NÃO móvel foi aberto - filtro de inatividade

**Restrições**: Tipo de dispositivo e plataforma

![](assets/image2015-8-17-13-3a13-3a55.png)

Tem/Teve Atividade de aplicativo móvel

Eles fornecem uma maneira poderosa de rastrear a atividade móvel personalizada. Você precisará trabalhar com seu desenvolvedor para configurar o rastreamento [para Android](http://developers.marketo.com/documentation/mobile/installation-instructions-on-android) e [para iOS](http://developers.marketo.com/documentation/mobile/installation-instructions-on-ios).

* Tem Atividade de aplicativo móvel - acionador

* Atividade do aplicativo móvel - filtro

* NÃO TINHA Atividade de aplicativo móvel - filtro de inatividade

**Restrições**: Tipo de dispositivo e plataforma, mais cinco outros:

* Ação - atividade móvel personalizada

* Tipo de ação - (opcional) Campo de texto usado para categorizar várias ações

* Detalhes da ação - (opcional) campo de texto que fornece informações adicionais sobre uma ação

* Métrica de ação - (opcional) Campo numérico que fornece informações adicionais sobre uma ação (por exemplo, preço)

* Duração da ação (segundos) - (opcional) Campo numérico que pode ser usado para capturar quanto tempo um usuário levou para concluir uma ação

As restrições de Ação permitem que você use o acionador e os filtros para acompanhar muito atentamente a atividade móvel.

>[!NOTE]
>
>**Exemplo**
>
>Sob o tipo de ação de *Shopping*, há uma ação muito específica, com as outras restrições que a definem:
>
>* Comprou uma camisa
>  * Era vermelho
>  * Custou US$ 30
>  * Demorou 20 segundos para comprar


Veja a aparência do filtro no Marketo:   ![](assets/image2015-8-17-13-3a16-3a12.png)

>[!NOTE]
>
>**Exemplo**
>
>É possível ter várias ações no mesmo tipo de ação. Na verdade, sua experiência de compras normal pode envolver várias colunas em Compras! Que tal umas meias para ir com isso?
>
>| Tipo de ação | Compras | Compras |
>|---|---|---|
>| Ação | Camisa comprada | Calças compradas |
>| Detalhes da ação | Cor | Cor |
>| Métrica de ação | Preço | Preço |


**Tem/Teve Sessão de Aplicativo Móvel**

* Tem sessão de aplicativo móvel - acionador

* Sessão de aplicativo móvel - filtro

* NOT Had Mobile App Session - filtro de inatividade

**Restrições**: Tipo de dispositivo, plataforma e duração da sessão (segundos)

![](assets/image2015-8-17-13-3a18-3a34.png)

Notificação por push com toques/toques

* Toque em Notificação por push - acionador

* Notificação por push com toque - filtro

* Notificação por push NÃO tocada - filtro de inatividade

**Restrições**: Tipo de dispositivo, Plataforma, Versão do aplicativo móvel, Notificação por push e Versão da plataforma

![](assets/image2015-8-21-14-3a2-3a24.png)

>[!TIP]
>
>Use o filtro de inatividade Notificação por push sem toque para encontrar pessoas que não tocaram em uma notificação por push enviada recentemente para elas, para que você possa acompanhar por email.

**Foi enviada a** notificação por pushEssa atividade está disponível somente como filtro.

* Notificação por push enviada - filtro

* NÃO Enviado Notificação por push - filtro de inatividade

**Restrições**: Notificação por push e aplicativo móvel

![](assets/image2015-8-21-14-3a3-3a50.png)

>[!MORELIKETHIS]
>
>* [Adicionar uma restrição a um filtro de Lista inteligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md)
>* [Usar Filtros de inatividade em uma Lista inteligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md)

