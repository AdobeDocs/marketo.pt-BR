---
description: Motivos de chamada de registro e resultados de chamada para o Salesforce - Documentos da Marketo - Documentação do produto
title: Motivos de chamada de registro e resultados de chamada para o Salesforce
hide: true
hidefromtoc: true
source-git-commit: 1dd4a4f6bfac0b101f85f3776396aeef1a1f7182
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Motivos de chamada de registro e resultados de chamada para o Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Se você deseja registrar os resultados da chamada e chamar os motivos para o Salesforce para fins de relatório ou visibilidade, é possível criar um campo de atividade personalizado para cada um. Cada campo deve usar um nome de API específico.

* Nome da API de Resultados da Chamada: mktosales_call_result
* Nome da API dos Motivos da Chamada: mktosales_call_reason

Para utilizar esses campos, primeiro será necessário criar o campo como um campo de atividade personalizado. Para torná-lo visível para os usuários, será necessário adicioná-lo ao layout da página do objeto da tarefa.

## Criar campo de atividade personalizado no Salesforce Classic  {#create-custom-activity-field-in-salesforce-classic}

1. No Salesforce, vá para Setup.

PICC

1. Digite &quot;Atividades&quot; na caixa Localização rápida.

PICC

1. Clique em **Campos personalizados da atividade**.

PICC

1. Clique em **Novo**.

PICC

## Criar campo de atividade personalizado no Salesforce Lightning {#create-custom-activity-field-in-salesforce-lightning}

1. No Salesforce, clique no ícone de engrenagem na parte superior direita.

PICC

1. Clique em **Configuração**.

PICC

1. Clique em **Gerenciador de objetos**.

PICC

1. Insira Atividade na caixa Localização rápida e clique no rótulo Atividade para abrir a configuração do objeto.

PICC

1. No lado esquerdo, clique em **Campos e Relações**.

PICC

1. Clique em **Novo**.

PICC

## Adicionar campo de atividade personalizado ao layout da página de tarefa no Salesforce Classic {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

ETAPAS

## Adicionar campo de atividade personalizado ao layout da página de tarefa no Salesforce Lightning {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

ETAPAS

>[!MORELIKETHIS]
>
>[Instalar campos de evento do Sales Connect no histórico de atividades](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
