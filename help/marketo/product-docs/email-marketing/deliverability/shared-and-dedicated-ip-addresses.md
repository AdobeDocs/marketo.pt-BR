---
unique-page-id: 10912085
description: Endereços IP compartilhados e dedicados - Documentação do Marketo - Documentação do produto
title: Endereços IP Compartilhados e Dedicados
exl-id: 3d7a78f4-531a-4ad7-a20b-1385bd62d1d9
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Endereços IP Compartilhados e Dedicados {#shared-and-dedicated-ip-addresses}

## O que é um endereço IP? {#what-is-an-ip-address}

Um rótulo numérico que significa o endereço de um computador conectado à Internet.

## O que são endereços IP compartilhados? {#what-are-shared-ip-addresses}

Isso se refere a quando vários remetentes utilizam os mesmos endereços IP para iniciar campanhas de email. Todos eles compartilham os mesmos IPs de envio.

## O que é um endereço IP dedicado? {#what-is-a-dedicated-ip-address}

Um endereço IP específico do usuário que somente um remetente envia.

## O que é melhor — compartilhado ou dedicado? {#which-is-better-shared-or-dedicated}

Como de costume, há vantagens e desvantagens em ambas as opções.

**Vantagens e desvantagens de um IP dedicado**

_Vantagens_

**Reputação** - Você é totalmente proprietário da sua reputação e capacidade de entrega.\
**Monitoramento** - O monitoramento dos relatórios de capacidade de entrega permite que você responda rapidamente às alterações em suas métricas de entrega.\
**Resolução de problemas** - É mais fácil pesquisar, entender e resolver problemas de entrega.

_Contras_

**Alterações de volume** - Os picos de volume podem afetar negativamente sua reputação e precisam ser gerenciados.\
**Processo de aquecimento de IP** - A reputação é criada ao longo do tempo. Alguns ISPs (provedores de serviço de internet) limitam endereços IP sem histórico de volume, portanto, você terá que criar uma reputação durante as primeiras semanas (o Marketo pode ajudar a orientá-lo).\
**Custo** - Geralmente, há uma cobrança adicional para enviar a partir de um IP dedicado com qualquer provedor.

**Vantagens e desvantagens de um IP compartilhado**

_Vantagens_

**Colegas de quarto bons** - Se as pessoas com quem você está compartilhando seu IP seguirem as práticas recomendadas de envio, você se beneficiará.\
**Frequência de endereçamento** - Não há uma frequência de endereçamento mínima necessária para se qualificar para um IP compartilhado, ao contrário dos IPs dedicados.\
**Custo** - Nunca há um encargo adicional a ser enviado de um IP Compartilhado.

_Contras_

**Colegas de quarto inválidos** - Se as pessoas com quem você está compartilhando seu IP se envolverem em práticas de envio ruins, suas campanhas de email poderão ser afetadas negativamente.\
**Controle** - Você tem muito menos controle sobre a reputação do remetente.\
**Resolução de Problemas** - Geralmente, pode ser mais difícil resolver um problema ao enviar de IPs Compartilhados.

>[!NOTE]
>
>Ao tomar uma decisão, há outro fator importante a ser considerado: o volume de envio. Se você planeja enviar menos de 100.000 emails por mês, ou menos de duas correspondências em um mês, você provavelmente não se beneficiará de um IP dedicado. O envio de números como esse é considerado baixo e seria difícil manter seu IP dedicado &quot;quente&quot; o suficiente para ser considerado seguro pelos principais ISPs. Basicamente, se você não enviar emails com a frequência suficiente, os ISPs verão uma correspondência como um &quot;surto&quot; súbito de atividade e poderão acabar bloqueando-a como suspeita de spam.

Se tiver dúvidas ou estiver interessado em configurar um IP dedicado, entre em contato com o representante de vendas da Marketo.
