---
unique-page-id: 4719294
description: Personalizar sincronização de atividades - Documentação do Marketo - Documentação do produto
title: Personalizar sincronização de atividades
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 12%

---

# Personalizar sincronização de atividades {#customize-activities-sync}

Se você não usar o Marketo Sales Insight, o Marketo Engage poderá criar registros do histórico de atividades do Salesforce para determinados eventos. Veja como ativá-los.

1. Vá para **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Clique em **[!DNL Salesforce]** e em **[!UICONTROL Editar Opções de Sincronização]**.

   ![](assets/two-1.png)

1. Marque as caixas ao lado das atividades que você deseja que o Marketo envie para o Salesforce e clique em **[!UICONTROL Salvar]**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Depois de habilitado, o Marketo enviará o histórico de atividades correspondente a três meses. Dependendo da quantidade de dados, _a conclusão pode demorar vários dias_. As atualizações que ocorrem durante o push inicial de Atividades podem ser atrasadas até que a sincronização inicial de Atividades seja concluída.

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
   <td>Preencheu qualquer formulário do Marketo</td> 
  </tr> 
  <tr> 
   <td>Adicionado à lista</td> 
   <td><p>Etapa de fluxo: foi adicionado a uma lista estática</p></td> 
  </tr> 
  <tr> 
   <td>E-mail enviado</td> 
   <td>Etapa de fluxo: email enviado</td> 
  </tr> 
  <tr> 
   <td>E-mail enviado</td> 
   <td>Recebeu um email (não rejeitado)</td> 
  </tr> 
  <tr> 
   <td>E-mail aberto</td> 
   <td>Abertura de um email (sem bloqueio de imagens)</td> 
  </tr> 
  <tr> 
   <td>Clicou em link de e-mail</td> 
   <td>Clicou em um link em um email enviado pelo Marketo</td> 
  </tr> 
  <tr> 
   <td>Removido da lista</td> 
   <td>Etapa de fluxo: foi removido de uma lista estática</td> 
  </tr> 
  <tr> 
   <td>Remover do fluxo</td> 
   <td>Etapa de fluxo: Remover do fluxo</td> 
  </tr> 
  <tr> 
   <td>E-mail de vendas enviado</td> 
   <td>Recebeu um email por meio do Marketo Sales Insight</td> 
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
>&quot;Email de vendas recebido&quot; _não_ significa entregue. O status de Entregue não é capturado para emails enviados pelo Sales Insight.

>[!TIP]
>
>Se você estiver interessado em obter mais informações do Marketo no Salesforce, confira nosso produto [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
