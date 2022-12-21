---
unique-page-id: 10097202
description: Primeiros passos para programas de email - Documentos do Marketo - Documentação do produto
title: Início do cabeçalho para programas de email
exl-id: f7c8b082-4d83-4e3b-8aa4-7b252e3dacd3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Início do cabeçalho para programas de email {#head-start-for-email-programs}

>[!PREREQUISITES]
>
>[Criar um programa de email](/help/marketo/product-docs/email-marketing/email-programs/creating-an-email-program/create-an-email-program.md)

Quando você escolhe uma data/hora para um Programa de email, determina quando o programa começará o processamento. Se você quiser que seus emails sejam iniciados no horário selecionado, Head Start lhe dará essa opção processando o programa antecipadamente.

## Início do Cabeçalho Padrão {#standard-head-start}

1. Clique em **Atividades de marketing**.

   ![](assets/one-1.png)

1. Localize e selecione seu Programa de email.

   ![](assets/selectemailprogram-4.jpg)

   >[!NOTE]
   >
   >Início do cabeçalho não pode ser usado com testes A/B.

1. No bloco Agendar , programe seu email e selecione o **Início da Cabeça** caixa.

   ![](assets/three-1.png)

   Com a opção Início do cabeçalho selecionada, o programa começará a processar aproximadamente 12 horas antes do horário programado. Quando o processamento começar, o programa será bloqueado.

   >[!CAUTION]
   >
   >Qualquer pessoa do seu público que cancelar a assinatura após o bloqueio de programa ainda receberá o email. Recomendamos o ajuste da sua notificação de cancelamento de subscrição para refletir que os cancelamentos de subscrição podem levar de 1 a 2 dias úteis para serem processados.

1. Clique em **Aprovar programa**.

   ![](assets/four-1.png)

   Após a aprovação do programa, há quatro status diferentes que você pode ver no bloco Aprovação .

   * **Aguardando execução:** Após a aprovação do programa.
   * **Processamento iniciado, aguardando execução:** O processamento está em andamento.
   * **Processamento concluído, aguardando execução:** Processamento concluído, o email agora aguarda o tempo agendado para inicialização.
   * **Concluído:** Programa concluído.

   >[!TIP]
   >
   >Deseja cancelar depois que o programa for bloqueado, mas antes que o email seja enviado? Sem problemas! Basta clicar em **Abortar programa** no lado inferior direito do bloco Aprovação.

   >[!NOTE]
   >
   >Se você cancelar a aprovação do seu programa de email com menos de 12 horas de antecedência em relação ao tempo de execução agendado, mas depois mudar de ideia, você precisará escolher uma nova data/hora com pelo menos 12 horas de antecedência em relação à aprovação.

## Início do Cabeçalho com Fuso Horário do Recipient {#head-start-with-recipient-time-zone}

A nossa funcionalidade de Início de Cabeça existente requer que o programa seja agendado com pelo menos 12 horas de antecedência. O que isso significa para Fuso horário do destinatário? Lembre-se de que quando o Fuso horário do destinatário estiver ativo, começamos a executar o programa de email à meia-noite no fuso horário mais antigo (UTC +14:00). Assim, para permitir **both** Fuso Horário de Início do Cabeçalho e do Recipient, os programas precisam ser agendados **pelo menos 12 horas antes do fuso horário mais antigo (UTC +14:00**.)

Isso significa que, se você estiver na América/Los Angeles e quiser ativar o Fuso Horário de Início e de Recipient, será necessário agendar o programa **34 horas** antecipadamente. Como chegamos a esse número?

![](assets/image2017-12-5-13-3a11-3a46.png)

[Saiba mais](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md) sobre como programar programas de email com Fuso horário do destinatário.

>[!MORELIKETHIS]
>
>* [Agendar seu programa de email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/schedule-your-email-program.md)
>* [Programar programas de e-mail com fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)
>* [Noções básicas sobre fuso horário do destinatário](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)

