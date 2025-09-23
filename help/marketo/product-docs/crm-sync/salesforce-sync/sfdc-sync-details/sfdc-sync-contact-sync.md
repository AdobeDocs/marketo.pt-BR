---
unique-page-id: 2953457
description: SFDC Sync - Sincronização de contatos - Documentação do Marketo - Documentação do produto
title: SFDC Sync - Sincronização de contatos
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 1%

---

# Sincronização do SFDC: sincronização de contato {#sfdc-sync-contact-sync}

Você sabia que o Marketo sincroniza todo o seu banco de dados com o [!DNL Salesforce]? Ele sincroniza, depois aguarda 5 minutos e depois sincroniza novamente, o dia todo, todos os dias. Estes são alguns detalhes sobre como a Marketo trata especificamente Contatos do [!DNL Salesforce].

## Direção da sincronização {#sync-direction}

A sincronização de contatos é bidirecional. Se você fizer alterações em um contato no [!DNL Salesforce] ou no Marketo, suas atualizações serão refletidas em ambos os sistemas.

## E se forem feitas alterações em ambos os sistemas ao mesmo tempo? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Estamos agradáveis e deixamos [!DNL Salesforce] ganhar. É raro ocorrer esse tipo de colisão de dados.

## Posso converter uma pessoa em um contato no Marketo? {#can-i-convert-a-person-into-a-contact-in-marketo}

Sim, use a ação de fluxo **[Converter pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}**.

>[!CAUTION]
>
>A conversão de uma pessoa no Marketo resultará em uma nova conta e oportunidade em [!DNL Salesforce]. Se não quiser contas duplicadas, use [!DNL Salesforce] para converter.

## Posso forçar manualmente uma sincronização de um contato? {#can-i-manually-force-a-sync-of-a-contact}

Sim, use a ação de fluxo **[Sincronizar Pessoa com o SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** e ela será sincronizada em tempo real.

## Cada campo padrão é sincronizado com o Marketo? {#does-every-single-standard-field-sync-to-marketo}

Não, nem todos os campos padrão são úteis. Todos os campos personalizados podem fazer parte da sincronização.

>[!NOTE]
>
>O Marketo só sincronizará os campos aos quais o usuário do Marketo Sync tem acesso.

## O Marketo respeitará as regras de validação [!DNL Salesforce]? {#will-marketo-respect-the-salesforce-validation-rules}

Sim, se houver um conflito, ele registrará o resultado no Registro de atividades dos clientes potenciais.
