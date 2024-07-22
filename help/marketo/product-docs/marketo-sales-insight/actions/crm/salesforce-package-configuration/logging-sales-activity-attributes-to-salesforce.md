---
description: Registrando atributos da atividade de vendas no Salesforce - Documentação do Marketo - Documentação do produto
title: Registrando Atributos de Atividade de Vendas no Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 29%

---

# Registrando Atributos de Atividade de Vendas no Salesforce {#logging-sales-activity-attributes-to-salesforce}

O administrador do Salesforce pode adicionar manualmente campos de atividade personalizados ao Salesforce.

1. Na sua conta do Salesforce, clique em **Configurar**.

1. Pesquise por &quot;Campos personalizados de atividade&quot; no campo de pesquisa rápida e clique nele.

1. Clique em **Novo**.

1. Selecione o Tipo de Dados correspondente ao campo que deseja adicionar com base na tabela abaixo e clique em **Avançar**.

1. Insira o Nome do campo e o rótulo correspondente ao campo que deseja adicionar.

Descrição de cada coluna da tabela abaixo:

* **Rótulo do campo**: nome do campo mostrado na interface do usuário (esse nome pode ser personalizado para melhorar a leitura pela sua equipe)
* **Nome do Campo**: nome técnico do campo (verifique se o Nome do Campo inserido corresponde ao Nome do Campo na tabela abaixo)
* **Nome da API**: nome técnico do campo da API (verifique se o nome da API inserido corresponde ao nome da API na tabela abaixo)
* **Tipo de dados**: tipo de campo
* **Tamanho**: tamanho do campo de texto

<table>
 <tr>
  <th>Rótulo do campo</th>
  <th>Nome do campo</th>
  <th>Nome da API</th>
  <th>Tipo de dados</th>
  <th>Tamanho</th>
 </tr>
  <tr>
  <td>Resultados da chamada</td>
  <td>mktosales_call_result</td>
  <td>mktosales_call_result_c</td>
  <td>Texto</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Motivos da chamada</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Texto</td>
  <td>50</td>
 </tr>
 <tr>
  <td>ID de presença local da chamada do Marketo Sales</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL da gravação da chamada do Marketo Sales</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Campanha do Marketo Sales</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign_c</td>
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
  <td>MSE_Clicked__c</td>
  <td>Caixa de seleção</td>
  <td></td>
 </tr>
 <tr>
  <td>Respostas ao e-mail do Marketo Sales</td>
  <td>MSE_Reply</td>
  <td>MSE_Reply__c</td>
  <td>Caixa de seleção</td>
  <td></td>
 </tr>
 <tr>
  <td>Status do e-mail do Marketo Sales</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status_c</td>
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
  <td>MSE_Details_c</td>
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
