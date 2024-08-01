---
description: Notas de versão - março de 2024 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Março de 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: 1839ccb646e775b67efa8de7d2d2bf3dbbbefa72
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 4%

---

# Notas de versão: março de 2024 {#release-notes-mar-24}

Abaixo você encontrará todos os recursos incluídos na versão de março de 2024. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **8 de março de 2024**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Recurso</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr> 
   <td><strong>Lógica de Fluxo de Conversação Avançado</strong>: adicione campos adicionais para avaliação em uma única opção para acompanhamento de Fluxo de Conversação.</td> 
   <td>Remetido</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Configurações de fluxo de conversa para Marketo Engage Forms</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Reordenar Lógica de Fluxo de Conversação</strong>: no Marketo Engage Forms, agora você pode reordenar as opções de Fluxo de Conversação, em vez de ter que excluir e adicionar novamente.</td> 
   <td>Remetido</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Configurações de fluxo de conversa para Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Metadados de atividade de API</strong>: 
   Metadados como Agente do usuário, Plataforma e Dispositivo agora são incluídos em atividades da Web e de email, ajudando a fornecer insights consistentes sobre essas atividades por meio da API REST do Marketo.</td> 
   <td>Remetido</td>
   <td>n/d</td>
  </tr>
 </tbody> 
</table>
<br/>

## Anúncios {#announcements}

* **Correção da API Obter Membro do Programa**: uma alteração foi feita recentemente para corrigir o comportamento do ponto de extremidade [Obter Membros do Programa](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Program-Members/operation/getProgramMembersUsingGET){target="_blank"}. Anteriormente, ao utilizar o tipo de filtro `updatedAt` para especificar um intervalo de datas, havia uma chance de os registros de associação de programa atualizados nesse intervalo não serem incluídos na resposta. Além disso, havia uma chance de os registros de associação ao programa serem atualizados fora do intervalo de datas especificado e incluídos incorretamente na resposta. Ambos os problemas foram resolvidos.

* **Substituição do plug-in do navegador do Account Insight**: o Adobe está removendo o [plug-in do navegador Account Insight](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} do Target Account Management da Chrome Web Store em 8 de abril de 2024. Usuários existentes: você pode continuar a usar o plug-in até migrar a instância do Marketo Engage para a Identidade e Admin Console do Adobe. Essa alteração **não afetará** nenhum outro recurso/dado de TAM no Marketo Engage ou nos plug-ins de email do Chrome e do Outlook que funcionam com o Sales Insight. [Saiba mais](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
