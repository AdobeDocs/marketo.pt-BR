---
unique-page-id: 4720433
description: Configurar protocolos para o Marketo Engage - Documentação do Marketo Engage - Documentação do produto
title: Configurar protocolos para o Marketo Engage
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '2131'
ht-degree: 8%

---

# Configurar protocolos para o Marketo Engage{#configure-protocols-for-marketo-engage}

Incluir na lista de permissões Se você ou sua organização usarem configurações restritivas de firewall ou servidor proxy, talvez você ou o administrador de rede precise pesquisar determinados domínios e intervalos de endereço IP para garantir que o Adobe Marketo Engage funcione conforme esperado.

Para obter ajuda sobre como implementar os protocolos abaixo, compartilhe este artigo com seu departamento de TI. Se eles restringirem o acesso à Web usando um incluo na lista de permissões, verifique se adicionaram os seguintes domínios (incluindo o asterisco) para permitir todos os recursos e websockets do Marketo Engage:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Etapa 1: criar registros DNS para landing pages e email {#step-create-dns-records-for-landing-pages-and-email}

**CNAMEs do Link de Rastreamento**

Sua equipe de marketing deve ter enviado duas solicitações para novos registros CNAME. O primeiro é para URLs de página de aterrissagem, para que as páginas de aterrissagem apareçam em URLs que refletem seu domínio, não o Marketo Engage (o host real). O segundo é para os links de rastreamento incluídos nos emails enviados pelo Marketo Engage.

`1` **Adicionar CNAME para Páginas de Aterrissagem**

Adicione a CNAME da página de aterrissagem que eles enviaram a você ao seu registro DNS, para que `[YourLandingPageCNAME]` aponte para a Cadeia de Caracteres da Conta exclusiva atribuída às Páginas de aterrissagem do Marketo Engage. Faça logon no site do registrador de domínios e digite a página de aterrissagem CNAME e a sequência de caracteres da conta. Normalmente, isso envolve três campos:

* Alias: insira `[YourLandingPageCNAME]` (fornecido por marketing)
* Tipo: CNAME
* Apontar para: Insira `[MunchkinID].mktoweb.com` (fornecido por marketing)

`2` **Adicionar CNAME para Links de Acompanhamento de Email**

Adicione o email CNAME marketing enviado a você, para que `[YourEmailCNAME]` aponte para [MktoTrackingLink], o link de rastreamento padrão atribuído pelo Marketo Engage, no formato:
`[YourEmailCNAME].[YourDomain].com` NO CNAME `[MktoTrackingLink]`

Por exemplo:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` deve ser o Domínio de marca padrão.

`3` **Notifique a sua equipe de marketing**

Notifique a equipe de marketing quando concluir esse processo.

`4` **Contate o [Suporte da Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para iniciar o processo de provisionamento de um Certificado SSL.**

Esse processo pode levar até 3 dias úteis para ser concluído.

## Etapa 2: Marketo Engage IPs da Incluir na lista de permissões {#step-allowlist-marketo-ips}

Quando seu grupo de marketing usa o Marketo Engage para enviar emails de teste (uma prática recomendada antes de enviar propagações de email), os emails de teste às vezes são bloqueados por sistemas antisspam que dependem de endereços IP de remetente para verificar se o email é válido. Para garantir que esses emails de teste cheguem, adicione o Marketo Engage ao seu incluo na lista de permissões de teste.

Incluir na lista de permissões Adicione esses endereços IP ao seu arquivo de pesquisa corporativo:

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Alguns sistemas antisspam usam o campo Return-Path do email em vez do endereço IP para incluir na lista de permissões. Incluir na lista de permissões Nesses casos, a melhor abordagem é pesquisar o arquivo &#39;&#42;.mktomail.com&#39;, pois o Marketo Engage usa vários subdomínios de caixa de correio. Outros sistemas antisspam incluem na lista de permissões com base no endereço Do. Nessas situações, inclua todos os domínios de envio (&quot;From&quot;) que seu grupo de marketing usa para se comunicar com pessoas/clientes potenciais.

>[!NOTE]
>
>O Postini emprega uma tecnologia exclusiva e requer o incluir na lista de permissões de intervalos IP. Consulte [Incluindo na lista de permissões com Postini](https://nation.marketo.com/docs/DOC-1066).

## Etapa 3: configurar o SPF e o DKIM {#step-set-up-spf-and-dkim}

Sua equipe de marketing também deve ter enviado informações do DKIM (Domain Keys Identified Mail) para que sejam adicionadas ao registro de recursos DNS (também listadas abaixo). Siga as etapas para configurar com êxito o DKIM e o SPF (Sender Policy Framework) e, em seguida, notifique sua equipe de marketing de que isso foi atualizado.

1. Para configurar o SPF, adicione a seguinte linha às suas entradas de DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`
incluir: mktomail.com ~all

   Se já tivermos um registro SPF existente em nossa entrada DNS, basta adicionar o seguinte a ele:
incluir: mktomail.com

   Substitua CompanyDomain pelo domínio principal do site (por exemplo: &quot;`(company.com/)`&quot;) e CorpIP pelo endereço IP do servidor de email corporativo (por exemplo, 255.255.255.255). Se você for enviar emails de vários domínios por meio do Marketo Engage, a equipe de TI deve adicionar essa linha para cada domínio (em uma linha).

1. Para o DKIM, crie Registros de Recursos de DNS para cada domínio que gostaríamos de configurar. Abaixo estão os Registros do host e Valores TXT para cada domínio que estaremos assinando:

   `[DKIMDomain1]`: o Registro do Host é `[HostRecord1]` e o Valor TXT é `[TXTValue1]`.

   `[DKIMDomain2]`: o Registro do Host é `[HostRecord2]` e o Valor TXT é `[TXTValue2]`.

   Copie o HostRecord e o TXTValue para cada DKIMDomain que você configurou depois de seguir as [instruções aqui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. Não se esqueça de verificar cada domínio em Admin > Email > DKIM depois que sua equipe de TI concluir esta etapa.

## Etapa 4: configurar o DMARC {#set-up-dmarc}

O DMARC (Domain-based Message Authentication, Reporting &amp; Conformance) é um protocolo de autenticação usado para ajudar as organizações a proteger seu domínio contra o uso não autorizado. O DMARC estende os protocolos de autenticação existentes, como SPF e DKIM, para informar aos servidores recipients quais ações eles devem tomar caso ocorra uma falha na autenticação em seus domínios. Embora o DMARC seja opcional no momento, ele é altamente recomendado, pois protegerá melhor a marca e a reputação de sua organização. Os principais provedores, como Google e Yahoo, exigirão o uso do DMARC para remetentes em massa a partir de fevereiro de 2024.

Para que o DMARC funcione, você deve ter pelo menos um dos seguintes registros DNS TXT:

* Uma SPF válida
* Um registro DKIM válido para o domínio FROM: (recomendado para Marketo Engage)

Além disso, você deve ter um registro TXT de DNS específico da DMARC para o seu FROM: Domain. Opcionalmente, um endereço de email de sua escolha pode ser definido para indicar para onde os relatórios do DMARC devem ir na organização, para que você possa monitorar os relatórios.

Como prática recomendada, é recomendável implantar lentamente a implementação do DMARC, escalando sua política do DMARC de p=none para p=quarantine, para p=reject conforme você entende o impacto potencial do DMARC e definir sua política do DMARC para alinhamento relaxado no SPF e no DKIM.

### Exemplo de fluxo de trabalho do DMARC {#dmarc-example-workflow}

1. Se estiver configurado para receber relatórios do DMARC, você deve fazer o seguinte...

   I. Analise o feedback e os relatórios que você recebe e usa (p=none), o que instrui o destinatário a não executar nenhuma ação contra mensagens com falha de autenticação, mas ainda enviar relatórios de email ao remetente.

   II. Revise e corrija problemas com o SPF/DKIM se as mensagens legítimas estiverem falhando na autenticação.

   III. Determine se a SPF ou o DKIM estão alinhados e autenticando todos os emails legítimos.

   IV. Revise os relatórios para garantir que os resultados sejam os esperados com base em suas políticas SPF/DKIM.

1. Continue para ajustar a política para (p=quarentena), que instrui o servidor de email de recebimento a colocar em quarentena emails que não são autenticados (geralmente significa colocar essas mensagens na pasta de spam).

   I. Analise os relatórios para garantir que os resultados sejam o que você espera.

1. Se você estiver satisfeito com o comportamento das mensagens no nível p=quarentena, será possível ajustar a política para (p=reject). A política p=reject informa ao destinatário para negar completamente (retornar) qualquer email para o domínio que não é autenticado. Com essa política ativada, somente os emails verificados como 100% autenticados pelo seu domínio terão uma chance de inserção na caixa de entrada.

>[!CAUTION]
>
>Use esta política com cautela e determine se ela é apropriada para sua organização.

### Relatórios do DMARC {#dmarc-reporting}

O DMARC oferece a capacidade de receber relatórios sobre emails com falham na SPF/DKIM. Há dois relatórios diferentes gerados por servidores ISP como parte do processo de autenticação que os remetentes podem receber por meio das tags RUA/RUF em sua política do DMARC.

* Relatórios agregados (RUA): não contém nenhuma PII (Informações de identificação pessoal) que seja sensível ao GDPR (Regulamento Geral sobre a Proteção de Dados).

* Relatórios forenses (RUF): contém endereços de email que são sensíveis ao GDPR. Antes de usar o, é melhor verificar internamente como lidar com informações que precisam ser compatíveis com o GDPR.

O principal uso desses relatórios é receber uma visão geral dos emails que são tentativas de falsificação. Esses relatórios são altamente técnicos e são melhor analisados por meio de uma ferramenta de terceiros.

### Exemplo de registros DMARC {#example-dmarc-records}

* Registro mínimo: `v=DMARC1; p=none`

* Registro direcionando para um endereço de email para receber relatórios: `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### Tags do DMARC e suas funções {#dmarc-tags-and-what-they-do}

Os registros DMARC têm vários componentes chamados tags DMARC. Cada tag tem um valor que especifica um determinado aspecto do DMARC.

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
    <td>Mostra a política do DMARC selecionada e direciona o destinatário para relatar, colocar em quarentena ou rejeitar emails que não passaram nas verificações de autenticação.</td>
    <td>p=nenhum, colocar em quarentena ou rejeitar</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Opcional</td>
    <td>Permite que o proprietário do domínio especifique opções de relatórios.</td>
    <td>0: Gerar relatório se tudo falhar
    <br>1: gerar relatório se algo falhar
    <br>d: gerar relatório se o DKIM falhar
    <br>s: gerar relatório se o SPF falhar</td>
    <td>1 (recomendado para relatórios do DMARC)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>Opcional</td>
    <td>Informa a porcentagem de mensagens sujeitas à filtragem.</td>
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
    <td>Especifica a política do DMARC para subdomínios do domínio pai.</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>Opcional</td>
    <td>Pode ser Estrito (s) ou Relaxado ®. Alinhamento simples significa que o domínio usado na assinatura do DKIM pode ser um subdomínio do endereço "De". Alinhamento estrito significa que o domínio usado na assinatura do DKIM deve corresponder exatamente ao domínio usado no endereço "De".</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>Opcional</td>
    <td>Pode ser Estrito (s) ou Relaxado ®. Alinhamento relaxado significa que o Domínio do ReturnPath pode ser um subdomínio do Endereço do remetente. Alinhamento estrito significa que o domínio Return-Path deve ter uma correspondência exata com o endereço From.</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

Para obter detalhes completos sobre a DMARC e todas as suas opções, visite [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC e MARKETO ENGAGE {#dmarc-and-marketo-engage}

Há dois tipos de alinhamento para o DMARC — alinhamento DKIM e alinhamento SPF.

>[!NOTE]
>
>É recomendável fazer o alinhamento do DMARC no DKIM versus o SPF para o Marketo Engage.

* DMARC alinhado à DKIM — Para configurar o DMARC alinhado à DKIM, você deve:

   * Configure o DKIM para o FROM: domínio da sua mensagem. Use as instruções [neste artigo](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Configure o DMARC para o domínio FROM:/DKIM que foi configurado anteriormente

* SPF alinhado à DMARC — Para configurar o SPF alinhado à DMARC por meio de um caminho de retorno com marca, você deve:

   * Configurar o domínio do caminho de retorno com marca
      * Configurar o registro SPF apropriado
      * Altere o registro MX para apontar de volta para o MX padrão do data center do qual seu email será enviado

   * Configurar o DMARC para o domínio do caminho de retorno com marca

* Se você estiver enviando emails da Marketo Engage por meio de um IP dedicado e ainda não tiver implementado um caminho de retorno com marca, ou se não tiver certeza se já implementou, abra um tíquete com o [Suporte da Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Se você estiver enviando emails do Marketo Engage por meio de um pool compartilhado de IPs, poderá ver se está qualificado para IPs Confiáveis [inscrevendo-se aqui](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. O caminho de retorno de marca é oferecido gratuitamente para os envios de IPs confiáveis da Marketo Engage. Se aprovado para este programa, entre em contato com o Suporte da Adobe para configurar um caminho de retorno de marca.

   * IPs confiáveis: um pool compartilhado de IPs reservados para usuários de menor volume que enviam menos de 75 mil por mês e não se qualificam para um IP dedicado. Esses usuários também devem atender aos requisitos das práticas recomendadas.

* Se estiver enviando emails da Marketo Engage por meio de IPs compartilhados e não se qualificar para IPs confiáveis e enviar mais de 100.000 mensagens por mês, você precisará entrar em contato com a Equipe de contas da Adobe (seu gerente de conta) para comprar um IP dedicado.

* O alinhamento estrito do SPF não é compatível nem recomendado no Marketo Engage.

## Etapa 5: Configurar registros MX para o seu domínio {#step-set-up-mx-records-for-your-domain}

Um registro MX permite que você receba emails no domínio de onde está enviando os emails para processar respostas e respostas automáticas. Se estiver enviando do domínio corporativo, provavelmente você já tem essa configuração. Caso contrário, geralmente é possível configurá-lo para mapear para o registro MX do domínio corporativo.

## Endereços IP de Saída {#outbound-ip-addresses}

Uma conexão de saída é feita pelo Marketo Engage a um servidor na Internet em seu nome. Alguns parceiros/fornecedores com os quais você trabalha ou sua própria organização de TI podem usar as listas de permissões de para restringir o acesso aos servidores. Nesse caso, você deve fornecer a eles blocos de endereços IP de saída do Marketo Engage para adicionar às suas listas de permissão.

**Webhooks**

Os [Webhooks](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} do Marketo Engage são um mecanismo de integração de saída. Quando uma ação de fluxo [Webhook de chamada](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} é executada como parte de uma campanha inteligente, uma solicitação HTTP é feita a um serviço da Web externo. Incluir na lista de permissões incluir na lista de permissões Se o editor de serviços da Web usar um arquivo de replicação na rede em que o serviço da Web externo está localizado, o editor deverá adicionar os blocos de endereço IP listados abaixo ao seu arquivo de replicação.

**Sincronização do CRM**

A [Sincronização do Salesforce CRM](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} e a [Sincronização do Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} do Marketo Engage são mecanismos de integração que fazem solicitações HTTP de saída para APIs publicadas pelo seu fornecedor de CRM. Você deve garantir que sua organização de TI não bloqueie o acesso das APIs do fornecedor de CRM a nenhum dos blocos de endereço IP abaixo.

**Blocos de Endereço IP de Saída do Marketo Engage**

As tabelas a seguir abordam todos os servidores do Marketo Engage que fazem chamadas de saída. Incluir na lista de permissões Use as listas abaixo se você estiver configurando um arquivo IP, servidor, firewall, lista de controle de acesso, grupo de segurança ou serviço de terceiros para receber conexões de saída do Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Bloco de IP (Notação CIDR)</th>
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
   <td>13 237 155 207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34 247 24 245</td>
  </tr>
  <tr>
   <td>35 165 244 220</td>
  </tr>
  <tr>
   <td>44 235 171 179</td>
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
   <td>54 212 167 17</td>
  </tr>
  <tr>
   <td>54 220 138 65</td>
  </tr>
   <tr>
   <td>54 237 141 197</td>
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
