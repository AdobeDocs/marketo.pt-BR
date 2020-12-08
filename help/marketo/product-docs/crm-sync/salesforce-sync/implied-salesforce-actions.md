---
unique-page-id: 4719304
description: Ações Implementadas Do Salesforce - Documentos Do Marketing - Documentação Do Produto
title: Ações Implícitas do Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---


# Ações Implícitas do Salesforce {#implied-salesforce-actions}

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Quando uma etapa de fluxo específica do Salesforce é executada, às vezes as etapas extras são executadas automaticamente. Estas são as regras, então você sabe:

Essas regras serão aplicadas *quando a pessoa não estiver atualmente em [Salesforce.com](http://Salesforce.com)* como contato ou cliente potencial.

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
   <td>Sincronizar pessoa com a Campanha<br>SFDCAdd com SFDC</td> 
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

Você pode filtrar os registros SFDC em uma Lista inteligente usando o Filtro de tipo **** SFDC com o operador definido como &quot;não está vazio&quot;. Todos os registros SFDC têm um valor neste campo.

Lembre-se, essas ações automáticas só acontecem se o cliente potencial não estiver no [Salesforce.com](http://Salesforce.com)

A sincronização do Salesforce é legal, certo?
