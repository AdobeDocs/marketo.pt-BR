---
description: Filtrar atividade de bot de email - Documentos do Marketo - Documentação do produto
title: Filtrar atividade de bot de email
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: f5a4fa76510cc70fe5b4746d58c6e0d4daf93a72
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Filtrar atividade de bot de email {#filtering-email-bot-activity}

Às vezes, a atividade de bot de email pode aumentar erroneamente seus dados de aberturas e cliques de email. Siga as etapas abaixo para corrigir isso.

Usamos três métodos separados para confirmar a atividade de bot:

* Corresponder a [Lista de bots do Interative Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target=&quot;_blank&quot;}: As atividades que correspondem a qualquer coisa na lista IAB UA/IP (Agente do usuário/endereço IP) serão marcadas como bots.
* Corresponder ao padrão de proximidade: Quando mais de duas atividades acontecem ao mesmo tempo (em menos de um segundo), elas são identificadas como bots. Os atributos considerados durante a comparação são:
   * ID de lead (deve ser a mesma)
   * Ativo de email (deve ser o mesmo)
   * Clique no link ou abra o email
   * Diferença de tempo (deve ser menor que um segundo)

Em relação ao clique em links de email e à atividade de abertura de email, os novos atributos serão preenchidos com os valores abaixo:

* As atividades identificadas como bots terão &quot;Atividade de bot&quot; como &quot;Verdadeiro&quot; e &quot;Padrão de atividade de bot&quot; como o padrão/método identificado
* As atividades identificadas como não bots terão &quot;Atividade de bot&quot; como &quot;Falso&quot; e &quot;Padrão de atividade de bot&quot; como &quot;N/A&quot;
* As atividades que ocorreram antes da introdução desses atributos terão &quot;Atividade de bot&quot; como &quot; (vazio) e &quot;Padrão de atividade de bot&quot; como &quot; &quot; (vazio)

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
