---
unique-page-id: 2359467
description: Relatório de desempenho de email - Documentação do Marketo - Documentação do produto
title: Relatório de desempenho de email
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
feature: Email Programs
source-git-commit: 2cfb8381d3207efb00b7d4751e21244a188a411e
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 2%

---

# Relatório de desempenho de email {#email-performance-report}

Para ver o desempenho de seus emails com estatísticas como entregue, aberto, clicado etc., crie um Relatório de desempenho de email.

1. [Crie um Relatório em um Programa](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) e selecione o **Desempenho de Email** [Tipo de Relatório](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Altere o Intervalo de Tempo do Relatório](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) e clique na guia **Relatório**.
1. Você está aí! Agora explore o relatório para ver como seus emails se comportaram.

   >[!NOTE]
   >
   >O filtro Data de envio se baseia na primeira data em que o email foi enviado.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Clique no nome de um email para abri-lo no Pré-visualizador de email.

   >[!NOTE]
   >
   >Um relatório de desempenho de email inclui atividades para todas as pessoas, incluindo aquelas que foram excluídas desde que o email foi enviado. Às vezes, você deseja ver as atividades somente para pessoas ativas. Nesse caso, você precisa filtrar as pessoas excluídas do seu relatório. Use a guia **Lista Inteligente** para [criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para o relatório. Se você não estiver filtrando nenhum campo específico, defina o filtro de Endereço de Email como: **não está vazio**.

   [Selecione as Colunas do Relatório](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) para um relatório de Desempenho de Email:

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
    <td>Devolvido temporariamente</td>
    <td>O email foi rejeitado devido a uma condição temporária, como um servidor inativo ou uma caixa de entrada cheia.</td>
  </tr>
  <tr>
    <td>Pendente</td>
    <td>Esse número é calculado subtraindo o número de emails Delivered, Bounce e Soft Bounce do número total de Sent.</td>
  </tr>
  <tr>
    <td>Link clicado</td>
    <td>Número de destinatários de email que clicaram em um link no email.</td>
  </tr>
  <tr>
    <td>Inscrição cancelada</td>
    <td>Número de recipients do email que clicaram no link Cancelar inscrição no email e preencheram o formulário.</td>
  </tr>
  <tr>
    <td>Anulado(s)</td>
    <td>Número de emails que não puderam ser entregues e nenhum evento de devolução foi recebido. Um email é automaticamente chamado de Abortado se uma resposta não for recebida dentro de três dias do envio do email.</td>
  </tr>
</tbody></table>

>[!NOTE]
>
>Os links de cancelamento de inscrição e endereços de email clicados em um email não serão registrados em Links clicados no relatório.

Em geral, tentamos usar o senso comum para registrar essas estatísticas. Por exemplo, se alguém clicou em um link em um email, obviamente abriu o email primeiro. Seguimos estas regras específicas para o Relatório de desempenho de email:

* **Regra 1**: cada registro de atividade de email está definido como um, e somente como um, dos seguintes itens: _Entregues_, _Com rejeição permanente_, _Com rejeição temporária_ ou _Pendentes_.

* **Regra 2**: se o registro de email mostrar *Aberto*, será contado como *Entregue*.

* **Regra 3**: se o registro de email mostrar _Email Clicado_ ou _Cancelado_, ele será contado como _Entregue_ e _Aberto_.

* **Regra 4**: se o email estiver _Aberto_, as rejeições serão ignoradas. Se o email não tiver sido aberto, _Com rejeição permanente_ terá prioridade sobre _Com rejeição temporária_ e _Entregue_.

* **Regra 5**: se nenhuma atividade de email for recebida três dias após seu envio, ela será considerada _Anulada_.

>[!NOTE]
>
>* Vários envios da mesma campanha para a mesma pessoa são contados apenas uma vez.
>
>* Vários envios de campanhas diferentes para a mesma pessoa são contados separadamente.

>[!MORELIKETHIS]
>
>* [Filtrar Assets em Relatórios de email de campanha](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Relatório de desempenho do link de email](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)
