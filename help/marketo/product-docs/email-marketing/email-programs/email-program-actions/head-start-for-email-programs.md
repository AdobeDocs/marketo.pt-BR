---
unique-page-id: 10097202
description: Start principal para Programas de e-mail - Documentos do Marketing - Documentação do produto
title: Start principal para Programas de e-mail
translation-type: tm+mt
source-git-commit: 8d45a28e1c2adad3e04645f7150f1757414092f0
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---


# Start principal para Programas de e-mail {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Criar um Programa por email](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Quando você escolhe uma data/hora para um Programa de e-mail, isso determina quando o programa começará a processar. Se você quiser que seus e-mails sejam iniciados no horário selecionado, o Head Start oferece essa opção processando o programa antecipadamente.

## Start de cabeçalho padrão {#standard-head-start}

1. Clique em **Atividades de marketing**.

   ![](assets/one-1.png)

1. Localize e selecione seu Programa de email.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >O Start de cabeça não pode ser utilizado com o teste A/B.

1. No bloco Agendar, agende seu email e selecione a caixa **Start chefe**.

   ![](assets/three-1.png)

   Com a opção Cabeçalho Start selecionada, o programa começará a processar aproximadamente 12 horas antes do horário agendado. Após o processamento dos start, o programa é bloqueado.

   >[!CAUTION]
   >
   >Qualquer pessoa da sua audiência que se cancelar a inscrição após o bloqueio do programa ainda receberá o email. Recomendamos o ajuste da sua notificação de cancelamento de assinatura para refletir que as cancelar a assinatura podem levar de 1 a 2 dias úteis para serem processadas.

1. Clique em **Aprovar Programa**.

   ![](assets/four-1.png)

   Após a aprovação do programa, há quatro status diferentes que você pode ver no bloco Aprovação.

   * **Aguardando a execução:** Depois que o programa for aprovado.
   * **Processamento iniciado, aguardando execução:** Processamento em andamento.
   * **Processamento concluído, aguardando execução:** Processamento concluído, e-mail agora aguardando o horário agendado para inicialização.
   * **Concluído:** Programa concluído.

   >[!TIP]
   >
   >Deseja cancelar após o programa ser bloqueado, mas antes do envio do email? Sem problemas! Basta clicar em **Abortar Programa** no lado inferior direito do bloco Aprovação.

   >[!NOTE]
   >
   >Se você não aprovar seu programa de e-mail com menos de 12 horas antes do tempo de execução agendado, mas mudar de ideia, você precisará escolher uma nova data/hora que esteja pelo menos 12 horas antes de aprová-la.

## Start principal com fuso horário do Recipient {#head-start-with-recipient-time-zone}

A nossa característica de Start principal exige que o programa seja agendado com pelo menos 12 horas de antecedência. O que isso significa para o Fuso Horário do Recipient? Lembre-se de que, quando o Fuso horário do Recipient estiver ativo, será start executar o programa de e-mail à meia-noite no fuso horário mais antigo (UTC +14:00). Portanto, para habilitar **tanto** Start do cabeçalho quanto Fuso horário do Recipient, os programas precisam ser programados **pelo menos 12 horas antes do fuso horário mais antigo (UTC +14:00**.)

Isso significa que se você estiver na América/Los Angeles e quiser ativar o fuso horário dos Recipient e Start, você precisará agendar o programa **34 horas** antecipadamente. Como chegamos a esse número?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Saiba ](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) mais sobre como agendar programas de e-mail com fuso horário do Recipient.

>[!MORELIKETHIS]
>
>* [Agendar seu Programa de email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Agendar Programas de e-mail com fuso horário do Recipient](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Noções básicas sobre o fuso horário do Recipient](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

