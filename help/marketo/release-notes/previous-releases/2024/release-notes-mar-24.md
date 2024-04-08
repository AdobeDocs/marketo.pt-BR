---
description: Notas de versão - março de 2024 - Documentação do Marketo - Documentação do produto
title: Notas de versão - março de 2024
feature: Release Information
exl-id: d8bc7f88-a77b-4b49-aed5-aceab9e639f0
source-git-commit: fd92f5307880019f54bb2f1778093c110a53ed2c
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 3%

---

# Notas de versão: março de 2024 {#release-notes-mar-24}

Abaixo você encontrará todos os recursos incluídos na versão de março de 2024. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

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
   <td><strong>Lógica de Fluxo de Conversação Avançada</strong>: adicione campos adicionais para avaliação em uma única escolha para acompanhamento do Fluxo de conversa.</td> 
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
   <td><strong>Reordenar Lógica de Fluxo de Conversação</strong>: no Marketo Engage Forms, agora é possível reordenar as opções de Fluxo de conversa, em vez de precisar excluir e adicionar novamente.</td> 
   <td>Remetido</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/conversational-flow-settings-for-marketo-engage-forms.md" target="_blank">Configurações de fluxo de conversa para Marketo Engage Forms</a></td>
   </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Metadados de atividade da API</strong>: Metadados como Agente do usuário, Plataforma e Dispositivo agora são incluídos em atividades da Web e de email, ajudando a fornecer insights consistentes sobre essas atividades por meio da API REST do Marketo.</td> 
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anúncios {#announcements}

* **Obter correção da API do membro do programa**: uma alteração foi feita recentemente para corrigir o comportamento do [Obter membros do programa](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Program_Members/getProgramMembersUsingGET){target="_blank"} terminal. Anteriormente, ao utilizar a variável `updatedAt` tipo de filtro para especificar um intervalo de datas. Houve uma chance de os registros de associação de programa atualizados nesse intervalo não serem incluídos na resposta. Além disso, havia uma chance de os registros de associação ao programa serem atualizados fora do intervalo de datas especificado e incluídos incorretamente na resposta. Ambos os problemas foram resolvidos.

* **Substituição do plug-in do navegador do Insight da conta**: o Adobe está removendo o Gerenciamento de conta do Target [Plug-in de navegador do Account Insight](/help/marketo/product-docs/target-account-management/setup-tam/account-insight-plug-in-overview.md){target="_blank"} from the Chrome Web Store on April 8, 2024. Existing users: you can continue to use the plug-in until you migrate your Marketo Engage instance to Adobe Identity and Admin Console. This change **will not impact** any other TAM features/data within Marketo Engage or the Chrome and Outlook email plug-ins that work with Sales Insight. [Learn more](https://nation.marketo.com/t5/product-blogs/marketo-engage-account-insights-browser-plug-in-end-of-life/ba-p/344834){target="_blank"}.
