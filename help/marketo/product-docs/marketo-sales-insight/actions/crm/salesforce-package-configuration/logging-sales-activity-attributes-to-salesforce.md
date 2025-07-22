---
description: Registro dos atributos da atividade de vendas no Salesforce - Documentação do Marketo - Documentação do produto
title: Registrando Atributos de Atividade de Vendas no Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 10%

---

# Registrando Atributos de Atividade de Vendas em Log para [!DNL Salesforce] {#logging-sales-activity-attributes-to-salesforce}

O administrador do Salesforce pode adicionar manualmente campos de atividade personalizados a [!DNL Salesforce].

1. Na conta do [!DNL Salesforce], clique em **[!UICONTROL Instalação]**.

1. Pesquise por &quot;Campos personalizados de atividade&quot; no campo de pesquisa rápida e clique nele.

1. Clique em **[!UICONTROL Novo]**.

1. Selecione o Tipo de Dados correspondente ao campo que deseja adicionar com base na tabela abaixo e clique em **[!UICONTROL Avançar]**.

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
  <td>[!UICONTROL Resultados de Chamadas]</td>
  <td>mktosales_call_result</td>
  <td>mktosales_call_result_c</td>
  <td>Texto</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Motivos de chamada]</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Texto</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL ID de Presença Local de Chamada de Vendas do Marketo]</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL de Gravação de Chamada de Vendas do Marketo]</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Campanha de vendas do Marketo]</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Etapa Atual da Campanha de Vendas do Marketo]</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL da campanha de vendas do Marketo]</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Anexo de Email de Vendas do Marketo Exibido]</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed_c</td>
  <td>Caixa de seleção</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Email De Vendas Do Marketo Clicado]</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>Caixa de seleção</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Email de Vendas do Marketo Respondido]</td>
  <td>MSE_Reply</td>
  <td>MSE_Reply__c</td>
  <td>Caixa de seleção</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Status do Email de Vendas do Marketo]</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status_c</td>
  <td>Texto</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Modelo de email de vendas do Marketo]</td>
  <td>MSE_Template</td>
  <td>MSE_Template_c</td>
  <td>Texto</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL do Modelo de email de vendas do Marketo]</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL URL do email de vendas do Marketo]</td>
  <td>MSE_Details</td>
  <td>MSE_Details_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Email de Vendas do Marketo Exibido]</td>
  <td>MSE_Viewed</td>
  <td>MSE_Viewed_c</td>
  <td>Caixa de seleção</td>
  <td></td>
 </tr>
</table>
