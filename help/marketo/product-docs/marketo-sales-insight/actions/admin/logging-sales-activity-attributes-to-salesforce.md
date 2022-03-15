---
description: Registrando atributos de atividade de vendas no Salesforce - Documentos da Marketo - Documentação do produto
title: Registrando atributos de atividade de vendas no Salesforce
hide: true
hidefromtoc: true
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 94f89e64b69d3997effe6736241a68f8314db1e6
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 24%

---

# Registrando atributos de atividade de vendas no Salesforce {#logging-sales-activity-attributes-to-salesforce}

O administrador do Salesforce pode adicionar manualmente campos de atividade personalizados ao Salesforce.

1. Em sua conta do Salesforce, clique em **Configuração**.

1. Procure por &quot;Campos personalizados de atividade&quot; no campo de pesquisa rápida e clique nele.

1. Clique em **Novo**.

1. Selecione Tipo de dados correspondente ao campo que deseja adicionar com base na tabela abaixo e clique em **Próximo**.

1. Insira o Nome do campo e o rótulo correspondentes ao campo que você deseja adicionar.

Descrição de cada coluna da tabela abaixo:

* **Rótulo do campo**: Nome do campo mostrado na interface do usuário (esse nome pode ser personalizado para melhorar a legibilidade pela sua equipe)
* **Nome do campo**: Nome técnico do campo (verifique se o Nome do campo inserido corresponde ao Nome do campo na tabela abaixo)
* **Nome da API**: Nome técnico do campo para API (verifique se o nome da API inserido corresponde ao nome da API na tabela abaixo)
* **Tipo de dados**: Tipo de campo
* **Tamanho**: Tamanho do campo de texto

<table>
 <tr>
  <th>Rótulo do campo</th>
  <th>Nome do campo</th>
  <th>Nome da API</th>
  <th>Tipo de dados</th>
  <th>Tamanho</th>
 </tr>
 <tr>
  <td>ID de presença local da chamada do Marketo Sales</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL da gravação da chamada do Marketo Sales</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Campanha do Marketo Sales</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Etapa atual da campanha do Marketo Sales</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL da campanha do Marketo Sales</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Anexo do e-mail do Marketo Sales visualizado</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed_c</td>
  <td>Caixa de seleção</td>
  <td></td>
 </tr>
 <tr>
  <td>Cliques em e-mail do Marketo Sales</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked_c</td>
  <td>Caixa de seleção</td>
  <td></td>
 </tr>
 <tr>
  <td>Respostas ao e-mail do Marketo Sales</td>
  <td>MSE_Replied</td>
  <td>MSE_Replied__c</td>
  <td>Caixa de seleção</td>
  <td></td>
 </tr>
 <tr>
  <td>Status do e-mail do Marketo Sales</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Texto</td>
  <td></td>
 </tr>
 <tr>
  <td>Modelo de e-mail do Marketo Sales</td>
  <td>MSE_Template</td>
  <td>MSE_Template_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL do modelo de e-mail do Marketo Sales</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>URL do e-mail do Marketo Sales</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>E-mail do Marketo Sales visualizado</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed_c</td>
  <td>Caixa de seleção</td>
  <td></td>
 </tr>
</table>
