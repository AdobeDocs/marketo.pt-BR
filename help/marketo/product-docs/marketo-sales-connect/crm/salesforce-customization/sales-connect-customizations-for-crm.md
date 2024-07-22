---
unique-page-id: 14745793
description: Personalizações do Sales Connect para CRM - Documentação do Marketo - Documentação do produto
title: Personalizações do Sales Connect para CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Personalizações do Sales Connect para CRM {#sales-connect-customizations-for-crm}

Os campos e botões abaixo são criados pela API de metadados no Salesforce CRM. Depois que os campos forem criados, os administradores deverão configurar os layouts de página em seus CRMs para expô-los. As instruções podem ser encontradas [aqui](https://s3.amazonaws.com/tout-user-store/salesforce/assets/Marketo+Sales+Engage+For+Salesforce_+Installation+and+Success+Guide.pdf).

>[!NOTE]
>
>Isso afeta os clientes do ToutApp e do Sales Connect.

## Como instalar personalizações no Salesforce {#how-to-install-customizations-in-salesforce}

1. No Sales Connect, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/one.png)

1. Em Configurações do administrador, selecione **Salesforce**.

   ![](assets/two.png)

1. Clique em **Personalizações do Marketo Sales Connect**.

   ![](assets/three.png)

1. Clique em **Conectar ao Salesforce**.

   ![](assets/four.png)

1. Faça logon no Salesforce.

   ![](assets/five.png)

## Atualizar personalização do Salesforce {#update-salesforce-customization}

As atualizações do pacote de Personalização do Salesforce incluirão melhorias e correções de erros. Para verificar se há atualizações disponíveis ou para executar uma atualização, siga as etapas abaixo.

>[!NOTE]
>
>**Permissões de administrador necessárias.**

1. No [aplicativo Web](https://www.toutapp.com), clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/sales-connect-customizations-for-crm-6.png)

1. Em Configurações do administrador, clique em **Salesforce**.

   ![](assets/sales-connect-customizations-for-crm-7.png)

1. O cartão Personalização do Sales Connect mostrará se há atualizações disponíveis. Clique em **Atualizar Personalizações**.

   ![](assets/sales-connect-customizations-for-crm-8.png)

1. Clique em **Atualizar**.

   ![](assets/sales-connect-customizations-for-crm-9.png)

1. Aguarde a instalação das atualizações. Dependendo de quantos números de versão você precisa, o tempo de instalação varia.

   ![](assets/sales-connect-customizations-for-crm-10.png)

Depois de concluído, seu cartão mostrará &quot;Suas personalizações do Sales Connect estão atualizadas&quot;.

![](assets/sales-connect-customizations-for-crm-11.png)

## Campos de atividades personalizadas {#custom-activity-fields}

O Marketo detectará a criação de novos campos e então fará um preenchimento retroativo de dados único, um remapeamento e uma sincronização contínua de valores somente nos campos **novos**. Campos antigos não serão atualizados.

| **Nome do Campo** | **Descrição** |
|---|---|
| ID de presença local da chamada MSE | Como usuário, você pode escolher Presença local como opção ao fazer chamadas do telefone MSE. As chamadas recebidas mostrarão um número local para o receptor. |
| URL de Gravação de Chamada MSE | As chamadas podem ser gravadas e um link para a gravação será registrado aqui. |
| Campanha MSE | Registra o nome da campanha do MSE da qual o Contato/Cliente Potencial é membro. |
| URL da campanha MSE | Registra o URL da campanha que foi criada no MSE. Clicar nisso abrirá a campanha no aplicativo Web do MSE. |
| Etapa atual da campanha MSE | Se um contato/cliente potencial fizer parte de uma campanha, esse campo registrará o nome da etapa na qual o cliente potencial/contato está no momento. |
| Anexo de email do MSE exibido | Registra dados quando um email é enviado com um anexo e o anexo é visualizado pelo recipient. |
| Email MSE clicado | Registra uma marca de seleção quando o recipient clica em um link de um email. |
| Email do MSE respondido | Registra uma marca de seleção quando o destinatário responde a um email. |
| Status de email do MSE | Mostra se um email foi enviado/está em andamento/foi rejeitado (o rastreamento dos emails devolvidos depende do canal de delivery usado). |
| Modelo de email MSE | Registra o nome do modelo MSE que foi usado no email enviado ao lead/contato. |
| URL de modelo de email do MSE | Registra o URL do modelo que foi criado no MSE. Clicar nisso abrirá o modelo no aplicativo Web do MSE. |
| URL de email do MSE | Clicar nesse URL abrirá o Centro de comando no MSE e obterá a guia de histórico Exibição de detalhes de pessoas, onde você poderá ver o email enviado. |
| Email do MSE Exibido | Registra uma marca de seleção quando o destinatário visualiza um email. |

## Campos de Log de Roll-Up {#roll-up-logging-fields}

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
   <td>MSE - Último engajamento de marketing</td> 
   <td>Último envolvimento recebido de Marketing. </td> 
  </tr> 
  <tr> 
   <td>MSE - Última data de compromisso de marketing</td> 
   <td>Carimbo de data e hora do envolvimento do Marketing.</td> 
  </tr> 
  <tr> 
   <td>MSE - Última Descrição de Compromisso de Marketing</td> 
   <td>Descrição do compromisso.</td> 
  </tr> 
  <tr> 
   <td>MSE - Último Source de envolvimento de marketing</td> 
   <td>Source do envolvimento de marketing.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Último Tipo de Compromisso de Marketing</td> 
   <td colspan="1">Tipo de contrato.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última atividade por vendas<br></td> 
   <td colspan="1">Última atividade de saída executada pela equipe de vendas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Última Resposta</td> 
   <td colspan="1">Último email de resposta ao Email de vendas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Campanha de vendas atual</td> 
   <td colspan="1">Registra o nome da campanha do MSE da qual o lead/contato é membro.</td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Último contrato de vendas</td> 
   <td colspan="1">Último envolvimento recebido de Vendas. </td> 
  </tr> 
  <tr> 
   <td colspan="1">MSE - Recusa</td> 
   <td colspan="1">Campo de recusa.</td> 
  </tr> 
 </tbody> 
</table>

## Botões {#buttons}

| **Nome do Botão** | **Descrição** |
|---|---|
| Enviar Email MSE | Envie emails de Vendas do Salesforce. |
| Adicionar à campanha MSE | Adicionar às campanhas do MSE do Salesforce. |
| Encaminhar para o MSE | Contato por push do Salesforce para o MSE. |
| Chamar com MSE | Faça chamadas de vendas do Salesforce. |

## Botões de ação em massa {#bulk-action-buttons}

| **Nome do Botão** | **Descrição** |
|---|---|
| Adicionar à campanha MSE | Adicionar às campanhas do MSE do Salesforce. |
| Encaminhar para o MSE | Contato por push do Salesforce para o MSE. |

## Guias do usuário {#user-guides}

[Relatórios personalizados do MSE no Salesforce](https://docs.marketo.com/display/docs/assets/mse-custom-reports-in-sf.docx)

[MSE para Salesforce](https://docs.marketo.com/display/docs/assets/mse-for-sf-classic.pdf)

[MSE para Salesforce Lightning](https://s3.amazonaws.com/tout-user-store/salesforce/assets/SF+Guide+for+Lightning.pdf)
