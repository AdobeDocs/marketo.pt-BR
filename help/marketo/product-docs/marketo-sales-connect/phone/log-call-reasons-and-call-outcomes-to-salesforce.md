---
description: Registrar motivos da chamada e resultados da chamada no Salesforce - Documentação do Marketo - Documentação do produto
title: Registrar motivos da chamada e resultados da chamada para o Salesforce
exl-id: b35acdc2-8ec7-4dec-92b8-58ba7a1ad858
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# Registrar em log os motivos da chamada e seus resultados para [!DNL Salesforce] {#log-call-reasons-and-call-outcomes-to-salesforce}

Se você quiser registrar os resultados da chamada e os motivos da chamada para [!DNL Salesforce] para fins de relatório ou visibilidade, poderá criar um campo de atividade personalizado para cada um. Cada campo deve usar um Nome de API específico (conhecido como &quot;Nome do Campo&quot; em [!DNL Salesforce]).

* Nome do campo Resultados da chamada: mktosales_call_result
* Nome do Campo Motivos da Chamada: mktosales_call_reason

Para utilizar esses campos, primeiro será necessário criar o campo como um campo de atividade personalizado. Para torná-la visível aos usuários, será necessário adicioná-la ao layout da página do objeto da tarefa.

## [!DNL Salesforce] Classic {#salesforce-classic}

### Criar Campo de Atividade Personalizado no [!DNL Salesforce] Classic  {#create-custom-activity-field-in-salesforce-classic}

1. Em [!DNL Salesforce], clique em **[!UICONTROL Instalação]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-1.png)

1. Digite &quot;Atividades&quot; na caixa Localização rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-2.png)

1. Clique em **[!UICONTROL Campos Personalizados de Atividade]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-3.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-4.png)

1. Selecione o tipo de dados &quot;[!UICONTROL Texto]&quot; e clique em **[!UICONTROL Avançar]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-5.png)

1. Dê ao campo personalizado o nome do campo conforme definido acima. O comprimento do campo tem um limite de 255 caracteres. Rótulo de campo será o campo visível para sua equipe de vendas e pode ser personalizado para atender às necessidades de sua equipe.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-6.png)

1. O restante das configurações é opcional. Depois de concluir a configuração, clique em **[!UICONTROL Avançar]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-7.png)

1. Selecione as configurações de segurança em nível de campo desejadas para este campo e clique em **[!UICONTROL Avançar]** (a imagem abaixo é apenas um exemplo).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-8.png)

   >[!NOTE]
   >
   >Verifique se o campo personalizado está visível para o perfil que seus usuários do [!DNL Sales Connect] usam, juntamente com qualquer outro lugar em que você deseje que ele fique visível.

1. Selecione os layouts de página aos quais você deseja adicionar o campo e clique em **[!UICONTROL Salvar]** (opcionalmente, você pode clicar em **[!UICONTROL Salvar e novo]** e repetir o processo para o campo Motivo da chamada).

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-9.png)

### Adicionar Campo De Atividade Personalizado Ao Layout Da Página De Tarefas No [!DNL Salesforce] Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

>[!NOTE]
>
>Você só precisará seguir essas etapas se não tiver selecionado o layout de página desejado na Etapa 9 acima.

1. Em [!DNL Salesforce], clique em **[!UICONTROL Instalação]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-10.png)

1. Digite &quot;Tarefa&quot; na caixa Localização Rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-11.png)

1. Clique em **[!UICONTROL Layouts de Página de Tarefa]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-12.png)

1. Clique em **[!UICONTROL Editar]** ao lado do layout da página de tarefas à qual você deseja adicionar este campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-13.png)

1. Arraste e solte o campo até a seção desejada do layout da página Tarefa.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-14.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-15.png)

## [!DNL Salesforce] Relâmpago {#salesforce-lightning}

### Criar campo de atividade personalizado no [!DNL Salesforce] Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. Em [!DNL Salesforce], clique no ícone de engrenagem na parte superior direita e selecione **[!UICONTROL Instalação]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-16.png)

1. Clique em **[!UICONTROL Gerenciador de objetos]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-17.png)

1. Digite &quot;[!UICONTROL Atividade]&quot; na caixa Localização Rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-18.png)

1. Clique no rótulo **[!UICONTROL Atividade]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-19.png)

1. Clique em **[!UICONTROL Campos e Relações]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-20.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-21.png)

### Adicionar Campo de Atividade Personalizado ao Layout da Página de Tarefa no [!DNL Salesforce] Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

1. Em [!DNL Salesforce], clique no ícone de engrenagem na parte superior direita e selecione **[!UICONTROL Instalação]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-22.png)

1. Clique em **[!UICONTROL Gerenciador de objetos]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-23.png)

1. Digite &quot;[!UICONTROL Tarefa]&quot; na caixa Localização Rápida.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-24.png)

1. Clique no rótulo **[!UICONTROL Tarefa]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-25.png)

1. Clique em **[!UICONTROL Layouts de página]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-26.png)

1. Clique no layout da página de tarefas à qual deseja adicionar este campo.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-27.png)

1. Arraste e solte o campo até a seção desejada do layout da página Tarefa.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-28.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/log-call-reasons-and-call-outcomes-to-salesforce-29.png)

>[!MORELIKETHIS]
>
>[Instalar Campos de Evento do Sales Connect no Histórico de Atividades](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
