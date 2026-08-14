---
description: Migração do AWS - Documentação do Marketo Engage - Documentação do produto
title: Migração do AWS
feature: Getting Started
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 86ea4c057d6a02526083a14105ea036f835aad89
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 4%

---

# Migração do AWS {#aws-migration}

Nos próximos meses, todas as assinaturas do Marketo Engage estarão sendo migradas de um data center privado para a nuvem pública da AWS para melhorar a confiabilidade, a escalabilidade e a velocidade.

Você receberá um email e uma notificação no aplicativo aproximadamente 30 dias antes da migração. Use este guia para se preparar.

## Ações recomendadas {#actions}

Durante a janela de migração, todos os serviços da Marketo Engage ficarão indisponíveis. Recomendamos seguir as etapas a seguir para atenuar qualquer impacto em sua empresa.

* **Evite criar ou atualizar clientes potenciais/pessoas** ou executar processos que modificam registros de Pessoa.

* **Não acionar processos de acompanhamento**, pois as campanhas agendadas serão pausadas.

* **Desabilite temporariamente todas as integrações** que enviam ou recebem dados para ou da Marketo Engage.

* **Evite executar** importações ou exportações de dados ou quaisquer campanhas importantes de geração de leads/pessoas.

* **Revise e atualize as incluis na lista de permissões de IP** para logon, acesso à API, envio de email, rastreamento Web e integrações.

* **Adicione novos endereços IP** e mantenha seus IPs atuais como estão. Consulte os endereços IP a serem adicionados através da [tabela abaixo](#ip-addresses).

## Impactos esperados do serviço {#impacts}

Os impactos abaixo não exigem nenhuma ação da sua parte.

* **As integrações de CRM e os serviços do LaunchPoint** serão desabilitados, mas serão retomados automaticamente depois.
* **As páginas de aterrissagem, os formulários e a coleção de dados** não estarão disponíveis, e uma mensagem de manutenção será exibida.

>[!NOTE]
>
>Se você usa [formulários externos](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} e deseja evitar a perda de dados de envio de formulário coletados enquanto o Marketo Engage não estiver disponível durante a janela de migração, contate o [Suporte da Adobe](https://experienceleague.adobe.com/en/support){target="_blank"} **com pelo menos dois dias úteis** de antecedência e forneça a ID do Formulário e a Munchkin ID da sua assinatura.

## Identificar o data center/pod {#identify}

Antes de examinar as tabelas abaixo, [saiba como identificar](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) em qual data center e pod/servidor sua assinatura está localizada.

## Programação {#schedule}

Novas datas e informações de data center/pod são adicionadas ou alteradas periodicamente, portanto, monitore essa programação para obter atualizações.

+++Calendário de julho
<table>
 <tbody>
  <tr>
   <th style="width:25%">Data</th>
   <th style="width:25%">Data Center/Pod</th>
   <th style="width:25%">Hora</th>
   <th style="width:25%">Status</th>
  </tr>
  <tr>
   <td>8 de julho de 2026</td>
   <td>AB69<br>
   AB64</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Concluído<br>
   Concluído</td>
  </tr>
  <tr>
   <td>9 de julho de 2026</td>
   <td>AB70</td>
   <td>17:00 PDT</td>
   <td>Concluído</td>
  </tr>
  <tr>
   <td>11 de julho de 2026</td>
   <td>AB46</td>
   <td>10h PDT (horário do Pacífico)</td>
   <td>Concluído</td>
  </tr>
  <tr>
   <td>13 de julho de 2026</td>
   <td>NLD101</td>
   <td>10h PDT (horário do Pacífico)</td>
   <td>Concluído</td>
  </tr>
  <tr>
   <td>15 de julho de 2026</td>
   <td>NLD102<br>
   NLD104</td>
   <td>10h PDT (horário do Pacífico)<br>
   11:00 PDT</td>
   <td>Concluído<br>
   Concluído</td>
  </tr>
  <tr>
   <td>17 de julho de 2026</td>
   <td>NLD103<br>
   NLD105</td>
   <td>10h PDT (horário do Pacífico)<br>
   11:00 PDT</td>
   <td>Concluído<br>
   Concluído</td>
  </tr>
  <tr>
   <td>21 de julho de 2026</td>
   <td>AB54</td>
   <td>17:00 PDT</td>
   <td>Concluído</td>
  </tr>
  <tr>
   <td>23 de julho de 2026</td>
   <td>AB48</td>
   <td>17:00 PDT</td>
   <td>Concluído</td>
  </tr>
  <tr>
   <td>31 de julho de 2026</td>
   <td>AB43</td>
   <td>15h PDT</td>
   <td>Concluído</td>
  </tr>
  </body>
</table>

+++

<table>
 <tbody>
  <tr>
   <th style="width:25%">Data</th>
   <th style="width:25%">Data Center/Pod</th>
   <th style="width:25%">Hora</th>
   <th style="width:25%">Status</th>
  </tr>
  <tr>
   <td>12 de agosto de 2026</td>
   <td>AB61<br>
   AB17</td>
   <td>15h PDT<br>
   16:00 PDT</td>
   <td>Concluído<br>
   Concluído</td>
  </tr>
  <tr>
  <td>13 de agosto de 2026</td>
   <td>AB68</td>
   <td>16:00 PDT</td>
   <td>Concluído</td>
  </tr>
  <tr>
  <td>18 de agosto de 2026</td>
   <td>AB39</td>
   <td>17:00 PDT</td>
   <td>Adiado (data a ser definida)</td>
  </tr>
  <tr>
   <td>20 de agosto de 2026</td>
   <td>AB42<br>
   AB44</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>No cronograma<br>
   No prazo</td>
  </tr>
  <tr>
   <td>26 de agosto de 2026</td>
   <td>AB40<br>
   AB50</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>No cronograma<br>
   No prazo</td>
  </tr>
  <tr>
   <td>28 de agosto de 2026</td>
   <td>AB53<br>
   AB56</td>
   <td>15h PDT<br>
   16:00 PDT</td>
   <td>No cronograma<br>
   No prazo</td>
  </tr>
  <tr>
   <td>8 de setembro de 2026</td>
   <td>AB01<br>
   AB02</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>No cronograma<br>
   No prazo</td>
  </tr>
  <tr>
   <td>10 de setembro de 2026</td>
   <td>AB03</td>
   <td>17:00 PDT</td>
   <td>No cronograma</td>
  </tr>
  <tr>
   <td>15 de setembro de 2026</td>
   <td>AB05<br>
   AB06</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>No cronograma<br>
   No prazo</td>
  </tr>
  <tr>
   <td>17 de setembro de 2026</td>
   <td>AB07<br>
   AB08</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>No cronograma<br>
   No prazo</td>
  </tr>
  </body>
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
</body>
</table>

## Atualizações e suporte {#support}

Para obter as atualizações mais recentes, salve esta página como favorita. Em caso de dúvidas, entre em contato com o Suporte da Adobe pelo Portal de suporte da Admin Console ou [Experience League](https://experienceleague.adobe.com/en/support){target="_blank"}.

## Perguntas frequentes {#faq}

**Onde os dados são armazenados?**
Todos os dados de usuários do Marketo são armazenados no Amazon Web Services (AWS). A Marketo migrou sua infraestrutura de data centers físicos próprios para a plataforma de nuvem corporativa da AWS.

**Onde especificamente são armazenados os dados pessoais?**
Os dados pessoais são armazenados no Amazon Aurora, o serviço de banco de dados relacional totalmente gerenciado da AWS. A Aurora replica dados de seis maneiras em três zonas de disponibilidade separadas na região da AWS para proteger os dados pessoais contra falhas de hardware, degradação do armazenamento e eventos localizados de infraestrutura.

**Quem é o proprietário do ambiente de armazenamento?**
A infraestrutura de armazenamento pertence e é operada pela Amazon Web Services (AWS). A Adobe (Marketo) opera como cliente da AWS sob um modelo de responsabilidade compartilhada: a AWS é responsável pela segurança e disponibilidade da infraestrutura subjacente, enquanto a Adobe é responsável pela segurança dos dados e aplicativos em execução nela.

**Quais são os detalhes completos sobre produção, locais de backup/DR e tecnologia de armazenamento?**
O Marketo usa o Amazon Aurora, um mecanismo de banco de dados relacional nativo em nuvem totalmente gerenciado pela AWS, como sua tecnologia de banco de dados principal. A Aurora dissocia o computador e o armazenamento, replicando automaticamente os dados de seis maneiras em três zonas de disponibilidade na região de produção e exigindo um quorum de quatro cópias para confirmar qualquer operação de gravação.

O Aurora também executa backups automáticos contínuos no Amazon S3 em tempo real, permitindo a recuperação point-in-time (PITR) a qualquer segundo dentro da janela de retenção configurada.

No momento, a implantação do Marketo Aurora opera em uma única região da AWS, sem replicação entre regiões. Os dados de produção permanecem dentro da infraestrutura regional designada, e a recuperação de desastres é fornecida por meio da redundância de armazenamento de dados de vários AZ e backups contínuos do Aurora, em vez de failover geográfico para uma região secundária. Isso pode ser avaliado ainda mais à medida que a infraestrutura AWS da Marketo amadurece.
