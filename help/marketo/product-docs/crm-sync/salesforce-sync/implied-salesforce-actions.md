---
unique-page-id: 4719304
description: Ações Implementadas Do Salesforce - Documentos Do Marketo - Documentação Do Produto
title: Ações do Salesforce Implementadas
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 21%

---

# Ações do Salesforce Implementadas {#implied-salesforce-actions}

Quando uma etapa de fluxo específica do Salesforce é executada, às vezes etapas extras são executadas automaticamente. Estas são as regras, para que você saiba:

Estas regras serão aplicáveis _quando a pessoa não está no momento [Salesforce.com](https://Salesforce.com)_ como contato ou cliente potencial.

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
   <td>Sincronizar pessoa com o SFDC<br>Adicionar à campanha SFDC</td> 
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

Você pode filtrar os registros SFDC em uma Smart List usando o **Tipo SFDC** O filtro com o operador definido como &quot;não está vazio&quot;. Todos os registros SFDC têm um valor neste campo.

Lembre-se, essas ações automáticas só acontecem se o lead não estiver no momento [Salesforce.com](https://salesforce.com)
