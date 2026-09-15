---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
hide: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
TQID: https://experienceleague.adobe.com/RZsCx9HAyJuDLO46WfshT30be-rMMDZjnygvU32NGfk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: df650f93bedc7202ad82f8f725616cd25e4a99ef
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 18%
---
# Notas de versão: setembro de 2026 {#release-notes-sep-26}

Abaixo você encontrará todos os recursos incluídos na versão de setembro de 2026. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **25 de setembro de 2026**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Nova interface do Marketo Engage</strong>: a interface do Marketo Engage tem uma aparência atualizada, incluindo menus, ícones e layout atualizados para oferecer uma experiência mais limpa e moderna. Esta é apenas uma atualização visual; nenhuma funcionalidade ou fluxo de trabalho existente é afetado. <i>A capacidade de selecionar a interface clássica estará disponível até a versão de janeiro de 2027</i>.
</td>
   <td>Disponibilidade geral até o final de setembro</td>
   <td><i>n/d</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Selecionar Partição na Importação</strong>: agora é possível selecionar na lista de Partições do espaço de trabalho local ao importar registros de pessoas em ambientes que tenham Espaços de Trabalho e Partições habilitados.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Alerta instantâneo na sincronização do CRM</strong>: os usuários que assinaram notificações do CRM receberão uma notificação imediata quando o status habilitado de suas alterações de sincronização do CRM nativas, dando aos administradores maior visibilidade de seu status de sincronização do CRM.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Etapas de Fluxo de Autoatendimento - Tempo Limite de Retorno de Chamada Aumentado</strong>: o período de tempo limite de retorno de chamada para Etapas de Fluxo de Autoatendimento está sendo aumentado de uma hora para quatro horas. Nenhuma ação é necessária da sua parte.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Restrições de Nome de API para Atributos de Atividade Personalizados**: Os Nomes de API para Atributos de Atividade Personalizados criados por meio da API ou da interface agora podem conter apenas caracteres alfanuméricos e sublinhados, e devem começar com um caractere alfanumérico.

* **Limites de Tamanho de Lista Estática para Obter Atividades de Cliente Potencial e Obter Alterações de Cliente Potencial**: a partir de 30 de setembro de 2026, as chamadas para Obter Atividades de Cliente Potencial ou Obter Alterações de Cliente Potencial que incluem o parâmetro `listId` falharão com um Código de Erro 1003 (indicando que a lista estática de destino tem muitos registros) se as listas de destino contiverem 10.000 ou mais clientes potenciais. Consulte o [Guia de Migração](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obter mais informações.

* **Descontinuação do Parâmetro &#39;access_token&#39; da API**: O parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo foi descontinuado a partir de 31 de agosto de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **ID de Execução da Campanha da API REST**: em determinadas circunstâncias, o valor da ID de Execução da Campanha de uma atividade era retornado com formatação incorreta, entre dois pares de aspas (por exemplo, `"campaignRunId": ""102938""`).<br/>A partir da versão de agosto, esse valor sempre será retornado com o formato numérico correto (`"campaignRunId": 102938`).

* **Descontinuação da Captura de Imagens da Web**: para estar em conformidade com as práticas recomendadas modernas de segurança e privacidade, o recurso [Capturar Imagens da Web](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"} será descontinuado a partir da versão de outubro.
