---
unique-page-id: 4720433
description: Configurar protocolos para o Marketing - Documentos do Marketing - Documentação do produto
title: Configurar protocolos para o Marketing
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 1%

---


# Configurar protocolos para o Marketing {#configure-protocols-for-marketo}

Seu grupo de marketing está usando o Marketo para criar landings page de campanha com marca e e-mails. Para garantir que essas landings page e emails funcionem, eles precisam de uma pequena ajuda da TI. Configure os seguintes protocolos, com as informações que seu grupo de marketing deve ter enviado por email.

>[!NOTE]
>
>Este artigo específico deve ser exibido pelo departamento de TI da empresa que deseja implementar esses protocolos.

## Etapa 1: Criar registros DNS para Landing page e e-mail {#step-create-dns-records-for-landing-pages-and-email}

**Rastreamento de CNAMEs de links**

Sua equipe de marketing deve ter enviado duas solicitações para novos registros CNAME. A primeira é para URLs de landing page, de modo que as landings page sejam exibidas em URLs que reflitam seu domínio e não em Marketo (o host real). O segundo é para os links de rastreamento que estão incluídos nos emails enviados do Marketo.

1 - **Adicionar CNAME para Landing page**

Adicione o CNAME da landing page que eles enviaram para seu registro DNS, de modo que `[YourLandingPageCNAME]` aponte para a sequência exclusiva de caracteres da conta atribuída às landings page de marketing. Faça logon no site do registrador de domínio e digite a landing page CNAME e a Sequência de caracteres da conta. Normalmente, isso envolve três campos:

・ Outros nomes: Digite `[YourLandingPageCNAME]` (fornecido pelo marketing) ・ Tipo: CNAME\
・ Aponte para: Enter `[MarketoAccountString].mktoweb.com` (fornecido pelo marketing)

2 - **Adicionar CNAME para links de Tracking de email**

Adicione o email de marketing CNAME enviado para você, de modo que `[YourEmailCNAME]` aponte para [MktoTrackingLink], o link de rastreamento padrão atribuído pelo Marketo, no formato:\
`[YourEmailCNAME].[YourDomain].com` NO CNAME `[MktoTrackingLink]`

Por exemplo:

`pages.abc.com IN CNAME mkto-a0244.com`

3 - **Notificar sua equipe de marketing**

Informe sua equipe de marketing quando tiver concluído esse processo.

## Etapa 2: lista de permissões IPs de marketing {#step-allowlist-marketo-ips}

Quando seu grupo de marketing usa o Marketo para enviar emails de teste (uma prática recomendada antes de enviar blastos de email), os emails de teste às vezes são bloqueados por sistemas antisspam que dependem de endereços IP do remetente para verificar se o email é válido. Para garantir que os emails de teste cheguem, adicione Marketo à sua lista de permissões.

Adicione estes endereços IP à sua lista de permissões corporativa:

199.15.212.0/22\
192.28.144.0/20\
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

Alguns sistemas antisspam usam o campo Caminho de devolução de e-mail em vez do endereço IP para permitir. Nesses casos, a melhor abordagem é lista de permissões &quot;*.mktomail.com&quot;, já que o Marketo usa vários subdomínios de caixa de correio. Outros sistemas antisspam lista de permissões com base no endereço De. Nestas situações, certifique-se de incluir todos os domínios de envio (&quot;De&quot;) que seu grupo de marketing usa para se comunicar com pessoas/clientes potenciais.

>[!NOTE]
>
>A Postini emprega uma tecnologia exclusiva e exige incluir na lista de permissões intervalos IP. Consulte [Inclua na lista de permissões com Postini](http://nation.marketo.com/docs/DOC-1066).

## Etapa 3: Configurar SPF e DKIM {#step-set-up-spf-and-dkim}

Sua equipe de marketing também deve ter enviado informações do DKIM para adicioná-las ao seu registro de recursos do DNS (também listado abaixo). Siga as etapas para configurar com êxito o DKIM e o SPF e, em seguida, notifique sua equipe de marketing de que isso foi atualizado.

1. Para configurar o SPF, adicione a seguinte linha às nossas entradas DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   incluem: [mktomail.com](http://mktomail.com/) ~all

   Se já tivermos um registro SPF existente em nossa entrada DNS, basta adicionar o seguinte:\
   incluem: [mktomail.com](http://mktomail.com)

   Substitua CompanyDomain pelo domínio principal de seu site (por exemplo: &quot;`(company.com/)`&quot;) e CorpIP com o endereço IP do seu servidor de e-mail corporativo (por exemplo, &quot;255.255.255.255&quot;). Se você for enviar emails de vários domínios por meio do Marketo, sua equipe de TI deverá adicionar esta linha para cada domínio (em uma linha).

1. Para o DKIM, crie Registros de recursos de DNS para cada domínio que gostaríamos de configurar. Abaixo estão os Registros do host e os Valores TXT para cada domínio que assinaremos:

   `[DKIMDomain1]`: O Registro de host é `[HostRecord1]` e o Valor TXT é `[TXTValue1]`.

   `[DKIMDomain2]`: O Registro de host é `[HostRecord2]` e o Valor TXT é `[TXTValue2]`.

   Copie o HostRecord e o TXTValue para cada DKIMDomain que você configurou depois de seguir as [instruções aqui](https://docs.marketo.com/display/public/DOCS/Set+up+a+Custom+DKIM+Signature). Não se esqueça de verificar cada domínio em Admin > Email > DKIM depois que sua equipe de TI concluir esta etapa.

## Etapa 4: Configurar registros MX para o seu domínio {#step-set-up-mx-records-for-your-domain}

Um registro MX permite que você receba emails para o domínio do qual você está enviando emails para processar respostas e respondedores automáticos. Se você estiver enviando de seu domínio corporativo, provavelmente já está configurado. Caso contrário, você pode configurá-lo para mapear para o registro MX do domínio corporativo.
