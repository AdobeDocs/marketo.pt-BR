---
unique-page-id: 14352480
description: Registro de resposta (SFDC) - Documentos do marketing - Documentação do produto
title: Registro de resposta (SFDC)
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# Registro de resposta (SFDC) {#reply-logging-sfdc}

O Sales Connect fornece a você a capacidade de registrar automaticamente as respostas dos prospectos no Salesforce. A estrutura que permite que você faça isso é baseada no nosso rastreamento de resposta por email. Se pudermos rastrear uma resposta do prospecto, podemos registrar essa resposta no Salesforce.

## Requisitos {#requirements}

* Deve estar registrando emails por meio do registro de API
* Deve ser possível rastrear [uma resposta](http://docs.marketo.com/x/BYPS)
* Deve estar conectado ao Salesforce
* Deve ter chamadas de API [Salesforce ](http://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) disponíveis

## Habilitar Registro de Resposta {#enable-reply-logging}

1. Para ativar o registro de respostas, você pode ir até a página [Configurações do Salesforce](http://docs.marketo.com/pages/assets/external-link.jspa). Depois que o registro em log da API for desligado, você verá a opção para marcar *Respostas de log.\
   *

   >[!NOTE]
   >
   >O registro de resposta segue as mesmas regras que você tem em vigor para o registro de emails enviados. Isso inclui como os e-mails são registrados; aos Clientes Potenciais e Contatos; quando existir um registro de duplicados; se nenhum registro correspondente for encontrado.

## Configuração do tipo para resposta no Salesforce {#setting-type-to-reply-in-salesforce}

É importante obter dados significativos de seus relatórios do Salesforce. Ter a capacidade de deixar o campo Tipo preenchido como &quot;Responder&quot; permite que você obtenha esses dados por meio de seus relatórios. Faça uma parceria com seu `Salesforce admin` para obter essa configuração.

1. Vá para **Configuração **> **Personalizar **> **Atividade **> **Campos de Tarefa**.
1. Clique em **Tipo**.
1. Em Valores da Lista de opções de tipo de Tarefa, clique em **Novo**.
1. Digite &quot;Reply&quot; na caixa vazia. Certifique-se de colocar a letra &#39;R&#39; em maiúsculas e clique em **Guardar**.

   >[!NOTE]
   >
   >Você não precisará selecionar um Padrão na lista de seleção Tipo. O Sales Connect verificará se esse Tipo de Atividade está disponível na instância do Salesforce e preencherá o campo tarefa nas atividades recebidas de acordo.

