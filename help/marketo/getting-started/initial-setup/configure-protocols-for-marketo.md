---
unique-page-id: 4720433
description: Configurar protocolos do Marketo Engage – Documentos do Marketo Engage – Documentação do produto
title: Configurar protocolos do Marketo Engage
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '2129'
ht-degree: 100%

---

# Configurar protocolos do Marketo Engage{#configure-protocols-for-marketo-engage}

Se você ou sua organização usarem configurações restritivas de firewall ou servidor proxy, talvez você ou o administrador de rede precisem incluir na lista de permissões determinados domínios e intervalos de endereço IP para garantir que o Adobe Marketo Engage funcione conforme esperado.

Para obter ajuda sobre como implementar os protocolos abaixo, compartilhe este artigo com seu departamento de TI. Se o departamento de TI restringir o acesso à web usando uma lista de permissões, solicite que adicionem os seguintes domínios (incluindo o asterisco) para permitir todos os recursos e websockets do Marketo Engage:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Etapa 1: criar registros DNS para páginas de destino e email {#step-create-dns-records-for-landing-pages-and-email}

**CNAMEs do link de rastreamento**

Sua equipe de marketing deve ter enviado duas solicitações para novos registros CNAME. O primeiro é para URLs de página de destino, para que elas apareçam em URLs que reflitam seu domínio, não o Marketo Engage (o host real). O segundo é para os links de rastreamento incluídos nos emails enviados pelo Marketo Engage.

`1` **Adicionar CNAME para páginas de destino**

Adicione o CNAME da página de destino que eles enviaram a você ao registro DNS, para que o `[YourLandingPageCNAME]` aponte para a string de conta exclusiva atribuída às páginas de destino do Marketo Engage. Faça logon no site do registrador de domínios e digite o CNAME da página de destino e a string de conta. Normalmente, isso envolve três campos:

* Alias: insira `[YourLandingPageCNAME]` (fornecido pela equipe de marketing)
* Tipo: CNAME
* Apontar para: insira `[MunchkinID].mktoweb.com` (fornecido pela equipe de marketing)

`2` **Adicionar CNAME para links de rastreamento de email**

Adicione o CNAME de email que a equipe de marketing enviou a você para que o `[YourEmailCNAME]` aponte para [MktoTrackingLink], o link de rastreamento padrão atribuído pelo Marketo Engage, no formato:
`[YourEmailCNAME].[YourDomain].com` NO CNAME `[MktoTrackingLink]`

Por exemplo:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` deve ser o Domínio de marca padrão.

`3` **Notifique a equipe de marketing**

Notifique a equipe de marketing quando concluir esse processo.

`4` **Entre em contato com o [Suporte da Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para iniciar o processo de provisionamento de um certificado SSL.**

Esse processo pode levar até 3 dias úteis para ser concluído.

## Etapa 2: incluir na lista de permissões IPs do Marketo Engage {#step-allowlist-marketo-ips}

Quando sua equipe de marketing usa o Marketo Engage para enviar emails de teste (uma prática recomendada antes do envio de emails em massa), esses emails às vezes são bloqueados por sistemas anti-spam que dependem dos endereços IP do remetente para verificar a validade do email. Para garantir que esses emails de teste cheguem ao destinatário, adicione o Marketo Engage à lista de permissões.

Adicione estes endereços IP à sua lista de permissões corporativa:

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Alguns sistemas anti-spam usam o campo do endereço de Return-Path do email em vez do endereço IP para determinar a permissão. Nesses casos, a melhor abordagem é incluir na lista de permissões “&#42;.mktomail.com”, pois o Marketo Engage usa vários subdomínios de caixa de correio. Outros sistemas anti-spam incluem listas de permissões baseadas no endereço do remetente. Nessas situações, inclua todos os domínios de envio (“De”) que seu grupo de marketing usa para se comunicar com pessoas/clientes potenciais.

>[!NOTE]
>
>Postini usa uma tecnologia exclusiva e exige a inclusão de intervalos de IP em listas de permissão. Consulte [Como incluir na lista de permissões com o Postini](https://nation.marketo.com/docs/DOC-1066).

## Etapa 3: configurar a SPF e o DKIM {#step-set-up-spf-and-dkim}

Sua equipe de marketing também deve ter enviado informações de DKIM (Domain Keys Identified Mail) para serem adicionadas ao seu registro de recurso DNS (também listado abaixo). Siga estas etapas para configurar o DKIM e a SPF (estrutura de política do remetente) e notifique a equipe de marketing quando ela for atualizada.

1. Para configurar a SPF, adicione a seguinte linha às entradas de DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`
include: mktomail.com ~all

   Se já tivermos um registro de SPF em nossa entrada DNS, basta adicionar o seguinte a ele: 
include: mktomail.com

   Substitua CompanyDomain pelo domínio principal do seu site (ex: “`(company.com/)`”) e CorpIP pelo endereço IP do seu servidor de email corporativo (ex: “255.255.255.255”). Se você for enviar emails de vários domínios por meio do Marketo Engage, a equipe de TI deve adicionar essa linha para cada domínio (em uma linha).

1. Para o DKIM, crie registros de recursos de DNS para cada domínio que gostaria de configurar. Abaixo estão os registros do host e valores TXT para cada domínio que assinaremos:

   `[DKIMDomain1]`: o Registro do Host é `[HostRecord1]` e o Valor TXT é `[TXTValue1]`.

   `[DKIMDomain2]`: o Registro do Host é `[HostRecord2]` e o Valor TXT é `[TXTValue2]`.

   Copie o HostRecord e o TXTValue para cada DKIMDomain que você configurou depois de seguir as [instruções aqui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. Não se esqueça de verificar cada domínio em Admin > Email > DKIM depois que sua equipe de TI concluir esta etapa.

## Etapa 4: configurar DMARC {#set-up-dmarc}

DMARC (Autenticação, Relatórios e Conformidade de Mensagens Baseadas em Domínio) é um protocolo de autenticação usado para ajudar organizações a proteger seus domínios contra uso não autorizado. Ele estende os protocolos de autenticação existentes, como SPF e DKIM, para informar os servidores destinatários sobre as ações a serem tomadas caso ocorra uma falha de autenticação em seu domínio. Embora o DMARC seja opcional no momento, ele é altamente recomendado, pois protegerá melhor a marca e a reputação da sua organização. Grandes provedores, como Google e Yahoo, começaram a exigir o uso do DMARC para remetentes em massa desde fevereiro de 2024.

Para que o DMARC funcione, você deve ter pelo menos um dos seguintes registros DNS TXT:

* Uma SPF válida
* Um registro DKIM válido para o domínio FROM: (recomendado para o Marketo Engage)

Além disso, você deve ter um registro TXT de DNS específico do DMARC para o domínio FROM:. Como opção, você pode definir um endereço de email de sua escolha para indicar para onde os relatórios DMARC devem ser enviados dentro da sua organização, permitindo que você monitore os relatórios.

Como prática recomendada, você deve fazer a implementação do DMARC lentamente, escalando a política do DMARC de p=nenhum para p=colocar em quarentena, para p=rejeitar conforme você entende o impacto potencial do DMARC e define sua política do DMARC para alinhamento relaxado na SPF e no DKIM.

### Exemplo de fluxo de trabalho do DMARC {#dmarc-example-workflow}

1. Se você configurou o recebimento de relatórios DMARC, siga os passos abaixo...

   I. Analise o feedback e os relatórios que você recebe e use (p=nenhum), que instrui o destinatário a não executar nenhuma ação em relação às mensagens que falham na autenticação, mas ainda assim enviar relatórios por email ao remetente.

   II. Analise e corrija problemas com a SPF/DKIM caso mensagens legítimas estejam com falha na autenticação.

   III. Determine se a SPF ou o DKIM estão alinhados e autenticando todos os emails legítimos.

   IV. Revise os relatórios para garantir que os resultados sejam os esperados com base nas políticas de SPF/DKIM.

1. Em seguida, ajuste a política para (p=colocar em quarentena), o que instrui o servidor de email receptor a colocar em quarentena os emails com falha na autenticação (normalmente, isso significa colocar essas mensagens na pasta de spam).

   I. Revise os relatórios para garantir que os resultados sejam o que era esperado.

1. Se você estiver satisfeito com o comportamento das mensagens no nível p=colocar em quarentena, você pode ajustar a política para (p=rejeitar). A política p=rejeitar instrui o destinatário a negar completamente (rejeição) qualquer email para o domínio com falha na autenticação. Com essa política habilitada, somente os emails que forem verificados como 100% autenticados pelo seu domínio terão chance de serem exibidos na caixa de entrada.

>[!CAUTION]
>
>Use esta política com cautela e determine se ela é apropriada para sua organização.

### Relatórios DMARC {#dmarc-reporting}

O DMARC oferece a capacidade de receber relatórios sobre emails com falhas na SPF/DKIM. Há dois relatórios diferentes gerados por servidores ISP como parte do processo de autenticação que os remetentes podem receber por meio das tags RUA/RUF em sua política DMARC.

* Relatórios agregados (RUA): não contêm nenhuma informação de identificação pessoal (PII) que seja sensível ao RGPD (Regulamento Geral sobre a Proteção de Dados).

* Relatórios forenses (RUF): contêm endereços de email que são sensíveis ao GDPR. Antes de usar, é melhor verificar internamente como lidar com informações que precisam estar em conformidade com o RGPD.

O principal uso desses relatórios é receber uma visão geral dos emails que são tentativas de falsificação. São relatórios altamente técnicos e são melhor assimilados por meio de uma ferramenta de terceiros.

### Exemplo de registros DMARC {#example-dmarc-records}

* Registro mínimo obrigatório: `v=DMARC1; p=none`

* Registro que direciona para um endereço de email para receber relatórios: `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### Tags DMARC e suas funções {#dmarc-tags-and-what-they-do}

Os registros DMARC têm vários componentes, chamados tags DMARC. Cada tag tem um valor que especifica um determinado aspecto do DMARC.

<table>
<thead>
  <tr>
    <th>Nome da tag </th>
    <th>Obrigatório/Opcional </th>
    <th>Função </th>
    <th>Exemplo </th>
    <th>Valor padrão </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>Obrigatório</td>
    <td>Esta tag DMARC especifica a versão. Há apenas uma versão a partir de agora, portanto, terá um valor fixo de v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>Obrigatório</td>
    <td>Exibe a política DMARC selecionada e instrui o destinatário a denunciar, colocar em quarentena ou rejeitar emails que não passarem nas verificações de autenticação.</td>
    <td>p=nenhum, colocar em quarentena ou rejeitar</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Opcional</td>
    <td>Permite que o proprietário do domínio especifique opções de relatórios.</td>
    <td>0: gerar relatório se tudo falhar
    <br>1: gerar relatório se algo falhar
    <br>d: gerar relatório se o DKIM falhar
    <br>s: gerar relatório se a SPF falhar</td>
    <td>1 (recomendado para relatórios DMARC)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>Opcional</td>
    <td>Especifica a porcentagem de mensagens sujeitas à filtragem.</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>Opcional (recomendado)</td>
    <td>Identifica onde os relatórios agregados serão entregues.</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>Opcional (recomendado)</td>
    <td>Identifica onde os relatórios forenses serão entregues.</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>Opcional</td>
    <td>Especifica a política DMARC para subdomínios do domínio principal.</td>
    <td>sp=rejeitar</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>Opcional</td>
    <td>Pode ser estrito (s) ou relaxado ®.  Alinhamento simples significa que o domínio é usado na assinatura do DKIM e pode ser um subdomínio do endereço “De”. Alinhamento estrito significa que o domínio usado na assinatura do DKIM deve ser uma correspondência exata do domínio usado no endereço “De”.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>Opcional</td>
    <td>Pode ser estrito (s) ou relaxado ®.  Alinhamento simples significa que o domínio ReturnPath pode ser um subdomínio do endereço De. Alinhamento estrito significa que o domínio Return-Path deve corresponder exatamente ao endereço De.</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

Para obter detalhes completos sobre o DMARC e todas as suas opções, acesse [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC e Marketo Engage {#dmarc-and-marketo-engage}

Há dois tipos de alinhamento para o DMARC — alinhamento DKIM e alinhamento SPF.

>[!NOTE]
>
>É recomendável fazer o alinhamento do DMARC no DKIM em relação à SPF para o Marketo Engage.

* DMARC alinhado ao DKIM: para configurar o DMARC alinhado ao DKIM, você deve:

   * Configurar o DKIM para o domínio FROM: da mensagem. Use as instruções [neste artigo](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Configure o DMARC para o domínio FROM:/DKIM que foi configurado anteriormente

* SPF alinhada ao DMARC: para configurar a SPF alinhada ao DMARC por meio de um return-path com marca, você deve:

   * Configurar o domínio Return-Path com marca
      * Configurar o registro SPF apropriado
      * Altere o registro MX para apontar de volta para o MX padrão do data center do qual seu email será enviado

   * Configurar o DMARC para o domínio Return-Path com marca

* Se você estiver enviando emails do Marketo Engage por meio de um IP dedicado e ainda não tiver implementado o return-path com marca, ou se não tiver certeza, abra um chamado junto ao [Suporte da Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Se você estiver enviando emails do Marketo Engage por meio de um pool compartilhado de IPs, poderá verificar se eles estão qualificados para IPs confiáveis [inscrevendo-se aqui](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. O return-path com marca é oferecido gratuitamente para quem envia emails de IPs confiáveis do Marketo Engage. Se aprovado para este programa, entre em contato com o Suporte da Adobe para configurar o return-path com marca.

   * IPs confiáveis: um conjunto compartilhado de IPs reservado para usuários com baixo volume de envio (&lt;75 mil/mês) que não se qualificam para um IP dedicado. Esses usuários também devem atender aos requisitos de práticas recomendadas.

* Se estiver enviando emails do Marketo Engage por meio de IPs compartilhados e não se qualificar para IPs confiáveis e enviar mais de 100.000 mensagens por mês, você precisará entrar em contato com a Equipe de contas da Adobe (seu gerente de conta) para comprar um IP dedicado.

* O alinhamento estrito da SPF não é compatível ou recomendado para o Marketo Engage.

## Etapa 5: configurar registros MX para o seu domínio {#step-set-up-mx-records-for-your-domain}

Um registro MX permite que você receba emails no domínio de onde está enviando os emails para processar respostas e respostas automáticas. Se estiver enviando do domínio corporativo, provavelmente você já tem essa configuração. Caso contrário, geralmente é possível configurá-lo para mapear para o registro MX do domínio corporativo.

## Endereços IP de saída {#outbound-ip-addresses}

Uma conexão de saída é aquela feita pelo Marketo Engage a um servidor na internet em seu nome. Alguns parceiros/fornecedores com quem você trabalha, ou seu próprio departamento de TI, podem usar listas de permissões para restringir o acesso aos servidores. Nesse caso, você deve fornecer a eles blocos de endereços IP de saída do Marketo Engage para adicionar às suas listas de permissão.

**Webhooks**

Os [webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} do Marketo Engage são um mecanismo de integração de saída. Quando uma ação de fluxo [Webhook de chamada](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} é executada como parte de uma campanha inteligente, uma solicitação HTTP é feita a um serviço da Web externo. Se o editor do serviço web usar uma lista de permissões no firewall da rede onde o serviço web externo está localizado, ele deverá adicionar os blocos de endereços IP indicados abaixo à sua lista de permissões.

**Sincronização com CRM**

A [sincronização do Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} e a [sincronização do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} do Marketo Engage são mecanismos de integração que fazem solicitações HTTP de saída para APIs publicadas pelo seu fornecedor de CRM. Você deve garantir que sua equipe de TI não bloqueie nenhum dos blocos de endereços IP abaixo, impedindo o acesso às APIs do seu fornecedor de CRM.

**Blocos de endereço IP de saída do Marketo Engage**

As tabelas a seguir englobam todos os servidores Marketo Engage que fazem chamadas de saída. Utilize as listas abaixo se estiver configurando alguma lista de permissões de IP, servidor, firewall, lista de controle de acesso, grupo de segurança ou serviço de terceiros para receber conexões de saída do Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Bloco de IP (Notação CIDR)</th>
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
  <tr>
   <td>124.47.174.193</td>
  </tr>
  <tr>
   <td>130.248.168.16</td>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
  <tr>
   <td>199.15.213.245</td>
  </tr>
  <tr>
   <td>199.15.215.245</td>
  </tr>
 </tbody>
</table>
