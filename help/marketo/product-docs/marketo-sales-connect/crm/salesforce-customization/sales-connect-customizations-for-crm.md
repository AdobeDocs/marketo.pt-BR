---
unique-page-id: 14745793
description: Personalizações do Sales Connect para CRM - Documentos do Marketo - Documentação do produto
title: Personalizações de Conexão de Vendas para CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
source-git-commit: 94f89e64b69d3997effe6736241a68f8314db1e6
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 1%

---

# Personalizações de Conexão de Vendas para CRM {#sales-connect-customizations-for-crm}

Os campos e botões abaixo são criados pela API de metadados no Salesforce CRM. Depois que os campos são criados, os administradores devem configurar os layouts de página em seu CRM para expô-los. Instruções podem ser encontradas [here](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Isso afeta os clientes do ToutApp e do Sales Connect.

## Como instalar personalizações no Salesforce {#how-to-install-customizations-in-salesforce}

1. No Sales Connect, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/one.png)

1. Em Configurações de administração, selecione **Salesforce**.

   ![](assets/two.png)

1. Clique em **Personalizações do Marketo Sales Connect**.

   ![](assets/three.png)

1. Clique em **Conectar-se ao Salesforce**.

   ![](assets/four.png)

1. Faça logon no Salesforce.

   ![](assets/five.png)

## Atualizar Personalização Do Salesforce {#update-salesforce-customization}

As atualizações do pacote de Personalização do Salesforce incluirão melhorias e correções de erros. Para verificar se há atualizações disponíveis ou para executar uma atualização, siga as etapas abaixo.

>[!NOTE]
>
>**Permissões de administrador necessárias.**

1. No [aplicação web](https://www.toutapp.com), clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. Em Configurações de administração, clique em **Salesforce**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. O cartão Personalização da Conexão de Vendas mostrará se houver atualizações disponíveis. Clique em **Atualizar personalizações**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Clique em **Atualizar**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Aguarde a instalação das atualizações. Dependendo de quantos números de versão forem necessários, o tempo de instalação varia.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Depois de concluído, seu cartão mostrará &quot;Suas personalizações do Sales Connect estão atualizadas&quot;.

![](assets/sales-connect-customizations-for-crm-11.png)

## Campos de atividades personalizadas {#custom-activity-fields}

O Marketo detectará a criação dos novos campos e, em seguida, fará um preenchimento retroativo único de dados, um remapeamento e uma sincronização contínua de valores no **novo** somente campos. Campos antigos não serão atualizados.

| **Nome do campo** | **Descrição** |
|---|---|
| ID de Presença Local da Chamada MSE | Como usuário, você pode escolher Presença local como opção ao fazer chamadas do Telefone MSE. As chamadas recebidas mostrarão um número local para o receptor. |
| URL de gravação de chamada MSE | As chamadas podem ser registradas e um link para a gravação será registrado aqui. |
| Campanha MSE | Registra o nome da campanha MSE do qual o Contato/Cliente Potencial é membro. |
| URL da campanha MSE | Registra o URL da campanha criada no MSE. Clicar nisso abrirá a campanha no aplicativo da Web MSE. |
| Etapa atual da campanha MSE | Se um contato/lead fizer parte de uma campanha, esse campo registrará o nome da etapa na qual o lead/contato está no momento. |
| Anexo de email do MSE exibido | Registra dados quando um email é enviado com um anexo e o anexo é visualizado pelo recipient. |
| MSE Email Clicado | Registra uma marca de seleção quando o recipient clica em um link em um email. |
| MSE Email Respondido | Registra uma marca de seleção quando o recipient responde a um email. |
| Status do Email MSE | Mostra se um email é enviado/em andamento/devolvido (o rastreamento de emails devolvidos depende do canal de delivery usado). |
| Modelo de Email MSE | Registra o nome do modelo MSE usado no email enviado para o cliente potencial/contato. |
| URL de Modelo de Email do MSE | Registra o URL para o modelo criado no MSE. Clicar nisso abrirá o modelo no aplicativo Web MSE. |
| URL de Email do MSE | Clicar nesse URL abrirá o Centro de comando no MSE e puxará a guia Histórico da Exibição de detalhes das pessoas, onde é possível visualizar o email enviado. |
| Email do MSE exibido | Registra uma marca de verificação quando o recipient exibe um email. |

## Campos de registro de rollup {#roll-up-logging-fields}

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
   <td>MSE - Último compromisso de marketing</td> 
   <td>Último engajamento recebido da Marketing Cloud. </td> 
  </tr> 
  <tr> 
   <td>MSE - Data do último compromisso de marketing</td> 
   <td>Carimbo de data e hora do envolvimento do Marketing.</td> 
  </tr> 
  <tr> 
   <td>MSE - Desc do último compromisso de marketing</td> 
   <td>Descrição do envolvimento.</td> 
  </tr> 
  <tr> 
   <td>MSE - Última fonte de envolvimento de marketing</td> 
   <td>Fonte do envolvimento de Marketing.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Último tipo de envolvimento de marketing</td> 
   <td colspan="1">Tipo de envolvimento.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última Atividade por Vendas<br></td> 
   <td colspan="1">Última atividade de saída realizada pela equipe de Vendas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última resposta</td> 
   <td colspan="1">Última resposta de email ao email de Vendas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Campanha de Vendas Atual</td> 
   <td colspan="1">Registra o nome da campanha MSE do qual o cliente potencial/contato é membro.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Último compromisso de vendas</td> 
   <td colspan="1">Último engajamento recebido de Vendas. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Recusar</td> 
   <td colspan="1">Campo de rejeição.</td> 
  </tr> 
 </tbody> 
</table>

## Botões {#buttons}

| **Nome do botão** | **Descrição** |
|---|---|
| Enviar Email MSE | Enviar emails de vendas do Salesforce. |
| Adicionar à Campanha MSE | Adicione às campanhas MSE do Salesforce. |
| Encaminhar para MSE | Encaminhe o contato do Salesforce para o MSE. |
| Chame com MSE | Efetuar chamadas de vendas do Salesforce. |

## Botões de ação em massa {#bulk-action-buttons}

| **Nome do botão** | **Descrição** |
|---|---|
| Adicionar à Campanha MSE | Adicione às campanhas MSE do Salesforce. |
| Encaminhar para MSE | Encaminhe o contato do Salesforce para o MSE. |

## Guias do usuário {#user-guides}

[Relatórios personalizados do MSE no Salesforce](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE para Salesforce](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE para o Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
