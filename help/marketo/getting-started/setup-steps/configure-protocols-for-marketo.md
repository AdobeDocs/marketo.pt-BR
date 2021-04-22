---
unique-page-id: 4720433
description: Configurar protocolos para Marketo - Documentos do Marketo - Documentação do produto
title: Configurar protocolos para Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---

# Configurar protocolos para Marketo {#configure-protocols-for-marketo}

Seu grupo de marketing está usando o Marketo para criar páginas de aterrissagem e emails de campanha de marca. Para garantir que essas landing pages e emails funcionem, eles precisam de uma pequena ajuda da TI. Configure os seguintes protocolos, com as informações que seu grupo de marketing deve ter enviado por email.

Este artigo deve ser compartilhado com o departamento de TI da empresa que deseja implementar esses protocolos.

>[!NOTE]
>
>Se sua equipe de TI restringir o acesso à Web usando uma  lista de permissões, peça para adicionar os seguintes domínios (incluindo o asterisco) para permitir todos os recursos e websockets da Marketo:

* `*.marketo.com`

* `*.marketodesigner.com`

* `*.mktoweb.com`

## Etapa 1: Criar registros DNS para páginas de aterrissagem e email {#step-create-dns-records-for-landing-pages-and-email}

**Rastreamento de CNAMEs de links**

Sua equipe de marketing deve ter enviado duas solicitações para novos registros CNAME. O primeiro é para URLs de página de aterrissagem, de modo que as páginas de aterrissagem sejam exibidas em URLs que reflitam seu domínio e não no Marketo (o host real). O segundo é para os links de rastreamento que estão incluídos nos emails enviados do Marketo.

`1` **Adicionar CNAME para páginas de aterrissagem**

Adicione a página de aterrissagem CNAME que eles enviaram para seu registro DNS, de modo que `[YourLandingPageCNAME]` aponte para a sequência de caracteres de conta exclusiva atribuída às suas páginas de aterrissagem do Marketo. Faça logon no site do registrador de domínios e insira a página de aterrissagem CNAME e a Sequência de caracteres da conta. Normalmente, isso envolve três campos:

* Alias: Digite `[YourLandingPageCNAME]` (fornecido pelo marketing)
* Tipo: CNAME
* Aponte para: Digite `[MarketoAccountString].mktoweb.com` (fornecido pelo marketing)

`2` **Adicionar CNAME para links de rastreamento de email**

Adicione o email de marketing CNAME para que `[YourEmailCNAME]` aponte para [MktoTrackingLink], o link de rastreamento padrão atribuído pela Marketo, no formato:\
`[YourEmailCNAME].[YourDomain].com` NO CNAME  `[MktoTrackingLink]`

Por exemplo:

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **Notificar sua equipe de marketing**

Notifique sua equipe de marketing quando tiver concluído esse processo.

## Etapa 2: lista de permissões os IPs Marketo {#step-allowlist-marketo-ips}

Quando seu grupo de marketing usa o Marketo para enviar emails de teste (uma prática recomendada antes de enviar emails explícitos), os emails de teste às vezes são bloqueados por sistemas antisspam que dependem de endereços IP de remetente para verificar se o email é válido. Para garantir que esses emails de teste cheguem, adicione Marketo à sua lista de permissões.

Adicione esses endereços IP à  de lista de permissões corporativa:

199.15.212.0/22\
192.28.144.0/20
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

Alguns sistemas antisspam usam o campo Return-Path de email em vez do endereço IP para permitir. Nesses casos, a melhor abordagem é lista de permissões &quot;*.mktomail.com&quot;, pois o Marketo usa vários subdomínios de caixa de correio. Outros sistemas antisspam lista de permissões com base no endereço De. Nessas situações, certifique-se de incluir todos os domínios de envio (&quot;De&quot;) que seu grupo de marketing usa para se comunicar com pessoas/leads.

>[!NOTE]
>
>A Postini emprega uma tecnologia exclusiva e requer intervalos IP de  incluir na lista de permissões. Consulte [Inclua na lista de permissões com Postini](https://nation.marketo.com/docs/DOC-1066).

## Etapa 3: Configurar SPF e DKIM {#step-set-up-spf-and-dkim}

Sua equipe de marketing também deve ter enviado informações do DKIM para adicioná-las ao registro de recursos do DNS (também listado abaixo). Siga as etapas para configurar o DKIM e o SPF com sucesso e, em seguida, notifique sua equipe de marketing de que isso foi atualizado.

1. Para configurar o SPF, adicione a seguinte linha às entradas de DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   incluem: mktomail.com ~all

   Se já houver um registro SPF existente em nossa entrada DNS, basta adicionar o seguinte a ele:\
   incluem: mktomail.com

   Substitua CompanyDomain pelo domínio principal de seu site (por exemplo: &quot;`(company.com/)`&quot;) e CorpIP com o endereço IP do seu servidor de email corporativo (por exemplo, &quot;255.255.255.255&quot;). Caso envie emails de vários domínios por meio do Marketo, sua equipe de TI deve adicionar essa linha para cada domínio (em uma linha).

1. Para DKIM, crie Registros de Recursos de DNS para cada domínio que gostaríamos de configurar. Abaixo estão os Registros de host e os Valores TXT para cada domínio que iremos assinar:

   `[DKIMDomain1]`: O registro do host é  `[HostRecord1]` e o valor TXT é  `[TXTValue1]`.

   `[DKIMDomain2]`: O registro do host é  `[HostRecord2]` e o valor TXT é  `[TXTValue2]`.

   Copie o HostRecord e o TXTValue para cada DKIMDomain que você configurou depois de seguir as [instruções aqui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). Não se esqueça de verificar cada domínio em Admin > Email > DKIM depois que sua equipe de TI concluir esta etapa.

## Etapa 4: Configurar registros MX para seu domínio {#step-set-up-mx-records-for-your-domain}

Um registro MX permite receber emails para o domínio do qual você está enviando emails para processar respostas e respondedores automáticos. Se você estiver enviando do seu domínio corporativo, provavelmente já terá isso configurado. Caso contrário, você geralmente pode configurá-lo para mapear para o registro MX do domínio corporativo.
