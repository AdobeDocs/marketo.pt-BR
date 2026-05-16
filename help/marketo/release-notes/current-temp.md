---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f71e690b-4480-4b67-9ef5-88f42f9cdfdbid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a04ec3931933c8e6cc0a0ffc26b1b559cd7cc9ce
workflow-type: tm+mt
source-wordcount: 421
ht-degree: 28%

---

# Notas de versão: maio de 2026 {#release-notes-may-26}

Abaixo você encontrará todos os recursos incluídos na versão de maio de 2026. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **22 de maio de 2026**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Conteúdo Condicional para Fragmentos de Email</strong>: <i>Paridade com o editor de email antigo</i>. O conteúdo condicional agora é compatível com Fragmentos.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Gerenciamento de lista de opções</strong>: agora é possível especificar os valores que podem ser usados em campos no Marketo Engage.
   </td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Campos de descontinuação de recursos sociais**: em 2025, o Marketo Engage descontinuou os seguintes recursos sociais:

   * Pesquisas
   * Botão de redes sociais
   * Oferta de recomendação
   * Compartilhamento de vídeo
   * Sorteios

No início deste ano, os campos relacionados que foram deixados para trás foram removidos do Marketo. Logo depois, as solicitações de API que referenciavam determinados campos de lead relacionados ao Social retornavam um erro &quot;campo não encontrado&quot;, causando interrupções. O serviço foi restaurado depois que os campos afetados foram disponibilizados novamente, para evitar mais interrupções, o Marketo desvinculou permanentemente os campos do Social da desativação de recursos do Social (e, como tal, estará disponível na conta do Marketo). Os usuários são incentivados a revisar consultas e integrações de API que fazem referência a campos relacionados ao Marketo Social e determinam se esses campos ainda são necessários para processos de negócios em andamento.

* **Descontinuação do parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo está sendo descontinuado e não estará disponível após 31 de julho de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API do SOAP**: o suporte para a API do Marketo SOAP terminará em 31 de julho de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Limites de Tamanho de Lista Estática para Obter Atividades de Cliente Potencial e Obter Alterações de Cliente Potencial**: a partir de 30 de setembro de 2026, as chamadas para Obter Atividades de Cliente Potencial e Obter Pontos de Extremidade de Alterações de Cliente Potencial que incluem o parâmetro `listId` retornarão um código de erro 1003 se a lista estática de destino contiver 10.000 ou mais clientes potenciais. Consulte o [Guia de Migração](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obter mais informações.
