---
unique-page-id: 4719294
description: Personalizar Atividade Sync - Documentos do Marketing - Documentação do produto
title: Personalizar Atividade Sync
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---


# Personalizar Atividade Sync {#customize-activities-sync}

Se você não usar o Marketing Insight de vendas, o Marketo poderá criar Registros de histórico de Atividade do Salesforce para determinados eventos. Aqui está como ativá-los.

1. Vá para **Admin**.

   ![](assets/admin.png)

1. Clique em **Salesforce** e, em seguida, clique em **Editar opções de sincronização**.

   ![](assets/two-1.png)

1. Marque as caixas ao lado das atividades que deseja que o Marketo envie para o Salesforce e clique em **Salvar**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Depois de habilitado, Marketo vai impulsionar três meses de história da atividade. Dependendo da quantidade de dados, _isso pode levar vários dias para ser concluído_. As atualizações que ocorrem durante o envio inicial do Atividade podem ser atrasadas até que a sincronização inicial do Atividade seja concluída.

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
   <td>Formulário preenchido</td> 
   <td>Preenchido qualquer formulário de marketing</td> 
  </tr> 
  <tr> 
   <td>Adicionado à lista</td> 
   <td><p>Etapa de fluxo: Foi adicionado a uma lista estática</p></td> 
  </tr> 
  <tr> 
   <td>Email enviado</td> 
   <td>Etapa de fluxo: Foi enviado um email</td> 
  </tr> 
  <tr> 
   <td>Email entregue</td> 
   <td>Recebido um email (não devolvido)</td> 
  </tr> 
  <tr> 
   <td>Email aberto</td> 
   <td>Aberto um email (sem bloquear imagens)</td> 
  </tr> 
  <tr> 
   <td>Link clicado no email</td> 
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
   <td>Email de vendas enviado</td> 
   <td>Foi enviado um email por meio do Marketing Insight de vendas</td> 
  </tr> 
  <tr> 
   <td>Email de vendas aberto</td> 
   <td>Aberto um email enviado por meio do Marketing Insight de vendas</td> 
  </tr> 
  <tr> 
   <td>Clique no link no email de vendas</td> 
   <td>Clicou em um link em um email enviado pelo Marketing Insight de vendas</td> 
  </tr> 
  <tr> 
   <td>E-mail de vendas recebido</td> 
   <td>Um email foi recebido e registrado pelo representante de vendas no Plug-in MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;Email de vendas recebido&quot; significa **não** entregue. O status entregue não é capturado para emails enviados via Sales Insight.

>[!TIP]
>
>Se você estiver interessado em obter mais informações sobre marketing no Salesforce, verifique nosso [produto Marketing to Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md).
