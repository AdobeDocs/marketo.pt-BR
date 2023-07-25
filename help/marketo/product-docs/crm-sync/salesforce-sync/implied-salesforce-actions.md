---
unique-page-id: 4719304
description: Ações Implícitas Do Salesforce - Documentação Do Marketo - Documentação Do Produto
title: Ações implícitas do Salesforce
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 21%

---

# Ações implícitas do Salesforce {#implied-salesforce-actions}

Quando uma etapa de fluxo específica do Salesforce é executada, às vezes etapas adicionais são executadas automaticamente. Estas são as regras, então você sabe:

Estas regras serão aplicadas _quando a pessoa não estiver atualmente em [Salesforce.com](https://Salesforce.com)_ como um contato ou lead.

<table> 
 <thead> 
  <tr> 
   <th>Etapa de fluxo do Marketo</th> 
   <th>Ação automática</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Adicionar à campanha da SFDC</td> 
   <td>Sincronizar pessoa à SFDC</td> 
  </tr> 
  <tr> 
   <td>Alterar status de campanha da SFDC</td> 
   <td>Sincronizar pessoa ao SFDC<br>Adicionar à campanha SFDC</td> 
  </tr> 
  <tr> 
   <td>Alterar proprietário</td> 
   <td><p>Sincronizar pessoa à SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Converter pessoa</td> 
   <td><p>Sincronizar pessoa à SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Criar tarefa</td> 
   <td>Sincronizar pessoa à SFDC</td> 
  </tr> 
 </tbody> 
</table>

Você pode filtrar registros SFDC em uma Smart List usando o **Tipo SFDC** O filtro com o operador definido como &quot;não está vazio&quot;. Todos os registros SFDC têm um valor nesse campo.

Lembre-se de que essas ações automáticas só ocorrerão se o lead não estiver em [Salesforce.com](https://salesforce.com)
