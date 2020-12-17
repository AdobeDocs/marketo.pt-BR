---
unique-page-id: 14745793
description: Personalizações do Sales Connect para CRM - Documentos do Marketing - Documentação do produto
title: Personalizações do Sales Connect para CRM
translation-type: tm+mt
source-git-commit: 07ae1b3f3ee3e9d7f35373eea039d336bd786f97
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---


# Personalizações do Sales Connect para CRM {#sales-connect-customizations-for-crm}

Os campos e botões abaixo são criados pela API Metadados no Salesforce CRM. Depois que os campos são criados, os administradores devem configurar os layouts de página em seu CRM para expô-los. As instruções podem ser encontradas [aqui](http://docs.marketo.com/display/docs/assets/marketo-sales-engage-for-salesforce-installation-and-success-guide.pdf).

>[!NOTE]
>
>Isso afeta os clientes do ToutApp e do Sales Connect.

## Como instalar personalizações no Salesforce {#how-to-install-customizations-in-salesforce}

1. No Sales Connect, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/one.png)

1. Em Configurações administrativas, selecione **Salesforce**.

   ![](assets/two.png)

1. Clique em **Personalizações do Marketing Connect**.

   ![](assets/three.png)

1. Clique em **Conectar-se ao Salesforce**.

   ![](assets/four.png)

1. Faça logon no Salesforce.

   ![](assets/five.png)

## Campos de Atividade personalizados {#custom-activity-fields}

O Marketo detectará a criação dos novos campos e, em seguida, fará um preenchimento retroativo único de dados, um novo mapeamento e uma sincronização contínua de valores somente nos campos **new**. Os campos antigos não serão atualizados.

| **Nome do campo** | **Descrição** |
|---|---|
| ID de Presença Local da Chamada MSE | Como um usuário, você pode escolher Presença local como uma opção ao fazer chamadas do telefone MSE. As chamadas recebidas mostrarão um número local para o receptor. |
| URL de gravação de chamada MSE | As chamadas podem ser gravadas e um link para a gravação será registrado aqui. |
| Campanha MSE | Registra o nome da campanha MSE da qual o Contato/Cliente Potencial é membro. |
| URL de Campanha MSE | Registra o URL para a campanha criada no MSE. Clicar nisso abrirá a campanha no aplicativo da Web MSE. |
| Etapa atual da Campanha MSE | Se um contato/cliente potencial fizer parte de uma campanha, esse campo registrará o nome da etapa na qual o cliente potencial/contato está. |
| Anexo de email do MSE exibido | Registra dados quando um email é enviado com um anexo e o anexo é visualizado pelo recipient. |
| Email do MSE clicado | Registra uma marca de seleção quando o recipient clica em um link em um email. |
| Email do MSE Respondido | Registra uma marca de seleção quando o recipient responde a um email. |
| Status de email do MSE | Mostra se um email é enviado/em andamento/retornado (o rastreamento de emails retorcidos depende do canal de delivery usado). |
| Modelo de e-mail MSE | Registra o nome do modelo MSE usado no email enviado para o cliente potencial/contato. |
| URL do Modelo de Email do MSE | Registra o URL no modelo criado no MSE. Clicar nisso abrirá o modelo no aplicativo da Web MSE. |
| URL de email do MSE | Clicar neste URL abrirá o Centro de comando no MSE e puxa a guia do histórico de Visualizações de detalhes de pessoas, onde é possível visualizar o email enviado. |
| Email do MSE exibido | Registra uma marca de seleção quando o recipient visualização um email. |

## Campos de Registro de Roll-Up {#roll-up-logging-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Nome do campo</strong></td> 
   <td><strong>Descrição</strong></td> 
  </tr> 
  <tr> 
   <td>MSE - Último envolvimento de marketing</td> 
   <td>Último envolvimento recebido do Marketing. </td> 
  </tr> 
  <tr> 
   <td>MSE - Data do último envolvimento de marketing</td> 
   <td>Carimbo de data e hora do envolvimento da Marketing.</td> 
  </tr> 
  <tr> 
   <td>MSE - Desc do último envolvimento de marketing</td> 
   <td>Descrição do envolvimento.</td> 
  </tr> 
  <tr> 
   <td>MSE - Última fonte de envolvimento de marketing</td> 
   <td>Fonte do envolvimento da Marketing.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Último tipo de envolvimento de marketing</td> 
   <td colspan="1">Tipo de envolvimento.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última Atividade por Vendas<br></td> 
   <td colspan="1">Última atividade de saída realizada pela equipe de vendas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última resposta</td> 
   <td colspan="1">Última resposta por email ao email de vendas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Campanha de vendas atual</td> 
   <td colspan="1">Registra o nome da campanha MSE da qual o cliente potencial/contato é membro.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Último envolvimento de vendas</td> 
   <td colspan="1">Último envolvimento recebido de Vendas. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Opt out</td> 
   <td colspan="1">campo Recusar.</td> 
  </tr> 
 </tbody> 
</table>

## Botões {#buttons}

| **Nome do botão** | **Descrição** |
|---|---|
| Enviar email MSE | Enviar emails de vendas do Salesforce. |
| Adicionar à Campanha MSE | Adicionar às campanhas MSE do Salesforce. |
| Empurrar para MSE | Encaminhe o contato do Salesforce para o MSE. |
| Ligar para MSE | Efetuar chamadas de vendas do Salesforce. |

## Botões de ação em massa {#bulk-action-buttons}

| **Nome do botão** | **Descrição** |
|---|---|
| Adicionar à Campanha MSE | Adicionar às campanhas MSE do Salesforce. |
| Empurrar para MSE | Encaminhe o contato do Salesforce para o MSE. |

## Guias do usuário {#user-guides}

[Relatórios personalizados do MSE no Salesforce](http://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE para Salesforce](http://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE for Salesforce Lightning](http://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)

## Vídeos relacionados {#related-videos}

**Como instalar personalizações no Salesforce**
`<iframe width="630" height="470" src="//play.vidyard.com/YEPWYBfFEa4nKCo2F6bKKc.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>` ** A vantagem de usar personalizações no Salesforce** 
`<iframe width="630" height="470" src="//play.vidyard.com/4PzSDb6o8Qg8WbvBsq8wJD.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`