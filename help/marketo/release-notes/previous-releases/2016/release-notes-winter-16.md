---
unique-page-id: 10097199
description: Notas de versão - inverno de 16 - Documentos da Marketo - Documentação do produto
title: Notas de versão - inverno de 16
exl-id: 1e3b9207-27fe-47b1-b709-1306ac57b93b
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 6%

---

# Notas de versão: Inverno de 16 {#release-notes-winter}

Os seguintes recursos estão incluídos na versão de inverno de 16. Clique nos links de título para exibir os artigos detalhados de cada recurso.

## [É Filtro Anônimo](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) {#is-anonymous-filter}

O filtro Is Anonymous foi removido para Smart Lists. Consulte a [Perguntas frequentes sobre o rastreamento do Munchkin de próxima geração](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website/next-generation-munchkin-tracking-faq.md) documento para detalhes. Essa alteração não afeta a Personalização da Web (RTP), que continua identificando visitantes anônimos e conhecidos da Web e personalizando o conteúdo em tempo real para esses visitantes.

## [Painel de banco de dados](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md) {#database-dashboard}

O banco de dados de lead tem um painel de resumo atualizado que inclui o tamanho total do banco de dados de pessoas, o número de leads comercializáveis e um detalhamento de leads por cinco principais fontes.

![](assets/image2016-1-12-16-3a18-3a7.png)

## [Navegador Microsoft Edge](/help/marketo/product-docs/administration/setup-administration/supported-browsers.md) {#microsoft-edge-browser}

Adicionamos o Microsoft Edge ao [lista de navegadores](https://docs.marketo.com/display/public/DOCS/Supported+Browsers) suportado pela Marketo.

## [Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) {#microsoft-outlook}

[Microsoft Outlook 2016](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-email-add-in-for-outlook-with-a-registration-code.md) agora é compatível.

## [Programa de e-mail Head Start](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs.md) {#email-program-head-start}

Use Início do cabeçalho para indicar que o processamento do seu envio deve ocorrer com antecedência. Em vez de qualificar leads e preparar emails no horário agendado do programa, o Head Start garante que essas tarefas sejam realizadas antecipadamente. Dessa forma, seu público-alvo começará a receber emails no horário agendado.

![](assets/image2016-1-11-15-3a38-3a3.png)

Para usar esse recurso, o programa de email deve ser agendado com pelo menos 12 horas de antecedência e a Smart List será bloqueada 12 horas antes do envio.

![](assets/image2016-1-11-15-3a35-3a55.png)

>[!NOTE]
>
>Esse recurso será lançado gradualmente por uma semana após a versão de inverno de 16. Não está disponível para uso com campanhas inteligentes ou a API.

## [Melhorias do Mobile Marketing](/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md) {#mobile-marketing-enhancements}

**Suporte para PhoneGap:** Agora oferecemos suporte PhoneGap para seu aplicativo móvel. [Saiba mais](https://developers.marketo.com/documentation/mobile/phonegap-plugin/).

**Suporte para aplicativos de sandbox**:

![](assets/image2016-1-12-10-3a47-3a13.png)

## [API do programa](https://developers.marketo.com/documentation/programs/) {#program-api}

Criar, atualizar e clonar programas por meio da API REST. Isso não inclui a criação ou a atualização de listas inteligentes e campanhas inteligentes em um programa.

## [Melhorias do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md) {#microsoft-dynamics-enhancements}

**[Sincronizar Status](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/sync-status.md)**: Mantenha as guias na taxa de transferência atual e no backlog do processo de sincronização. Detalhe por contagem de inserções e atualizações por objeto.

![](assets/pending-backog-cropped.png)

**[Notificações](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md)**: Receba notificações sobre erros comuns de sincronização, juntamente com uma lista de leads que apresentam esse erro.

![](assets/image2016-1-12-8-3a13-3a9.png)

## [Melhorias de objetos personalizados](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md) {#custom-objects-enhancements}

Agora é possível criar relações muitas para muitas entre Leads/Accounts e um objeto personalizado usando um objeto intermediário com vários campos de link.

![](assets/image2016-1-11-12-3a59-3a59.png)

## [Anúncios de leads do Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md) {#facebook-lead-ads}

[Anúncios de clientes em potencial da facebook](https://www.facebook.com/business/a/lead-ads) são uma maneira mais direta de uma empresa executar campanhas de geração de leads no Facebook. As pessoas preenchem um formulário para expressar interesse em um produto ou serviço, para que a empresa possa acompanhá-los. A integração do Marketo com os Anúncios de leads da Facebook captura automaticamente as informações fornecidas por um cliente potencial no formulário de Anúncio de lead. As ações e notificações de acompanhamento podem ser automatizadas usando o novo acionador Preenchimentos de leads do Facebook .

![](assets/image2016-1-11-10-3a20-3a39.png)

## [Agendador de campanha da Web (Personalização em tempo real)](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/schedule-a-web-campaign.md) {#web-real-time-personalization-campaign-scheduler}

Agende sua campanha antecipadamente. Configure uma data de início e término para o conteúdo personalizado da Web e repita as campanhas em dias e horários específicos. Personalize o agendamento para exibir a campanha de acordo com a hora do visitante da Web ou um fuso horário selecionado.

![](assets/image2016-1-14-8-3a36-3a36.png)
