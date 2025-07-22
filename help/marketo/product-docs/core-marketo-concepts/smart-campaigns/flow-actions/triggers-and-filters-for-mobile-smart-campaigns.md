---
unique-page-id: 9437991
description: Acionadores e filtros para campanhas inteligentes para dispositivos móveis - Documentação do Marketo - Documentação do produto
title: Acionadores e filtros para campanhas inteligentes para dispositivos móveis
exl-id: 76fc7a74-b27d-4898-a8ca-85c9c2828a28
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '814'
ht-degree: 1%

---

# Acionadores e filtros para campanhas inteligentes para dispositivos móveis {#triggers-and-filters-for-mobile-smart-campaigns}

É possível configurar acionadores e filtros para uma Campanha inteligente para aplicativos móveis.

Para a maioria das atividades, há um acionador, um filtro e um filtro de inatividade. Use filtros de inatividade para rastrear uma ação, como tocar em uma notificação por push, que _não_ ocorreu.

* O Aplicativo Móvel Está/Foi Instalado
* O Aplicativo Móvel Está/Foi Aberto
* Teve/Teve Atividade De Aplicativo Móvel
* Tem/Teve Sessão De Aplicativo Móvel
* Notificação por push de dispositivos móveis tocados/tocados

Há apenas filtros para esta atividade:

* Notificação por push enviada - filtro e filtro de inatividade

Procure por &quot;aplicativo móvel&quot; no painel direito para listar todos os acionadores e filtros do aplicativo móvel.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-1.png)

## Restrições {#constraints}

Use restrições com acionadores e filtros para classificar ainda mais os dados.

![](assets/triggers-and-filters-for-mobile-smart-campaigns-2.png)

Todos os acionadores e filtros, exceto Notificação por push enviada, contêm estas duas restrições padrão:

* Tipo de Dispositivo - [!DNL iPod], iPhone, [!DNL iPhone 6 Plus], [!DNL iPad mini], iPad, smartphone Android, tablet Android, Desconhecido (esta é uma lista predefinida)

* Plataforma - iPhone ou Android

Alguns acionadores e filtros oferecem restrições adicionais, como:

* Versão do aplicativo - uma maneira de direcionar pessoas que não estão na versão mais recente. Por exemplo, se a versão mais recente do aplicativo for 2.0, você poderá usá-la para encontrar pessoas que NÃO estejam na versão 2.0 do aplicativo

* Instalar o Source - Atualmente, a única opção é a API

* Localidade - A configuração no dispositivo

* Aplicativo móvel - O nome do aplicativo específico. Útil para especificar se você tem mais de um

* Versão da plataforma - A versão do SO

* Duração da sessão (segundos) - Tempo da sessão quando o aplicativo está em primeiro plano

* Habilitado para push - **Verdadeiro** significa que as notificações por push podem ser enviadas. **Falso** significa que não pode; por exemplo, a pessoa pode ter optado por não receber notificações por push

## Acionadores e filtros {#triggers-and-filters}

**Tem um aplicativo móvel**

Use este filtro para descobrir todas as pessoas que já tiveram seu aplicativo instalado. Isso está disponível somente como filtro.

>[!NOTE]
>
>O filtro encontrará as instalações atuais e anteriores, pois a Marketo não rastreia as desinstalações do aplicativo.

**Restrições** - Tipo de Dispositivo, Plataforma, Aplicativo Móvel, Versão do Aplicativo Móvel, Tipo de Dispositivo, Instalar Source, É Habilitado para Push e Localidade

![](assets/triggers-and-filters-for-mobile-smart-campaigns-3.png)

>[!TIP]
>
>É uma prática recomendada especificar Tem aplicativo móvel = true e Está habilitado para push = true, bem como o nome do aplicativo móvel ao definir a lista inteligente de quem deve receber uma notificação por push.

O Aplicativo Móvel Está/Foi Instalado

* O aplicativo móvel está instalado - acionador

* O aplicativo móvel foi instalado - filtro

* NÃO foi instalado o aplicativo móvel - filtro de inatividade

**Restrições** - Tipo de Dispositivo, Plataforma, Versão do Aplicativo, Localidade e Instalar Source

![](assets/triggers-and-filters-for-mobile-smart-campaigns-4.png)

O Aplicativo Móvel Está/Foi Aberto

* O aplicativo móvel está aberto - acionador

* O aplicativo móvel foi aberto - filtro

* NÃO foi aberto o aplicativo móvel - filtro de inatividade

**Restrições** - Tipo de Dispositivo e Plataforma

![](assets/triggers-and-filters-for-mobile-smart-campaigns-5.png)

Teve/Teve Atividade De Aplicativo Móvel

Eles fornecem uma maneira avançada de rastrear atividades móveis personalizadas. Você precisará trabalhar com seu desenvolvedor para configurar o rastreamento do [para o Android](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android){target="_blank"} e do [para o iOS](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#install-marketo-sdk-on-ios){target="_blank"}.

* Tem atividade de aplicativo móvel - acionador

* Tinha atividade no aplicativo móvel - filtro

* NÃO teve atividade no aplicativo móvel - filtro de inatividade

**Restrições** - Tipo de Dispositivo, Plataforma, Versão do Aplicativo Móvel, Localidade, Versão da Plataforma, mais cinco adicionais:

* Ação - Atividade móvel personalizada

* Tipo de ação - (opcional) Campo de texto usado para categorizar várias ações

* Detalhes da ação - (opcional) Campo de texto que fornece informações adicionais sobre uma ação

* Métrica de ação - (opcional) Campo numérico que fornece informações adicionais sobre uma ação (por exemplo, preço)

* Duração da ação (segundos) - (opcional) Campo numérico que pode ser usado para capturar quanto tempo um usuário levou para concluir uma ação

As Restrições de ação permitem usar o acionador e os filtros para rastrear a atividade móvel de perto.

>[!NOTE]
>
>**Exemplo**
>
>No tipo de ação de *Compras*, veja uma ação muito específica, com outras restrições definindo-a:
>
>* Comprei uma camisa
>   * Era vermelho
>   * Custou US$ 30
>   * Demorou 20 segundos para comprar

Veja como o filtro é exibido no Marketo:

![](assets/triggers-and-filters-for-mobile-smart-campaigns-6.png)

>[!NOTE]
>
>**Exemplo**
>
>Você pode ter várias ações no mesmo tipo de ação. Na verdade, sua experiência normal de compra pode envolver várias colunas em Compras! Que tal algumas meias para acompanhar isso?
>
>| Tipo de ação | Compras | Compras |
>|---|---|---|
>| Ação | Camiseta comprada | Calças compradas |
>| Detalhes da ação | Cor | Cor |
>| Métrica da ação | Preço | Preço |

**Teve/Teve Sessão De Aplicativo Móvel**

* Tem sessão de aplicativo móvel - acionador

* Sessão de aplicativo móvel prévia - filtro

* NÃO teve sessão de aplicativo móvel - filtro de inatividade

**Restrições** - Tipo de Dispositivo, Plataforma e Duração da Sessão (segundos)

![](assets/triggers-and-filters-for-mobile-smart-campaigns-7.png)

Notificação por push de toques/toques

* Toque em Notificação por push - acionador

* Notificação por push tocada - filtro

* Notificação por push sem toques - filtro de inatividade

**Restrições** - Tipo de Dispositivo, Plataforma, Versão do Aplicativo Móvel, Notificação por Push e Versão da Plataforma

![](assets/triggers-and-filters-for-mobile-smart-campaigns-8.png)

>[!TIP]
>
>Use o filtro de inatividade Notificação por push sem toque para encontrar pessoas que não tocaram em uma notificação por push enviada recentemente a elas, para que você possa fazer o acompanhamento por email.

**Notificação por Push Enviada** Esta atividade está disponível somente como filtro.

* Notificação por push enviada - filtro

* Notificação por push NÃO enviada - filtro de inatividade

**Restrições** - Notificação por push e Aplicativo Móvel

![](assets/triggers-and-filters-for-mobile-smart-campaigns-9.png)

>[!MORELIKETHIS]
>
>* [Adicionar uma Restrição a um Filtro de Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"}
>* [Usar Filtros de Inatividade em uma Smart List](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/use-inactivity-filters-in-a-smart-list.md){target="_blank"}
