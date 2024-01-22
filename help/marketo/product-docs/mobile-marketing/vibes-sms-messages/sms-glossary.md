---
description: Glossário de SMS - Documentação do Marketo - Documentação do produto
title: Glossário de SMS
feature: Mobile Marketing
source-git-commit: efaf34e8113fc6364655ff01aa788aa62bdd31af
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Glossário de SMS {#sms-glossary}

Abaixo estão alguns termos comuns que você encontrará ao usar mensagens SMS do Vibes com o Marketo Engage.

<table>
<thead>
  <tr>
    <th>Termo</th>
    <th>Definição</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Campanha de aquisição</td>
    <td>Uma campanha feita para adquirir novos assinantes para suas listas de assinaturas. Um assinante pode ser adicionado a uma campanha de aquisição por meio de um formulário web do Marketo ou enviando uma mensagem de texto com uma palavra-chave.</td>
  </tr>
  <tr>
    <td>Gerente de campanha</td>
    <td>Localizado na plataforma Vibes, o Gerenciador de campanhas é o local onde você pode configurar uma lista de assinaturas e uma campanha de aquisição. Os usuários com uma licença completa da plataforma Vibes têm acesso a tipos adicionais de campanha.</td>
  </tr>
  <tr>
    <td>Chave da empresa</td>
    <td>A company_key é um identificador alfanumérico exclusivo para a conta da plataforma. Se você tiver várias contas da empresa na plataforma Vibes (como contas de crianças), poderá ter várias company_keys. Cada instância de Marketo Engage pode ser mapeada somente para uma chave de empresa Vibes.</td>
  </tr>
  <tr>
    <td>CTA (plano de ação)</td>
    <td>Sinalização digital ou física ou script verbal para adquirir assinantes em um programa de mensagem de texto recorrente ou lista de assinaturas. Pode ser colocado on-line, em redes sociais, em e-mails, em papel, etc.</td>
  </tr>
  <tr>
    <td>Domínio curto personalizado</td>
    <td>Se você estiver usando o encurtador de links Vibes, o URL mais curto, por padrão, aparecerá no URL mais curto Vibes: https://vbs.cm/xxxxxx. Um domínio curto personalizado é um domínio exclusivo da sua marca. <a href="https://developer-platform.vibes.com/docs/creating-a-custom-short-domain">Saiba mais sobre domínios curtos personalizados</a>.<p>
    Isso se aplica somente a mensagens enviadas da plataforma Vibes, especificamente as mensagens da campanha de aquisição e as mensagens padrão de código curto.<p>
    O encurtador de URL do Marketo é recomendado para ter dados de cliques no programa do Marketo.</td>
  </tr>
  <tr>
    <td>Mensagens padrão</td>
    <td>Mensagens obrigatórias para o código curto responder a solicitações HELP, STOP e unknown message.</td>
  </tr>
  <tr>
    <td>Desconectar</td>
    <td>Desconexões são uma forma de recusa devido ao número de celular que está sendo removido de uma rede de operadora. Os motivos para uma desconexão incluem: uma conta foi totalmente fechada, uma conta pré-paga ficou sem fundos ou o número foi removido da rede da operadora por outros motivos desconhecidos. Os números de celular desconectados e não transferidos para outra operadora de celular têm a assinatura cancelada de todas as listas de assinatura na plataforma Vibes.</td>
  </tr>
  <tr>
    <td>Aceitação dupla</td>
    <td>Um método de aquisição que exige que um assinante em potencial confirme seu consentimento para ser adicionado a uma lista de assinaturas com um comando de resposta, como "Y" ou seu código postal. Usar um prompt de aceitação duplo pode ajudar você a cumprir as diretrizes de mensagens de texto estaduais e federais.</td>
  </tr>
  <tr>
    <td>Evento</td>
    <td>Um evento é uma ocorrência definida que pode ser enviada para a plataforma Vibes e usada para acionar ações acionadas por API, incluindo envios de mensagem. Cada evento contém dados específicos para o evento, incluindo um event_type, que é usado para determinar a campanha de mensagem acionada por API correspondente. A API de evento pode ser acionada por meio de um Webhook no Marketo Engage. Saiba mais com a nossa <a href="https://developer-platform.vibes.com/reference/event-api">Referência da API de evento</a>.</td>
  </tr>
  <tr>
    <td>Palavra-chave</td>
    <td>Uma palavra curta ou uma sequência alfanumérica enviada pelo consumidor ao código curto para iniciar uma experiência móvel.</td>
  </tr>
  <tr>
    <td>Código longo (10DLC)</td>
    <td>Uma ID de remetente da qual mensagens bidirecionais são enviadas entre a marca e o consumidor. Os códigos longos dos EUA têm 10 dígitos numéricos.</td>
  </tr>
  <tr>
    <td>MDN</td>
    <td>Número do Diretório de Celular ou o número de telefone de uma pessoa. Os números MDN e de telefone celular não são identificadores exclusivos no Marketo.</td>
  </tr>
  <tr>
    <td>Banco de dados móvel</td>
    <td>O banco de dados móvel é o banco de dados onde o Vibes armazena dados do assinante. Cada assinante tem um "registro de pessoa" exclusivo, em que o número do celular e quaisquer campos personalizados associados são preenchidos.</td>
  </tr>
  <tr>
    <td>Participante</td>
    <td>Uma pessoa que tem uma ou mais interações móveis (como o envio de uma mensagem de texto) com seu programa móvel, mas não se inscreveu em uma lista de assinaturas.</td>
  </tr>
  <tr>
    <td>Registro de pessoa</td>
    <td>Um registro de pessoa é uma coleção de dados para um número de telefone celular específico. Cada registro de pessoa também recebe uma person_key exclusiva para identificação. As IDs do Marketo são vinculadas às Vibrações usando o campo external_person_id. Saiba mais sobre registros de pessoa no <a href="https://developer-platform.vibes.com/reference/person-api">Documentação da API da pessoa de Vibes</a>.</td>
  </tr>
  <tr>
    <td>Código curto</td>
    <td>Uma ID de remetente da qual mensagens bidirecionais são enviadas entre a marca e o consumidor. Os códigos curtos dos EUA têm de 5 a 6 dígitos numéricos. Os códigos curtos canadenses têm de 4 a 6 dígitos numéricos. A integração do Marketo LaunchPoint com o Vibes é compatível com um código curto por instância.</td>
  </tr>
  <tr>
    <td>SMS</td>
    <td>Serviço de mensagens curtas. Esta é uma mensagem que inclui somente texto.</td>
  </tr>
  <tr>
    <td>Listas de assinaturas</td>
    <td>Uma lista de números de celular (e seus registros de pessoa correspondentes) que consentiram em receber mensagens recorrentes do seu programa.</td>
  </tr>
  <tr>
    <td>Assinante</td>
    <td>Um número de celular que se inscreveu em uma ou mais listas de inscrição.</td>
  </tr>
  <tr>
    <td>Plataforma Vibes</td>
    <td>O site no qual você faz logon para gerenciar suas campanhas. Ir para <a href="https://nexus.us.vibes.com/">https://nexus.us.vibes.com/</a> para acessar a plataforma Vibes.</td>
  </tr>
</tbody>
</table>
