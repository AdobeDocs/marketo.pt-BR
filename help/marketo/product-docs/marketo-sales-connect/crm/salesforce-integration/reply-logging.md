---
unique-page-id: 14352480
description: Registro de resposta (SFDC) - Documentos Marketo - Documentação do produto
title: Registro de resposta (SFDC)
exl-id: 11f84157-55b7-42a7-81d0-f5848adbb9f4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Registro de resposta (SFDC) {#reply-logging-sfdc}

O Sales Connect o capacita a registrar automaticamente as respostas de seus prospetos no Salesforce. A estrutura que permite fazer isso é baseada em nosso rastreamento de resposta de email. Se pudermos rastrear a resposta de um prospecto, podemos registrar essa resposta no Salesforce.

## Requisitos {#requirements}

* Deve registrar emails por meio do registro da API
* Deve ser capaz de [rastrear uma resposta](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Deve estar conectado ao Salesforce
* Deve ter o Salesforce [Chamadas de API](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) available

## Ativar o registro de respostas {#enable-reply-logging}

1. Para ativar o registro em log de resposta, você pode ir até a página de configurações do Salesforce . Quando o registro da API for desmarcado, você verá a opção para verificar _Respostas de Log_.

   >[!NOTE]
   >
   >O log de resposta segue as mesmas regras que você tem em vigor para registrar emails enviados. Isso inclui como os emails são registrados; aos Clientes Potenciais e Contatos; quando existir um registro duplicado; se nenhum registro correspondente for encontrado.

## Definir tipo como resposta no Salesforce {#setting-type-to-reply-in-salesforce}

Obter dados significativos de seus relatórios do Salesforce é importante. Ter a capacidade de deixar o campo Tipo preenchido como &quot;Resposta&quot; permite obter esses dados por meio de seus relatórios. Faça parceria com seu `Salesforce admin` para obter essa configuração.

1. Ir para **Configuração** > **Personalizar** > **Atividades** > **Campos de tarefa**.
1. Clique em **Tipo**.
1. Em Valores da Lista de Seleção de Tipo de Tarefa, clique em **Novo**.
1. Digite &quot;Reply&quot; na caixa vazia. Certifique-se de capitalizar o &#39;R&#39; e clique em **Salvar**.

   >[!NOTE]
   >
   >Não será necessário selecionar um Padrão na lista de opções Tipo. O Sales Connect verá que esse Tipo de atividade está disponível na instância do Salesforce e preencherá o campo de tarefa em suas atividades de entrada adequadamente.
