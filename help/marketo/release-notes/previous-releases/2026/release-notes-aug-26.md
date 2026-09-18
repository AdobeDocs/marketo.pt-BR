---
description: Notas de versão - julho de 2026 - Documentação do Marketo - Documentação do produto
title: Notas de versão - julho de 2026
feature: Release Information
source-git-commit: edeb795f12082fab9c72b0ff4305f3db90aa4c46
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 15%
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
   <td><strong>Nova interface do Marketo Engage</strong>: a interface do Marketo Engage tem uma aparência atualizada, incluindo menus, ícones e layout atualizados para oferecer uma experiência mais limpa e moderna. Esta é apenas uma atualização visual; nenhuma funcionalidade ou fluxo de trabalho existente é afetado.
</td>
   <td>Implantação em fases durante agosto e setembro</td>
   <td><i>n/d</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Desabilitar Campanhas no Arquivo Morto</strong>: o arquivamento de uma pasta agora desabilita e desagenda todas as campanhas nessa árvore de pastas, impedindo a execução inesperada de Campanhas Inteligentes arquivadas.
</td>
   <td>Lançado</td>
   <td><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders#disable-campaigns-archive" target="_blank">Desativar campanhas no arquivo</a></td>
  </tr>
    <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Menu Contextual Gerar Conteúdo</strong>: os recursos "Gerar conteúdo" do Email Designer agora podem ser acessados no menu contextual (a barra preta). Por exemplo, quando você seleciona conteúdo de texto, o ícone Gerar conteúdo é exibido no menu contextual, permitindo executar ações rápidas.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **O Marketo AI agora é o Co-worker para Marketo Engage**: o Co-worker para Marketo Engage fornece habilidades de agente projetadas para automatizar funções de marketing demoradas. Novo nome, mesmos recursos, disponíveis para todos os usuários. [Saiba mais](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/coworker-for-marketo/overview){target="_blank"}

* **Descontinuação do Parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo está sendo descontinuado e não estará disponível após 31 de agosto de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **ID de Execução da Campanha da API REST**: em determinadas circunstâncias, o valor da ID de Execução da Campanha de uma atividade era retornado com formatação incorreta, entre dois pares de aspas (por exemplo, `"campaignRunId": ""102938""`).<br/>A partir da versão de agosto, esse valor sempre será retornado com o formato numérico correto (`"campaignRunId": 102938`)

* **Limites de Tamanho de Lista Estática para Obter Atividades de Cliente Potencial e Obter Alterações de Cliente Potencial**: a partir de 30 de setembro de 2026, as chamadas para Obter Atividades de Cliente Potencial ou Obter Alterações de Cliente Potencial que incluem o parâmetro `listId` falharão com um Código de Erro 1003 (indicando que a lista estática de destino tem muitos registros) se as listas de destino contiverem 10.000 ou mais clientes potenciais. Consulte o [Guia de Migração](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obter mais informações.

* **Limite de Clientes Potenciais de Mesclagem da API REST**: a partir de 31 de julho de 2026, chamadas que incluem mais de 25 IDs no parâmetro leadIds de uma chamada da API de Clientes Potenciais de Mesclagem resultarão em um código de erro 1080, e a chamada será ignorada. As tarefas que exigem a fusão de mais de 25 registros em um devem ser divididas em várias tarefas para garantir o sucesso dessas chamadas.
