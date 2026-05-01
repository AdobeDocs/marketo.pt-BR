---
description: Migração do AWS - Documentação do Marketo Engage - Documentação do produto
title: Migração do AWS
feature: Getting Started
hide: true
hidefromtoc: true
source-git-commit: 88155ad99ba2899c3db3c1f7ae92a69f348dc020
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

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

* Adicione os seguintes endereços IP e mantenha seus IPs atuais como estão:

   * 54.160.246.246
   * 54.237.141.197
   * 52.20.211.99

## Impactos esperados do serviço

Os impactos abaixo não exigem nenhuma ação da sua parte.

* **As integrações de CRM e os serviços do LaunchPoint** serão desabilitados, mas serão retomados automaticamente depois.
* **As páginas de aterrissagem, os formulários e a coleção de dados** não estarão disponíveis, e uma mensagem de manutenção será exibida.

## Atualizações e suporte

Para obter as atualizações mais recentes, salve esta página como favorita. Em caso de dúvidas, entre em contato com o Suporte da Adobe pelo Portal de suporte da Admin Console ou [Experience League](https://experienceleague.adobe.com/en/support).

PARA ADICIONAR: POD/DETALHES DO DATA CENTER
