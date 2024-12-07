---
unique-page-id: 14745793
description: Personalizações do Sales Connect para CRM - Documentação do Marketo - Documentação do produto
title: Personalizações do Sales Connect para CRM
exl-id: c7344ec2-a16b-48a1-8e39-1bbd2818db80
feature: Marketo Sales Connect
source-git-commit: dbf058714f6c4e6003c5a64d1048ac8a47931a0f
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 2%

---

# Personalizações do Sales Connect para CRM {#sales-connect-customizations-for-crm}

Os campos e botões abaixo são criados pela API de metadados no Salesforce CRM. Depois que os campos forem criados, os administradores deverão configurar os layouts de página em seus CRMs para expô-los. As instruções [podem ser encontradas aqui](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf).

## Como instalar personalizações no Salesforce {#how-to-install-customizations-in-salesforce}

1. No Sales Connect, clique no ícone de engrenagem e selecione **Configurações**.

   ![](assets/one.png)

1. Em Configurações do Administrador, selecione **Salesforce**.

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

1. Em Configurações do Administrador, clique em **Salesforce**.

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

<table><thead>
  <tr>
    <th>Nome do campo</th>
    <th>Descrição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>ID de presença local da chamada MSE</td>
    <td>Como usuário, você pode escolher Presença local como opção ao fazer chamadas do telefone MSE. As chamadas recebidas mostrarão um número local para o receptor.</td>
  </tr>
  <tr>
    <td>URL de Gravação de Chamada MSE</td>
    <td>As chamadas podem ser gravadas e um link para a gravação será registrado aqui.</td>
  </tr>
  <tr>
    <td>Campanha MSE</td>
    <td>Registra o nome da campanha do MSE da qual o Contato/Cliente Potencial é membro.</td>
  </tr>
  <tr>
    <td>URL da campanha MSE</td>
    <td>Registra o URL da campanha que foi criada no MSE. Clicar nisso abrirá a campanha no aplicativo Web do MSE.</td>
  </tr>
  <tr>
    <td>Etapa atual da campanha MSE</td>
    <td>Se um contato/cliente potencial fizer parte de uma campanha, esse campo registrará o nome da etapa na qual o cliente potencial/contato está no momento.</td>
  </tr>
  <tr>
    <td>Anexo de email do MSE exibido</td>
    <td>Registra dados quando um email é enviado com um anexo e o anexo é visualizado pelo recipient.</td>
  </tr>
  <tr>
    <td>Email MSE clicado</td>
    <td>Registra uma marca de seleção quando o recipient clica em um link de um email.</td>
  </tr>
  <tr>
    <td>Email do MSE respondido</td>
    <td>Registra uma marca de seleção quando o destinatário responde a um email.</td>
  </tr>
  <tr>
    <td>Status de email do MSE</td>
    <td>Mostra se um email foi enviado/está em andamento/foi rejeitado (o rastreamento dos emails devolvidos depende do canal de delivery usado).</td>
  </tr>
  <tr>
    <td>Modelo de email MSE</td>
    <td>Registra o nome do modelo MSE que foi usado no email enviado ao lead/contato.</td>
  </tr>
  <tr>
    <td>URL de modelo de email do MSE</td>
    <td>Registra o URL do modelo que foi criado no MSE. Clicar nisso abrirá o modelo no aplicativo Web do MSE.</td>
  </tr>
  <tr>
    <td>URL de email do MSE</td>
    <td>Clicar nesse URL abrirá o Centro de comando no MSE e obterá a guia de histórico Exibição de detalhes de pessoas, onde você poderá ver o email enviado.</td>
  </tr>
  <tr>
    <td>Email do MSE Exibido</td>
    <td>Registra uma marca de seleção quando o destinatário visualiza um email.</td>
  </tr>
</tbody></table>

## Campos de Log de Roll-Up {#roll-up-logging-fields}

<table><thead>
  <tr>
    <th>Nome do campo</th>
    <th>Descrição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MSE - Último engajamento de marketing</td>
    <td>Último envolvimento recebido de Marketing.</td>
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
    <td>MSE - Último Tipo de Compromisso de Marketing</td>
    <td>Tipo de contrato.</td>
  </tr>
  <tr>
    <td>MSE - Última atividade por vendas</td>
    <td>Última atividade de saída executada pela equipe de vendas.</td>
  </tr>
  <tr>
    <td>MSE - Última Resposta</td>
    <td>Último email de resposta ao Email de vendas.</td>
  </tr>
  <tr>
    <td>MSE - Campanha de vendas atual</td>
    <td>Registra o nome da campanha do MSE da qual o lead/contato é membro.</td>
  </tr>
  <tr>
    <td>MSE - Último contrato de vendas</td>
    <td>Último envolvimento recebido de Vendas.</td>
  </tr>
  <tr>
    <td>MSE - Recusa</td>
    <td>Campo de recusa.</td>
  </tr>
</tbody></table>

## Botões {#buttons}

<table><thead>
  <tr>
    <th>Nome do botão</th>
    <th>Descrição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Enviar Email MSE</td>
    <td>Envie emails de Vendas do Salesforce.</td>
  </tr>
  <tr>
    <td>Adicionar à campanha MSE</td>
    <td>Adicionar às campanhas do MSE do Salesforce.</td>
  </tr>
  <tr>
    <td>Encaminhar para o MSE</td>
    <td>Contato por push do Salesforce para o MSE.</td>
  </tr>
  <tr>
    <td>Chamar com MSE</td>
    <td>Faça chamadas de vendas do Salesforce.</td>
  </tr>
</tbody>
</table>

## Botões de ação em massa {#bulk-action-buttons}

<table><thead>
  <tr>
    <th>Nome do botão</th>
    <th>Descrição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Adicionar à campanha MSE</td>
    <td>Adicionar às campanhas do MSE do Salesforce.</td>
  </tr>
  <tr>
    <td>Encaminhar para o MSE</td>
    <td>Contato por push do Salesforce para o MSE.</td>
  </tr>
</tbody>
</table>

## Guias do usuário {#user-guides}

[Relatórios personalizados do MSE no Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/reports-and-dashboards.pdf)

[MSE para Salesforce Classic](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/mse-for-sf-classic.pdf)

[MSE para Salesforce Lightning](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/assets/sfdc-guide-lightning.pdf)
