---
unique-page-id: 3571838
description: Microsoft Dynamics Sync - Sincronização de campo - Documentos do Marketing - Documentação do produto
title: Microsoft Dynamics Sync - Sincronização de campo
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronização de campo {#microsoft-dynamics-sync-field-sync}

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

A sincronização de marketing com o Dynamics é super poderosa. Aqui estão os detalhes.

## Como os detalhes de campo são mantidos em sincronia entre os dois sistemas? {#how-are-field-details-kept-in-sync-between-the-two-systems}

A sincronização é bidirecional para entidades de lead e contato. Se você fizer alterações em um cliente potencial ou contato no Dynamics ou em uma pessoa no Marketing Cloud, suas atualizações serão refletidas em ambos os sistemas.

Para entidades de conta, usuário, oportunidade, equipe e personalizadas, a sincronização é unidirecional: Dinâmica para o Marketo. Se você fizer alterações nessas entidades no Dynamics, suas atualizações serão refletidas no Marketo.

## E se forem feitas alterações no mesmo campo em ambos os sistemas ao mesmo tempo? (Colisão de dados) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Embora seja raro, o Marketo ganhará por pessoas (clientes potenciais) e o Dynamics ganhará por contatos. Isso porque consideramos o departamento de marketing autoritativo para as pessoas, enquanto o sistema oficial de registro de contatos está no departamento de vendas (CRM). Para entidades de sincronização unidirecionais, o Dynamics sempre ganhará.

## É possível criar um campo no Dynamics usando o Marketo? {#can-i-create-a-field-in-dynamics-using-marketo}

Não, isso não é suportado no momento.

## Criei um campo no Dynamics. Posso sincronizá-lo com o Marketo? {#i-created-a-field-in-dynamics-can-i-sync-it-to-marketo}

Sim, você pode [sincronizar o campo](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) desde que o usuário de sincronização tenha acesso a ele no Dynamics.

Quais campos serão sincronizados com o Marketo?

É possível [selecionar campos para sincronização](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) durante a configuração.

## E se eu precisar adicionar um campo personalizado após a sincronização do Marketo e do Dynamics? {#what-if-i-need-to-add-a-custom-field-after-marketo-and-dynamics-are-synced}

É possível adicionar campos a qualquer momento e esperar que os dados sejam atualizados do Dynamics para o Marketing. Consulte [Usar sincronização rápida com o Microsoft Dynamics para obter um novo campo](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md) personalizado para obter detalhes.

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Usar sincronização rápida com o Microsoft Dynamics para um novo campo personalizado](microsoft-dynamics-sync-field-sync/use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field.md)

>



