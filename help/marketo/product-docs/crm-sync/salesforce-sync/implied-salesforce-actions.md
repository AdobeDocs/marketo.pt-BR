---
unique-page-id: 4719304
description: Ações Implementadas Do Salesforce - Documentos Do Marketing - Documentação Do Produto
title: Ações Implícitas do Salesforce
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---


# Ações Implícitas do Salesforce {#implied-salesforce-actions}

Quando uma etapa de fluxo específica do Salesforce é executada, às vezes as etapas extras são executadas automaticamente. Estas são as regras, então você sabe:

Essas regras serão aplicadas _quando a pessoa não estiver atualmente em [Salesforce.com](http://Salesforce.com)_ como um contato ou cliente potencial.

<table> 
 <thead> 
  <tr> 
   <th>Etapa de fluxo de marketing</th> 
   <th>Ação automática</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Adicionar à Campanha SFDC</td> 
   <td>Sincronizar Pessoa com SFDC</td> 
  </tr> 
  <tr> 
   <td>Alterar status na Campanha SFDC</td> 
   <td>Sincronizar Pessoa com SFDC<br>Adicionar à Campanha SFDC</td> 
  </tr> 
  <tr> 
   <td>Alterar proprietário</td> 
   <td><p>Sincronizar Pessoa com SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Converter Pessoa</td> 
   <td><p>Sincronizar Pessoa com SFDC</p></td> 
  </tr> 
  <tr> 
   <td>Criar Tarefa</td> 
   <td>Sincronizar Pessoa com SFDC</td> 
  </tr> 
 </tbody> 
</table>

Você pode filtrar registros SFDC em uma Lista inteligente usando o filtro **SFDC Type** com o operador definido como &quot;não está vazio&quot;. Todos os registros SFDC têm um valor neste campo.

Lembre-se, essas ações automáticas só acontecem se o cliente potencial não estiver em [Salesforce.com](https://salesforce.com)
