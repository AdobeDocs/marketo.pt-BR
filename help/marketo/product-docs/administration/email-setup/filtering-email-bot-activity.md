---
description: Filtrar atividade de bot de email - Documentos do Marketo - Documentação do produto
title: Filtrar atividade de bot de email
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: 788084582a616b3cadd45f19d7a4779dad6f8c98
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 14%

---

# Filtrar atividade de bot de email {#filtering-email-bot-activity}

Às vezes, a atividade de bot de email pode aumentar erroneamente seus dados de aberturas e cliques de email. Siga as etapas abaixo para corrigir isso.

Usamos três métodos separados para confirmar a atividade de bot:

* Corresponder a [Lista de bots do Interative Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target="_blank"}: As atividades que correspondem a qualquer coisa na lista IAB UA/IP (Agente do usuário/endereço IP) serão marcadas como bots.
* Corresponder ao padrão de proximidade: Quando mais de duas atividades acontecem ao mesmo tempo (em menos de um segundo), elas são identificadas como bots. Os atributos considerados durante a comparação são:
   * ID de lead (deve ser a mesma)
   * Ativo de email (deve ser o mesmo)
   * Clique no link ou abra o email
   * Diferença de tempo (deve ser menor que um segundo)

Em relação ao clique em links de email e à atividade de abertura de email, os novos atributos serão preenchidos com os valores abaixo:

* As atividades identificadas como bots terão &quot;Atividade de bot&quot; como &quot;Verdadeiro&quot; e &quot;Padrão de atividade de bot&quot; como o padrão/método identificado
* As atividades identificadas como não bots terão &quot;Atividade de bot&quot; como &quot;Falso&quot; e &quot;Padrão de atividade de bot&quot; como &quot;N/A&quot;
* As atividades que ocorreram antes da introdução desses atributos terão &quot;Atividade de bot&quot; como &quot; (vazio) e &quot;Padrão de atividade de bot&quot; como &quot; &quot; (vazio)

## Selecionar tipo de filtro {#select-filter-type}

1. Clique em **Administrador**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Clique em **Email**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Clique no botão **Atividade de bot** guia .

   ![](assets/filtering-email-bot-activity-3.png)

1. Escolha para **Corresponder à Lista IAB**, **Corresponder ao padrão de proximidade** ou ambos. Escolha se deseja registrar a atividade bot _ou_ atividade de bot de filtro.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Se você escolher Filtrar atividade do robô, poderá ver uma queda em aberturas de email e cliques como atividades falsas esgotadas.

**ETAPA OPCIONAL**: Para desativar esse recurso, basta desmarcar os controle deslizantes. Se você desativar, os dados não serão redefinidos.

>[!TIP]
>
>Aproveite os dados de atividade de bot nas Smart Lists por meio do booleano &quot;Is Bot Activity&quot; (sim/não) e do &quot;Bot Activity Pattern&quot; nos filtros &quot;Clicked Link in Email&quot; e &quot;Open Email&quot; e dos acionadores &quot;Clicks Link in Email&quot; e &quot;Opens Email&quot;.

##  Lista de bloqueios IP {#ip-blocklist}

Compilamos uma lista de endereços IP responsáveis pela geração de milhões de envolvimentos falsos, pois esse engajamento recebido de qualquer um dos IPs a seguir é filtrado automaticamente e não adicionado à Instância do Marketo Engage. Isso pode resultar em uma redução de aberturas de email, cliques e outras atividades relacionadas. A lista abaixo pode ser atualizada periodicamente.

* 40.94.34.52
* 40.94.34.86
* 52.34.76.65
* 54.70.53.60
* 54.71.187.124
* 60.28.2.248
* 64.235.150.252
* 64.235.153.10
* 64.235.153.2
* 64.235.154.105
* 64.235.154.109
* 64.235.154.140
* 64.74.215.1
* 64.74.215.100
* 64.74.215.138
* 64.74.215.139
* 64.74.215.142
* 64.74.215.146
* 64.74.215.150
* 64.74.215.154
* 64.74.215.158
* 64.74.215.162
* 64.74.215.164
* 64.74.215.166
* 64.74.215.170
* 64.74.215.174
* 64.74.215.176
* 64.74.215.178
* 64.74.215.51
* 64.74.215.56
* 64.74.215.58
* 64.74.215.59
* 64.74.215.86
* 64.74.215.98
* 65.154.226.101
* 66.249.91.149
* 70.42.131.106
* 74.125.217.116
* 74.217.90.250
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
* 162.129.251.42
* 208.52.157.204
* 209.222.82.126
* 209.222.82.127
* 209.222.82.128
* 209.222.82.129
* 209.222.82.138
* 209.222.82.139
* 209.222.82.140
* 209.222.82.141
* 209.222.82.228
* 209.222.82.229
* 209.222.82.230
* 209.222.82.231
* 209.222.82.232
* 209.222.82.233
* 209.222.82.234
* 209.222.82.235

>[!NOTE]
>
>Analisamos e analisamos meticulosamente cada endereço IP antes de adicioná-lo a essa lista, garantindo que apenas os IPs mais críticos e prejudiciais sejam bloqueados.
