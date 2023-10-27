---
unique-page-id: 4720433
description: Configurar protocolos para o Marketo - Documentação do Marketo - Documentação do produto
title: Configurar protocolos para o Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: f95721d5007fc686a8de7d11233cfe08ccce7237
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 4%

---

# Configurar protocolos para o Marketo {#configure-protocols-for-marketo}

Incluir na lista de permissões Se você ou sua organização usarem configurações restritivas de firewall ou servidor proxy, talvez você ou o administrador de rede precise pesquisar determinados domínios e intervalos de endereço IP para garantir que o Adobe Marketo Engage funcione conforme esperado.

Para obter ajuda sobre como implementar os protocolos abaixo, compartilhe este artigo com seu departamento de TI. Se eles restringirem o acesso à Web usando um incluo na lista de permissões, verifique se adicionaram os seguintes domínios (incluindo o asterisco) para permitir todos os recursos e websockets do Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Etapa 1: criar registros DNS para landing pages e email {#step-create-dns-records-for-landing-pages-and-email}

**Rastreamento de CNAMEs de link**

Sua equipe de marketing deve ter enviado duas solicitações para novos registros CNAME. O primeiro é para URLs de página de aterrissagem, para que as páginas de aterrissagem apareçam em URLs que refletem seu domínio, não o Marketo (o host real). O segundo é para os links de rastreamento incluídos nos emails enviados pelo Marketo.

`1` **Adicionar CNAME para landing pages**

Adicione a página de aterrissagem CNAME que eles enviaram para você ao registro DNS, para que `[YourLandingPageCNAME]` aponta para a Cadeia de caracteres da conta exclusiva atribuída às páginas de aterrissagem do Marketo. Faça logon no site do registrador de domínios e digite a página de aterrissagem CNAME e a sequência de caracteres da conta. Normalmente, isso envolve três campos:

* Alias: Enter `[YourLandingPageCNAME]` (fornecido por marketing)
* Tipo: CNAME
* Apontar para: Inserir `[MunchkinID].mktoweb.com` (fornecido por marketing)

`2` **Adicionar CNAME para links de rastreamento de email**

Adicione o email CNAME marketing enviado a você, para que `[YourEmailCNAME]` aponta para [MktoTrackingLink], o link de rastreamento padrão atribuído pelo Marketo, no formato:\
`[YourEmailCNAME].[YourDomain].com` EM CNAME `[MktoTrackingLink]`

Por exemplo:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` deve ser o Domínio de marca padrão.

`3` **Notifique a sua equipe de marketing**

Notifique a equipe de marketing quando concluir esse processo.

`4` **Contato [Suporte ao Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para iniciar o processo de provisionamento de um Certificado SSL.**

Esse processo pode levar até 3 dias úteis para ser concluído.

## Etapa 2: Marketo IPs da Incluir na lista de permissões {#step-allowlist-marketo-ips}

Quando seu grupo de marketing usa o Marketo para enviar emails de teste (uma prática recomendada antes de enviar propagações de email), os emails de teste às vezes são bloqueados por sistemas antisspam que dependem de endereços IP de remetente para verificar se o email é válido. Para garantir que esses emails de teste cheguem, adicione o Marketo ao seu incluo na lista de permissões de teste.

Incluir na lista de permissões Adicione esses endereços IP ao seu arquivo de pesquisa corporativo:

94.236.119.0/26

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Alguns sistemas antisspam usam o campo Return-Path do email em vez do endereço IP para incluir na lista de permissões. Nesses casos, a melhor abordagem é incluir na lista de permissões &quot;&#42;.mktomail.com&#39;, pois o Marketo usa vários subdomínios de caixa de correio. Outros sistemas antisspam incluem na lista de permissões com base no endereço Do. Nessas situações, inclua todos os domínios de envio (&quot;From&quot;) que seu grupo de marketing usa para se comunicar com pessoas/clientes potenciais.

>[!NOTE]
>
>O Postini emprega uma tecnologia exclusiva e requer o incluir na lista de permissões de intervalos IP. Consulte [➡ Incluindo na lista de permissões com Postini](https://nation.marketo.com/docs/DOC-1066).

## Etapa 3: configurar SPF e DKIM {#step-set-up-spf-and-dkim}

Sua equipe de marketing também deve ter enviado informações DKIM para você serem adicionadas ao seu registro de recurso DNS (também listado abaixo). Siga as etapas para configurar com êxito o DKIM e o SPF e notifique sua equipe de marketing de que isso foi atualizado.

1. Para configurar o SPF, adicione a seguinte linha às suas entradas de DNS:

   `[CompanyDomain]` EM TXT v=spf1 mx ip4:`[CorpIP]`\
   incluir: mktomail.com ~all

   Se já tivermos um registro SPF existente em nossa entrada DNS, basta adicionar o seguinte a ele:\
   incluir: mktomail.com

   Substitua CompanyDomain pelo domínio principal do seu site (por exemplo: &quot;`(company.com/)`&quot;) e CorpIP com o endereço IP do seu servidor de email corporativo (por exemplo, &quot;255.255.255.255&quot;). Se você for enviar emails de vários domínios por meio do Marketo, a equipe de TI deve adicionar essa linha para cada domínio (em uma linha).

1. Para DKIM, crie Registros de Recursos DNS para cada domínio que gostaríamos de configurar. Abaixo estão os Registros do host e Valores TXT para cada domínio que estaremos assinando:

   `[DKIMDomain1]`: o registro do host é `[HostRecord1]` e o Valor de TXT for `[TXTValue1]`.

   `[DKIMDomain2]`: o registro do host é `[HostRecord2]` e o Valor de TXT for `[TXTValue2]`.

   Copie o HostRecord e o TXTValue para cada DKIMDomain que você configurou depois de seguir o [instruções aqui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. Não se esqueça de verificar cada domínio em Admin > Email > DKIM depois que sua equipe de TI concluir esta etapa.

## Etapa 4: configurar registros MX para o seu domínio {#step-set-up-mx-records-for-your-domain}

Um registro MX permite receber emails do domínio do qual você está enviando email para processar respostas e respostas automáticas. Se estiver enviando do domínio corporativo, provavelmente você já tem essa configuração. Caso contrário, geralmente é possível configurá-lo para mapear para o registro MX do domínio corporativo.

## Endereços IP de Saída {#outbound-ip-addresses}

Uma conexão de saída é feita por Marketo Engage a um servidor na Internet em seu nome. Alguns parceiros/fornecedores com os quais você trabalha ou sua própria organização de TI podem usar as listas de permissões de para restringir o acesso aos servidores. Em caso positivo, você deve fornecer a eles blocos de endereço IP de saída Marketo Engage para adicionar às suas incluis na lista de permissões.

**Webhooks**

Marketo Engage [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} A ação de fluxo é executada como parte de uma campanha inteligente, uma solicitação HTTP é feita a um serviço da web externo. Incluir na lista de permissões incluir na lista de permissões Se o editor de serviços da Web usar um arquivo de replicação na rede em que o serviço da Web externo está localizado, o editor deverá adicionar os blocos de endereço IP listados abaixo ao seu arquivo de replicação.

**Sincronização com CRM**

Marketo Engage [Sincronização do Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} são mecanismos de integração que fazem solicitações HTTP de saída para APIs publicadas pelo seu fornecedor de CRM. Você deve garantir que sua organização de TI não bloqueie o acesso das APIs do fornecedor de CRM a nenhum dos blocos de endereço IP abaixo.

**Blocos de Endereço IP de Saída Marketo Engage**

As tabelas a seguir cobrem todos os servidores Marketo Engage que fazem chamadas de saída. Incluir na lista de permissões Use as listas abaixo se você estiver configurando um arquivo IP, servidor, firewall, lista de controle de acesso, grupo de segurança ou serviço de terceiros para receber conexões de saída do Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Bloco IP (Notação CIDR)</th>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>130.248.244.88/29</td>
  </tr>
  <tr>
   <td>185.28.196.0/22</td>
  </tr>
  <tr>
   <td>192.28.144.0/20</td>
  </tr>
  <tr>
   <td>192.28.160.0/19</td>
  </tr>
  <tr>
   <td>199.15.212.0/22</td>
  </tr>
 </tbody>
</table>

<table>
 <tbody>
  <tr>
   <th>Endereço IP individual</th>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
  <tr>
   <td>35.165.244.220</td>
  </tr>
  <tr>
   <td>44.235.171.179</td>
  </tr>
  <tr>
   <td>52.20.211.99</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
  <tr>
   <td>54.220.138.65</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.16</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>

</tbody>
</table>

