---
unique-page-id: 4719294
description: Personalizar sincronização de atividades - Documentos do Marketo - Documentação do produto
title: Personalizar sincronização de atividades
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 12%

---

# Personalizar sincronização de atividades {#customize-activities-sync}

Se você não usar o Marketo Sales Insight, a Marketo poderá criar Registros do Histórico de Atividades do Salesforce para determinados eventos. Veja como habilitá-los.

1. Vá para **Admin**.

   ![](assets/admin.png)

1. Clique em **Salesforce** e em **Editar Opções de Sincronização**.

   ![](assets/two-1.png)

1. Marque as caixas ao lado das atividades que deseja que o Marketo envie para o Salesforce e clique em **Salvar**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Depois de habilitado, o Marketo enviará um histórico de atividades equivalente a três meses. Dependendo da quantidade de dados, _isso pode levar vários dias para ser concluído_. As atualizações que ocorrem durante o push inicial de Atividades podem ser adiadas até que a sincronização inicial de Atividades seja concluída.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>Tipo de atividade</th> 
   <th>Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Preencheu formulário</td> 
   <td>Preenchido qualquer formulário Marketo</td> 
  </tr> 
  <tr> 
   <td>Adicionado à lista</td> 
   <td><p>Etapa de fluxo: Foi adicionado a uma lista estática</p></td> 
  </tr> 
  <tr> 
   <td>E-mail enviado</td> 
   <td>Etapa de fluxo: Foi enviado um email</td> 
  </tr> 
  <tr> 
   <td>E-mail enviado</td> 
   <td>Recebido um email (não devolvido)</td> 
  </tr> 
  <tr> 
   <td>E-mail aberto</td> 
   <td>Aberto um email (sem bloquear imagens)</td> 
  </tr> 
  <tr> 
   <td>Clicou em link de e-mail</td> 
   <td>Clicou em um link em um email enviado pelo Marketo</td> 
  </tr> 
  <tr> 
   <td>Removido da lista</td> 
   <td>Etapa de fluxo: Foi removido de uma lista estática</td> 
  </tr> 
  <tr> 
   <td>Remover do fluxo</td> 
   <td>Etapa de fluxo: Remover do fluxo</td> 
  </tr> 
  <tr> 
   <td>E-mail de vendas enviado</td> 
   <td>Foi enviado um email por meio do Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-mail de vendas aberto</td> 
   <td>Aberto um email enviado pelo Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Clique no link no email de vendas</td> 
   <td>Clicou em um link em um email enviado pelo Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-mail de vendas recebido</td> 
   <td>Um email foi recebido e registrado pelo representante de vendas no plug-in MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;Email de vendas recebido&quot; significa **not** fornecido. O status do delivery não é capturado para emails enviados via Sales Insight.

>[!TIP]
>
>Se você estiver interessado em obter mais informações da Marketo no Salesforce, confira nosso produto [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md).
