---
unique-page-id: 2359467
description: Relatório de desempenho de email - Documentos do Marketo - Documentação do produto
title: Relatório de desempenho de email
exl-id: 327d4c0e-951f-4782-989d-4a4c6a513ebc
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 2%

---

# Relatório de desempenho de email {#email-performance-report}

Para ver o desempenho dos seus emails com estatísticas como entregues, abertas, clicadas, etc., crie um Relatório de desempenho de email.

1. [Criar um relatório em um programa](/help/marketo/product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) e selecione o **Desempenho de email** [Tipo de relatório](/help/marketo/product-docs/reporting/basic-reporting/report-types/report-type-overview.md).
1. [Alterar o intervalo de tempo do relatório](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) e clique no botão **Relatório** guia .
1. Você está aí! Agora explore o relatório para ver o desempenho dos seus emails.

   >[!NOTE]
   >
   >O filtro Data de envio baseia-se na primeira data em que o email foi enviado.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Clique no nome de um email para abri-lo no Visualizador de email.

   >[!NOTE]
   >
   >Um relatório de desempenho de email inclui atividades para todas as pessoas, incluindo aquelas que foram excluídas desde que o email foi enviado. Às vezes, você quer ver atividades apenas para pessoas ativas. Nesse caso, você precisa filtrar as pessoas excluídas do relatório. Use o **Lista inteligente** guia para [criar uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para o relatório. Se não estiver filtrando em nenhum campo específico, defina o filtro Endereço de email como: **não está vazio**.

   [Selecionar colunas de relatório](/help/marketo/product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) para um relatório de desempenho de email, inclua:

   | Coluna | Descrição |
   |---|---|
   | Devolvido permanentemente | O email foi rejeitado devido a uma condição permanente, como endereço de email inexistente. |
   | Devolvido temporariamente | O email foi rejeitado devido a uma condição temporária, como um servidor que estava inativo ou uma caixa de entrada completa. |
   | Pendente | Esse número é calculado subtraindo o número de emails Entregues, Rejeitados e Rejeitados Temporais do número total Enviados. |
   | Link clicado | Número de destinatários de email que clicaram em um link no email. |
   | Inscrição cancelada | Número de recipients do email que clicaram no **Cancelar inscrição** link no email e preencha o formulário. |

   >[!NOTE]
   >
   >Cancelar a assinatura de links e endereços de email que estão sendo clicados em um email não se registrará em Links clicados no relatório.

Em geral, tentamos usar o senso comum para registrar essas estatísticas. Por exemplo, se alguém clicou em um link em um email, obviamente ele abriu o email primeiro. Seguimos essas regras específicas para o Relatório de desempenho de email:

* **Regra 1**: Cada registro de atividade de email é definido como um, e apenas um, dos seguintes: _Entregue_, _Disparado intenso_, _Rejeitado Suave_ ou _Pending_.

* **Regra 2**: Se o registro de email mostrar *Aberto*, é contado como *Entregue*.

* **Artigo 3º**: Se o registro de email mostrar _Email clicado_ ou _Inscrições canceladas_, é contado como _Entregue_ e _Aberto_.

* **Artigo 4.o**: Se o email for _Aberto_, as rejeições são ignoradas. Se o email não tiver sido aberto, _Disparado intenso_ tem precedência sobre _Rejeitado Suave_ e _Entregue_.

>[!NOTE]
>
>Vários envios da mesma campanha para a mesma pessoa são contados apenas uma vez.

>[!MORELIKETHIS]
>
>* [Filtrar ativos em relatórios de email do Campaign](/help/marketo/product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Relatório de desempenho do link de email](/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-link-performance-report.md)

