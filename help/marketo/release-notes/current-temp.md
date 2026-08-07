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
source-git-commit: ebd911b99e1c4c8f8a76db3a14235ee0d4ee0485
workflow-type: tm+mt
source-wordcount: 408
ht-degree: 28%

---

# Notas de versão: agosto de 2026 {#release-notes-aug-26}

Abaixo você encontrará todos os recursos incluídos na versão de agosto de 2026. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **14 de agosto de 2026**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Nova interface do Marketo Engage</strong>: a interface do Marketo Engage tem uma aparência atualizada, incluindo menus, ícones e layout atualizados para oferecer uma experiência mais limpa e moderna. Esta é apenas uma atualização visual. Nenhuma funcionalidade ou fluxo de trabalho existente é afetado.
</td>
   <td>Implantação em fases durante o mês de agosto</td>
   <td><i>n/d</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Construtor de scripts</strong>: o Construtor de scripts é um assistente habilitado para IA que ajuda você a criar scripts de personalização mais rapidamente.
</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Desabilitar Campanhas no Arquivo Morto</strong>: o arquivamento de uma pasta agora desabilita e desagenda todas as campanhas nessa árvore de pastas, impedindo a execução inesperada de Campanhas Inteligentes arquivadas.
</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Descontinuação do Parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo está sendo descontinuado e não estará disponível após 31 de agosto de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **ID de Execução da Campanha da API REST**: o suporte para a API SOAP do Marketo terminará em 31 de julho de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
* **Limites de Tamanho de Lista Estática para Obter Atividades de Cliente Potencial e Obter Alterações de Cliente Potencial**: Em determinadas circunstâncias, o valor da ID de Execução de Campanha de uma atividade era retornado com formatação incorreta, entre dois pares de aspas (por exemplo, `"campaignRunId": ""102938""`).<br/>
A partir da versão de agosto, esse valor sempre será retornado com o formato numérico correto (`"campaignRunId": 102938`)

* **Limite de Clientes Potenciais de Mesclagem da API REST**: a partir de 31 de julho de 2026, chamadas que incluem mais de 25 IDs no parâmetro leadIds de uma chamada da API de Clientes Potenciais de Mesclagem resultarão em um código de erro 1080, e a chamada será ignorada. As tarefas que exigem a fusão de mais de 25 registros em um devem ser divididas em várias tarefas para garantir o sucesso dessas chamadas.
