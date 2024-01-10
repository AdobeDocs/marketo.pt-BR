---
description: Atividade de filtragem de bot por email - Documentação do Marketo - Documentação do produto
title: Filtrar atividade de bot por email
hide: true
hidefromtoc: true
feature: Email Setup
source-git-commit: d635fbd4807890266429d4a257cf7d6588736bb5
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Filtragem da atividade TEMP de bot por email{#filtering-email-bot-activity}

Às vezes, a atividade de bot por email pode inflar erroneamente seus dados de aberturas e cliques de email. Siga as etapas abaixo para corrigir isso.

Usamos dois métodos separados para confirmar a atividade do bot:

* Corresponder com [Lista de bot do Interative Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target="_blank"}: atividades que correspondem a qualquer item na lista UA/IP (Agente do usuário/endereço IP) do IAB serão marcadas como bots.
* Correspondência com o padrão de proximidade: quando mais de duas atividades acontecem ao mesmo tempo (em menos de um segundo), elas são identificadas como bots. Os atributos considerados durante a comparação são:
   * ID do lead (deve ser o mesmo)
   * Ativo de email (deve ser o mesmo)
   * Clique em links ou e-mail aberto
   * Diferença de tempo (deve ser menor que um segundo)

Em relação à atividade de clique em links de email e abertura de email, novos atributos serão preenchidos com os valores abaixo:

* As atividades identificadas como bots terão &quot;Atividade de bot&quot; como &quot;True&quot; e &quot;Padrão de atividade de bot&quot; como o padrão/método identificado
* As atividades identificadas como não bots terão &quot;Atividade de bot&quot; como &quot;Falso&quot; e &quot;Padrão de atividade de bot&quot; como &quot;N/A&quot;
* As atividades que ocorreram antes da introdução desses atributos terão &quot;Atividade de bot&quot; como &quot; &quot; (vazio) e &quot;Padrão de atividade de bot&quot; como &quot; &quot; (vazio)

## Selecionar tipo de filtro {#select-filter-type}

1. Clique em **[!UICONTROL Admin]**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Clique em **[!UICONTROL E-mail]**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Clique em **[!UICONTROL Atividade de bot]** guia.

   ![](assets/filtering-email-bot-activity-3.png)

1. Optar por **[!UICONTROL Corresponder com Lista IAB]**, **[!UICONTROL Corresponder com Padrão de Proximidade]**, ou ambos. Escolha se deseja [!UICONTROL registrar atividade de bot] _ou_ [!UICONTROL filtrar atividade de bot]. Definir a quantidade de segundos para **Duração entre atividades** de 0 a 3 segundos de duração (o padrão é 0).

   ![](assets/filtering-email-bot-activity-temp-4.png)

>[!NOTE]
>
>Com **Duração entre atividades** definido como 0 segundos, identificaremos as atividades de email que estão ocorrendo exatamente no mesmo segundo. Se várias atividades de email ocorrerem dentro da quantidade designada de segundos, elas serão identificadas como atividade de bot.

>[!NOTE]
>
>* Se você escolher [!UICONTROL Filtrar atividade de bot], você poderá ver uma queda nas aberturas e cliques no email, à medida que as atividades falsas forem eliminadas.

**ETAPA OPCIONAL**: para desativar esse recurso, basta desmarcar os controles deslizantes. Se você desativar, os dados não serão redefinidos.

>[!TIP]
>
>Aproveite os dados de atividade de bot nas Smart Lists por meio das opções &quot;Is Bot Activity&quot; (sim/não) e &quot;Bot Activity Pattern&quot; nos filtros &quot;Link clicado no email&quot; e &quot;Abrir email&quot;, e &quot;Clicks Link no email&quot; e &quot;Abrir email&quot; acionadores.

## INCLUIR NA LISTA DE BLOQUEIOS IP {#ip-blocklist}

Compilamos uma lista de endereços IP responsáveis por gerar milhões de engajamentos falsos, já que esse engajamento recebido de qualquer um dos seguintes IPs é automaticamente filtrado e não adicionado à instância do Marketo Engage. Isso pode resultar em uma redução nas aberturas de email, cliques e outras atividades relacionadas. A lista a seguir apresentada pode ser atualizada periodicamente.

* 40.94.34.52
* 40.94.34.86
* 52.34.76.65
* 54.70.53.60
* 54 71 187 124
* 60.28.2.248
* 64 235 150 252
* 64 235 153 10
* 64 235 153 2
* 64 235 154 105
* 64 235 154 109
* 64 235 154 140
* 64.74.215.1
* 64 74 215 100
* 64 74 215 138
* 64 74 215 139
* 64 74 215 142
* 64 74 215 146
* 64.74.215.150
* 64 74 215 154
* 64 74 215 158
* 64 74 215 162
* 64 74 215 164
* 64 74 215 166
* 64.74.215.170
* 64 74 215 174
* 64 74 215 176
* 64.74.215.178
* 64 74 215 51
* 64 74 215 56
* 64 74 215 58
* 64.74.215,59
* 64 74 215 86
* 64.74.215.98
* 65 154 226 101
* 66 249 91 149
* 70.42.131.106
* 74 125 217 116
* 74 217 90 250
* 104.129.41.4
* 104.47.55.126
* 104.47.58.126
* 104.47.70.126
* 104.47.73.126
* 104.47.73.254
* 104.47.74.126
* 128.220.160.1
* 155.70.39.101
* 162.129.251.14
* 162 129 251 42
* 208.52.157.204

>[!NOTE]
>
>Analisamos e examinamos meticulosamente cada endereço IP antes de adicioná-lo a esta lista, garantindo que apenas os IPs mais críticos e prejudiciais sejam bloqueados.
