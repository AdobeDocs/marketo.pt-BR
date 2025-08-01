---
description: Registro de respostas - Documentação do Marketo - Documentação do produto
title: Registro de respostas
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Registro de respostas {#reply-logging}

As Ações de Vendas do Insight oferecem a você a capacidade de registrar automaticamente as respostas de seus clientes potenciais em [!DNL Salesforce]. A estrutura que permite fazer isso se baseia no rastreamento de respostas por email. Se pudermos acompanhar a resposta de um cliente potencial, podemos registrar essa resposta em [!DNL Salesforce].

## Requisitos {#requirements}

* Deve registrar emails por meio do registro da API
* Deve poder [rastrear uma resposta](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* Deve estar conectado a [!DNL Salesforce]
* Deve ter [!DNL Salesforce] [chamadas de API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) disponíveis

## Ativar o registro de respostas {#enable-reply-logging}

1. Para habilitar o log de respostas, você pode ir para a página de configurações do [!DNL Salesforce]. Depois que o log da API for desmarcado, você verá a opção para verificar _Registrar Respostas_.

   >[!NOTE]
   >
   >O registro de respostas segue as mesmas regras que você tem em vigor para registrar emails enviados. Isso inclui como os emails são registrados; em clientes potenciais e contatos; quando há um registro duplicado; se nenhum registro correspondente for encontrado.

## Definindo Tipo para Resposta em [!DNL Salesforce] {#setting-type-to-reply-in-salesforce}

É importante obter dados significativos de seus relatórios do [!DNL Salesforce]. Ter a capacidade de ter o campo Tipo preenchido como &quot;Resposta&quot; permite que você obtenha esses dados por meio de seus relatórios. Faça parceria com o `[!DNL Salesforce] admin` para obter essa configuração.

1. Vá para **[!UICONTROL Configuração]** > **[!UICONTROL Personalizar]** > **[!UICONTROL Atividades]** > **[!UICONTROL Campos de Tarefa]**.
1. Clique em **[!UICONTROL Tipo]**.
1. Em [!UICONTROL Valores da Lista de Escolha de Tipo de Tarefa], clique em **[!UICONTROL Novo]**.
1. Digite &quot;Responder&quot; na caixa vazia. Certifique-se de colocar &#39;R&#39; em maiúsculas e clique em **[!UICONTROL Salvar]**.

   >[!NOTE]
   >
   >Não será necessário selecionar um Padrão na lista de opções Tipo. [!DNL Sales Insight Actions] verá que esse Tipo de atividade está disponível em sua instância [!DNL Salesforce] e preencherá o campo de tarefa em suas atividades de entrada adequadamente.
