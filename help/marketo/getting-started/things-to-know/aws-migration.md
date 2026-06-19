---
description: Migração do AWS - Documentação do Marketo Engage - Documentação do produto
title: Migração do AWS
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 6137b262cf085d5b270d16e0bf3e4e39351c5af4
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 3%

---

# Migração do AWS {#aws-migration}

Nos próximos meses, todas as assinaturas do Marketo Engage estarão sendo migradas de um data center privado para a nuvem pública da AWS para melhorar a confiabilidade, a escalabilidade e a velocidade.

Você receberá um email e uma notificação no aplicativo aproximadamente 30 dias antes da migração. Use este guia para se preparar.

## Ações recomendadas

Durante a janela de migração, todos os serviços da Marketo Engage ficarão indisponíveis. Recomendamos seguir as etapas a seguir para atenuar qualquer impacto em sua empresa.

* **Evite criar ou atualizar clientes potenciais/pessoas** ou executar processos que modificam registros de Pessoa.

* **Não acionar processos de acompanhamento**, pois as campanhas agendadas serão pausadas.

* **Desabilite temporariamente todas as integrações** que enviam ou recebem dados para ou da Marketo Engage.

* **Evite executar** importações ou exportações de dados ou quaisquer campanhas importantes de geração de leads/pessoas.

* **Revise e atualize as incluis na lista de permissões de IP** para logon, acesso à API, envio de email, rastreamento Web e integrações.

* **Adicione novos endereços IP** e mantenha seus IPs atuais como estão. Consulte os endereços IP a serem adicionados através da [tabela abaixo](#ip-addresses).

## Impactos esperados do serviço

Os impactos abaixo não exigem nenhuma ação da sua parte.

* **As integrações de CRM e os serviços do LaunchPoint** serão desabilitados, mas serão retomados automaticamente depois.
* **As páginas de aterrissagem, os formulários e a coleção de dados** não estarão disponíveis, e uma mensagem de manutenção será exibida.

## Identificar o data center/pod {#identify}

Antes de examinar as tabelas abaixo, [saiba como identificar](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) em qual data center e pod/servidor sua assinatura está localizada.

## Programação {#schedule}

Novas datas e informações de data center/pod são adicionadas periodicamente, portanto, verifique aqui para obter detalhes.

<table>
 <tbody>
  <tr>
   <th style="width:50%">Data</th>
   <th style="width:20%">Data Center/Pod</th>
   <th style="width:30%">Hora</th>
  </tr>
  <tr>
   <td>19 de junho de 2026</td>
   <td>AB46</td>
   <td>17:00 PST</td>
  </tr>
  <tr>
   <td>8 de julho de 2026</td>
   <td>AB69<br>
   AB64</td>
   <td>17:00 PST<br>
   18h00 PST</td>
  </tr>
  <tr>
   <td>9 de julho de 2026</td>
   <td>AB70<br>
   AB43</td>
   <td>17:00 PST<br>
   18h00 PST</td>
  </tr>
  &lt;/body>
  </table>

## Endereços IP a serem adicionados {#ip-addresses}

Com base em seu data center, trabalhe com seu departamento de TI para adicionar os respectivos endereços IP.

<table>
 <tbody>
  <tr>
   <th style="width:25%">Centro de dados</th>
   <th style="width:75%">Endereços IP</th>
  </tr>
  <tr>
   <td>AB</td>
   <td>54.160.246.246<br>
   54.237.141.197<br>
   52.20.211.99</td>
  </tr>
  <tr>
   <td>NLD</td>
   <td>34.247.24.245<br>
18.200.201.81<br>
54.220.138.65</td>
  </tr>
  &lt;/body>
  </table>

## Atualizações e suporte

Para obter as atualizações mais recentes, salve esta página como favorita. Em caso de dúvidas, entre em contato com o Suporte da Adobe pelo Portal de suporte da Admin Console ou [Experience League](https://experienceleague.adobe.com/en/support){target="_blank"}.
