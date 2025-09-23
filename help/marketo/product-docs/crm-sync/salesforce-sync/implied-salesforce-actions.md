---
unique-page-id: 4719304
description: Ações Implícitas Do Salesforce - Documentação Do Marketo - Documentação Do Produto
title: Ações implícitas do Salesforce
exl-id: 88533588-77f2-465e-9644-a4f95b87f99d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 26%

---

# Ações implícitas do Salesforce {#implied-salesforce-actions}

Quando uma etapa de fluxo específica do [!DNL Salesforce] é executada, às vezes etapas adicionais são executadas automaticamente. Estas são as regras, então você sabe:

Estas regras serão aplicadas quando a pessoa não estiver atualmente em [Salesforce.com](https://Salesforce.com){target="_blank"} como um contato ou cliente potencial.

<table>
 <thead>
  <tr>
   <th>Etapa de fluxo do Marketo</th>
   <th>Ação automática</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>Adicionar à campanha do SFDC</td>
   <td>Sincronizar pessoa ao SFDC</td>
  </tr>
  <tr>
   <td>Alterar status de campanha do SFDC</td>
   <td>Sincronizar pessoa com o SFDC<br>Adicionar ao SFDC Campaign</td>
  </tr>
  <tr>
   <td>Alterar proprietário</td>
   <td><p>Sincronizar pessoa ao SFDC</p></td>
  </tr>
  <tr>
   <td>Converter pessoa</td>
   <td><p>Sincronizar pessoa ao SFDC</p></td>
  </tr>
  <tr>
   <td>Criar tarefa</td>
   <td>Sincronizar pessoa ao SFDC</td>
  </tr>
 </tbody>
</table>

Você pode filtrar os registros SFDC em uma Smart List usando o Filtro **[!UICONTROL Tipo SFDC]** com o operador definido como &quot;[!UICONTROL não está vazio]&quot;. Todos os registros do SFDC têm um valor nesse campo.

Lembre-se, estas ações automáticas só acontecem se o cliente em potencial não estiver atualmente em [Salesforce.com](https://salesforce.com){target="_blank"}
