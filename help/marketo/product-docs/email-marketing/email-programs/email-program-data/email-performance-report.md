---
unique-page-id: 2359467
description: Saiba como criar e usar o relatório de desempenho de email. Rastrear aberturas, cliques, rejeições e outras métricas de email.
title: Relatório de desempenho de emails
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 96%

---

# Relatório de desempenho de emails {#email-performance-report}

Para ver o desempenho de seus emails com estatísticas como entregue, aberto, clicado etc., crie um Relatório de desempenho de email.

1. [Crie um Relatório em um Programa](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) e selecione **[!UICONTROL Desempenho de email]** [Tipo de relatório](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Altere o intervalo de tempo do relatório](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) e clique na guia **[!UICONTROL Relatório]**.
1. É isso aí! Agora explore o relatório para ver como seus emails se comportaram.

   >[!NOTE]
   >
   >O filtro Data de envio se baseia na primeira data em que o email foi enviado.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Clique no nome de um email para abri-lo no pré-visualizador de emails.

   >[!NOTE]
   >
   >Um relatório de desempenho de email inclui atividades para todas as pessoas, incluindo aquelas que foram excluídas desde que o email foi enviado. Às vezes, você deseja ver as atividades somente para pessoas ativas. Nesse caso, você precisa filtrar as pessoas excluídas do seu relatório. Use a guia **[!UICONTROL Lista Inteligente]** para [criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para o relatório. Se você não estiver filtrando nenhum campo específico, defina o filtro de Endereço de Email como: **[!UICONTROL não está vazio]**.

   [Selecione Colunas do relatório](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) para que um relatório de desempenho de email inclua:

   <table><thead>

<tr>
    <th>Coluna</th>
    <th>Descrição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Devolvido permanentemente</td>
    <td>O email foi rejeitado devido a uma condição permanente, como endereço de email inexistente.</td>
  </tr>
  <tr>
    <td>Rejeitado temporariamente</td>
    <td>O email foi rejeitado devido a uma condição temporária, como um servidor inativo ou uma caixa de entrada cheia.</td>
  </tr>
  <tr>
    <td>Pendente</td>
    <td>Esse número é calculado subtraindo a quantidade de emails entregues, devolvidos e com erro temporário do número total de emails enviados.</td>
  </tr>
  <tr>
    <td>Link clicado</td>
    <td>Número de destinatários de email que clicaram em um link no email.</td>
  </tr>
  <tr>
    <td>Inscrição cancelada</td>
    <td>Número de destinatários de email que clicaram no link “Cancelar inscrição” no email e preencheram o formulário.</td>
  </tr>
  <tr>
    <td>Anulado</td>
    <td>Número de emails que não puderam ser entregues e nenhum evento de rejeição foi recebido. Um email é automaticamente indicado como Cancelado se uma resposta não for recebida dentro de três dias do envio do email.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>Os links de cancelamento de inscrição e endereços de email clicados em um email não serão registrados em Links clicados no relatório.

Em geral, tentamos usar o senso comum para registrar essas estatísticas. Por exemplo, se alguém clicou em um link em um email, obviamente abriu o email primeiro. Seguimos estas regras específicas para o Relatório de desempenho de emails:

* **Regra 1**: cada registro de atividade de email está definido como um, e somente como um, dos seguintes itens: _Entregue_, _Rejeição permanente_, _Rejeição temporária_ ou _Pendente_.

* **Regra 2**: se o registro de email mostrar _[!UICONTROL Aberto]_, será contado como _Entregue_.

* **Regra 3**: se o registro de email mostrar _[!UICONTROL Email clicado]_ ou _[!UICONTROL Inscrição cancelada]_, ele será contado como _Entregue_ e _Aberto_.

* **Regra 4**: se o email estiver _[!UICONTROL Aberto]_, as rejeições serão ignoradas. Se o email não tiver sido aberto, o status _Rejeição permanente_ terá prioridade sobre _Rejeição temporária_ e _Entregue_.

* **Regra 5**: se nenhuma atividade de email for recebida três dias após seu envio, ela será considerada _Cancelada_.

>[!NOTE]
>
>* Vários envios da mesma campanha para a mesma pessoa são contados apenas uma vez.
>
>* Vários envios de campanhas diferentes para a mesma pessoa são contados separadamente.

>[!MORELIKETHIS]
>
>* [Filtrar ativos em relatórios de emails de campanha](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md){target="_blank"}
>* [Filtrar registros excluídos/mesclados em um relatório de desempenho de emails](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-deleted-merged-records-email-performance-report.md){target="_blank"}
>* [Relatório de desempenho do link de email](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md){target="_blank"}
