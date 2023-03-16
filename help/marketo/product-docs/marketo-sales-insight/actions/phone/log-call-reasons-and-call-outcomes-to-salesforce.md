---
description: Motivos de chamada de registro e resultados de chamada para o Salesforce - Documentos da Marketo - Documentação do produto
title: Motivos de chamada de registro e resultados de chamada para o Salesforce
source-git-commit: 0864f784d193bfc6dd7a087c9f89ce59bdff710c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Motivos de chamada de registro e resultados de chamada para o Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Se você deseja registrar os resultados da chamada e chamar os motivos para o Salesforce para fins de relatório ou visibilidade, é possível criar um campo de atividade personalizado para cada um. Cada campo deve usar um Nome de API específico (conhecido como &quot;Nome de campo&quot; no Salesforce).

* Nome do Campo de Resultados da Chamada: mktosales_call_result
* Nome do campo Motivos da chamada: mktosales_call_reason

Para utilizar esses campos, primeiro será necessário criar o campo como um campo de atividade personalizado. Para torná-lo visível para os usuários, será necessário adicioná-lo ao layout da página do objeto da tarefa.

## Salesforce Classic {#salesforce-classic}

### Criar campo de atividade personalizado no Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. No Salesforce, clique em **Configuração**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Digite &quot;Atividades&quot; na caixa Localização rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Clique em **Campos personalizados da atividade**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Clique em **Novo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Selecione o tipo de dados &quot;Texto&quot; e clique em **Próximo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Forneça ao campo personalizado o nome do campo conforme definido acima. O comprimento do campo tem um limite de 255 caracteres. O Rótulo do campo será o campo visível para a sua equipe de vendas e poderá ser personalizado para atender às necessidades da sua equipe.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. O restante das configurações são opcionais. Após concluir a configuração, clique em **Próximo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Selecione as configurações de segurança de nível de campo desejadas para este campo e clique em **Próximo** (a imagem abaixo é apenas um exemplo).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Certifique-se de que o campo personalizado esteja visível para o perfil que seus usuários utilizam das Ações de insight de vendas, juntamente com qualquer outro lugar que você gostaria que ele ficasse visível.

1. Selecione os layouts de página aos quais você deseja adicionar o campo e clique em **Salvar** (opcionalmente, você pode clicar em **Salvar e Novo** e repita o processo para o campo Motivo da chamada ).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Adicionar campo de atividade personalizado ao layout da página de tarefa no Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Você só precisará seguir essas etapas se não tiver selecionado o layout de página desejado na Etapa 9 acima.

1. No Salesforce, clique em **Configuração**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Digite &quot;Tarefa&quot; na caixa Localização rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Clique em **Layouts da Página de Tarefas**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Clique em **Editar** ao lado do layout da página da tarefa, você deseja adicionar este campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Arraste e solte o campo até a seção desejada do layout da página Tarefa.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Clique em **Salvar**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## Salesforce Lightning {#salesforce-lightning}

### Criar campo de atividade personalizado no Salesforce Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. No Salesforce, clique no ícone de engrenagem na parte superior direita e selecione **Configuração**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Clique em **Gerenciador de objetos**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Digite &quot;Atividade&quot; na caixa Localização rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Clique no botão **Atividade** rótulo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Clique em **Campos e Relações**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Clique em **Novo**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Adicionar campo de atividade personalizado ao layout da página de tarefa no Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. No Salesforce, clique no ícone de engrenagem na parte superior direita e selecione **Configuração**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Clique em **Gerenciador de objetos**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Digite &quot;Tarefa&quot; na caixa Localização rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Clique no botão **Tarefa** rótulo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Clique em **Layouts de página**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Clique no layout da página da tarefa à qual deseja adicionar este campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Arraste e solte o campo até a seção desejada do layout da página Tarefa.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Clique em **Salvar**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>* [Resultados da chamada](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-outcomes.md)
>* [Motivos da chamada](/help/marketo/product-docs/marketo-sales-insight/actions/phone/call-reasons.md)

