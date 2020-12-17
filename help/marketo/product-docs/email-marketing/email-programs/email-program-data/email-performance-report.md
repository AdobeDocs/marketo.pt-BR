---
unique-page-id: 2359467
description: Relatório de desempenho de e-mail - Documentos de marketing - Documentação do produto
title: Relatório de desempenho de email
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---


# Relatório de desempenho de email {#email-performance-report}

Para ver o desempenho de seus e-mails com estatísticas como entregues, abertas, clicadas etc., crie um Relatório de desempenho de e-mail.

1. [Crie um relatório em um ](../../../../product-docs/reporting/basic-reporting/creating-reports/create-a-report-in-a-program.md) programa e selecione o Tipo **de relatório** [Desempenho ](../../../../product-docs/reporting/basic-reporting/report-types/report-type-overview.md)de email.
1. [Altere o ](../../../../product-docs/reporting/basic-reporting/editing-reports/change-a-report-time-frame.md) Quadro de tempo do relatório e clique na guia  **** Relatório.
1. Você está aí! Agora, explore o relatório para ver como seus e-mails foram executados.

   >[!NOTE]
   >
   >O filtro Data de envio é baseado na primeira data em que o email foi enviado.

   ![](assets/email-performance-report.png)

   >[!TIP]
   >
   >Clique no nome de um email para abri-lo no Visualizador de email.

   >[!NOTE]
   >
   >
   >Um relatório de desempenho de email inclui atividades para todas as pessoas, incluindo aquelas que foram excluídas desde que o email foi enviado. Às vezes, você quer ver atividades somente para pessoas ativas. Nesse caso, é necessário filtrar as pessoas excluídas do seu relatório. Use a guia **Lista inteligente** para [criar uma lista inteligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) para o relatório. Se você não estiver filtrando em nenhum campo específico, defina o filtro Endereço de email como: **não está vazio**.

   [Selecionar ](../../../../product-docs/reporting/basic-reporting/editing-reports/select-report-columns.md) colunas de relatório para um relatório de desempenho de email incluem:

   | Coluna | Descrição |
   |---|---|
   | Disparado intenso | O email foi rejeitado devido a uma condição permanente, como endereço de email inexistente. |
   | Rejeitado macio | O email foi rejeitado devido a uma condição temporária, como um servidor que estava inativo ou uma caixa de entrada completa. |
   | Pendente | Esse número é calculado subtraindo o número de emails entregues, retorcidos e retorcidos suaves do número total de Enviados. |
   | Link clicado | Número de recipient de email que clicaram em um link no email. |
   | Inscrito | Número de recipient de e-mail que clicaram no link **Cancelar assinatura** no e-mail e preencheram o formulário. |

   >[!NOTE]
   >
   >Os links de cancelamento de assinatura e os endereços de email que estão sendo clicados em um email não se registram em Links clicados no relatório.

Em geral, tentamos usar o senso comum para registrar essas estatísticas. Por exemplo, se alguém clicou em um link em um email, obviamente eles abriram o email primeiro. Seguimos estas regras específicas para o Relatório de desempenho de email:

* **Regra 1**: Cada registro de atividade de email é definido como um dos seguintes:  *Entregues*,  *com salto* intenso,  *com salto suave* ou  *pendentes*.

* **Regra 2**: Se o registro de email mostrar  *Aberto*, ele será contado como  *Entregue*.

* **Regra 3**: Se o registro de e-mail mostrar  *Clicked* Emailor  *Unsubscription*, ele será contado como  ** Deliveredand  *Open (Entregue e aberto*).

* **Regra 4**: Se o email estiver  *aberto*, as rejeições serão ignoradas. Se o e-mail não foi aberto, *Ritmo Rígido* tem precedência sobre *Ritmo Comprado* e *Entregue*.

>[!NOTE]
>
>Vários envios da mesma campanha para a mesma pessoa são contados apenas uma vez.

>[!MORELIKETHIS]
>
>* [Filtrar ativos em relatórios de e-mail de Campanha](../../../../product-docs/reporting/basic-reporting/report-activity/filter-assets-in-a-campaign-email-reports.md)
>* [Relatório de desempenho do link de email](email-link-performance-report.md)

>



>[!NOTE]
>
>**Mergulho profundo**
>
>Saiba mais em [Relatórios básico](http://docs.marketo.com/display/docs/basic+reporting).

