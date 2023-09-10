---
description: Comportamento Do Chatbot - Documentação Do Marketo - Documentação Do Produto
title: Comportamento do Chatbot
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 801c9935cacf79971ce42a9517647e310a1ed25a
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Comportamento do Chatbot {#chatbot-behavior}

A seguir estão diferentes cenários possíveis que descrevem o comportamento esperado do Chatbot para o visitante em cada um.

<table>
  <tbody>
    <tr>
      <th>Abreviação</th>
      <th>Detalhes</th>
    </tr>
    <tr>
      <td>D1, D2, D3, etc.</td>
      <td>Representa várias caixas de diálogo onde D1 é a caixa de diálogo um</td>
    </tr>
    <tr>
      <td>P1, P2, P3, etc.</td>
      <td>Representa as prioridades de diálogo em que P1 é a prioridade mais alta</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3, etc.</td>
      <td>Representa várias páginas da Web em que WP1 é a primeira página da Web</td>
    </tr>
    <tr>
      <td>V1, V2, V3 etc.</td>
      <td>Representa vários visitantes da página da Web em que V1 é o visitante um</td>
    </tr>
   </tbody>
</table>

## Cenários {#scenarios}

<table>
  <tr>
      <th>Cenário</th>
      <th>Comportamento de Chatbot esperado</th>
      <th>Ação de backend</th>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 será resolvido para V1</p>
      </td>
      <td>A contagem de acionadores de D1 será aumentada em 1</td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 será resolvido para V1</p>
        <p>Após a atualização, D1 será resolvido novamente</p>
      </td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>Após a atualização, nenhuma alteração no acionador D1 ou na contagem de engajamento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clicou em D1, mas não respondeu</p>
      </td>
      <td>D1 será resolvido para V1</td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>Nenhuma alteração na contagem de engajamento D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clica em D1 e fornece a primeira resposta</p>
      </td>
      <td>D1 será resolvido para V1</td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>A contagem de engajamento para D1 será aumentada em 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clica em D1 e fornece a primeira resposta</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 será resolvido para V1</p>
        <p>Após a atualização, D1 continuará</p>
      </td>
      <td>
        <p>A contagem de acionadores e de engajamento de D1 será aumentada em 1</p>
        <p>Após a atualização, nenhuma alteração será feita em qualquer contagem</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clica em D1, interage com o chatbot e conclui D1</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 será resolvido para V1</p>
        <p>Após a atualização, nenhuma caixa de diálogo ou próxima caixa de diálogo será resolvida para V1</p>
      </td>
      <td>
        <p>A contagem de acionadores, contagem de engajamento e contagem concluída para D1 será aumentada em 1</p>
        <p>Após a atualização, nenhuma caixa de diálogo ou próxima caixa de diálogo será resolvida</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1, WP2</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clicou em D1, mas não respondeu</p>
        <p>V1 visita WP2</p>
      </td>
      <td>
        <p>A visita à página WP1, D1 será resolvida para V1</p>
        <p>Visita à página WP2, D1 será resolvido para V2</p>
      </td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>No WP2, nenhuma alteração na contagem de acionadores D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1, WP2</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clica em D1 e engatada</p>
        <p>V1 visita WP2</p>
      </td>
      <td>
        <p>A visita à página WP1, D1 será resolvida para V1</p>
        <p>Visita à página WP2, D1 será resolvida para V1</p>
      </td>
      <td>
        <p>A contagem de acionadores e de engajamento de D1 será aumentada em 1</p>
        <p>No WP2, nenhuma alteração em qualquer contagem</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>D2 direcionado somente para WP2</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clica em D1 e fornece a primeira resposta</p>
        <p>V1 visita WP2</p>
      </td>
      <td>
        <p>D1 será resolvido no WP1</p>
        <p>D1 continuará para V1 no WP2</p>
      </td>
      <td>
        <p>A contagem de acionadores e de engajamento de D1 será aumentada em 1</p>
        <p>Nenhuma alteração no acionador D2 ou na contagem de engajamento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>D2 direcionado somente para WP2</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clicou em D1, mas não respondeu</p>
        <p>V1 visita WP2</p>
      </td>
      <td>D1 será resolvido no WP1<br/>
      D2 será resolvido no WP2</td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>A contagem de acionadores para D2 será aumentada em 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>D2 direcionado somente para WP2</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clica em D1 e conclui D1</p>
        <p>V1 visita WP2</p>
      </td>
      <td>D1 será resolvido no WP1 e na pós-conclusão<br/>D2 será resolvido no WP2</td>
      <td>
        <p>A contagem de acionadores, contagem de engajamento e contagem concluída para D1 será aumentada em 1</p>
        <p>A contagem de acionadores para D2 será aumentada em 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>D2 direcionado somente para WP2</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clica em D1 e conclui D1</p>
        <p>V1 visita WP2</p>
        <p>V1 clica em D2 fornece a primeira resposta</p>
      </td>
      <td>D1 será resolvido no WP1 e na pós-conclusão<br/>D2 será resolvido no WP2</td>
      <td>
        <p>A contagem de acionadores, contagem de engajamento e contagem concluída para D1 será aumentada em 1</p>
        <p>O acionador e a contagem de engajamento para D2 serão aumentados em 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clicou em D1, mas não respondeu</p>
        <p>A publicação de D1 foi desfeita</p>
      </td>
      <td>D1 será resolvido para V1</td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>Nenhuma alteração na contagem de engajamento D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clicou em D1, mas não respondeu</p>
        <p>A publicação de D1 foi desfeita</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 será resolvido para V1 pela primeira vez</p>
        <p>Após a atualização, nenhuma caixa de diálogo será resolvida</p>
      </td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>Nenhuma alteração na contagem de engajamento D1</p>
        <p>Após a atualização, nenhuma alteração no acionador D1 ou na contagem de engajamento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 engajada com D1</p>
        <p>A publicação de D1 foi desfeita</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 será resolvido para V1</p>
        <p>Após a atualização, D1 continuará</p>
      </td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>A contagem de envolvimento D1 será aumentada em 1</p>
        <p>Após a atualização, como D1 continuará, não haverá mais alterações para acionar ou contagem de engajamento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clicou em D1, mas não respondeu</p>
        <p>D1 é publicado com novas alterações</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 será resolvido para V1 pela primeira vez</p>
        <p>Após a atualização, a caixa de diálogo com novas alterações será resolvida</p>
      </td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>Após a atualização, como D1 com novas alterações, mas sem mais alterações para acionar a contagem</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado somente para WP1</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clica em D1 fornece a primeira resposta</p>
        <p>D1 é publicado com novas alterações</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 será resolvido para V1 pela primeira vez</p>
        <p>Após a atualização, a caixa de diálogo com as alterações antigas continuará</p>
      </td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>A contagem de engajamento para D1 será aumentada em 1</p>
        <p>Após a atualização, como o D1 antigo aparecerá, nenhuma alteração acionará a contagem</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 direcionado para WP1 com prioridade 1</p>
        <p>D2 direcionado para WP1 com prioridade 2</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clicou em D1, mas não respondeu</p>
        <p>A publicação de D1 foi desfeita</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 será resolvido para V1 pela primeira vez</p>
        <p>Após a atualização, D2 será resolvido para V1</p>
      </td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>Após a atualização, a contagem de acionadores para D2 será aumentada em 1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1 com prioridade 1</p>
        <p>D2 direcionado para WP1 com prioridade 2</p>
        <p>V1 visita WP1 pela primeira vez</p>
        <p>V1 clica em D1 e conclui D1</p>
        <p>V1 atualiza WP1 e consulte D2<br/>V1 clica em D2 e conclui D2</p>
        <p>O profissional de marketing fez alterações no D1 e publicou novamente</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 será resolvido para V1 pela primeira vez</p>
        <p>Após a atualização, D2 será resolvido para V1</p>
        <p>Depois de concluir D1 e D2, independentemente de quais alterações ou D1 foi republicado, D2 não será exibido novamente para V1</p>
      </td>
      <td>
        <p>A contagem de acionadores, contagem de engajamento e contagem concluída para D1 será aumentada em 1</p>
        <p>Atualizar depois que D2 for concluído, nenhuma ação a ser executada</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1 com acionador "Tempo no site" de 30 segundos</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 será resolvido, mas não será acionado para V1</p>
        <p>Após 30 segundos, D1 será exibido/acionado para V1</p>
      </td>
      <td>A contagem de acionadores de D1 será aumentada em 1 somente após mais de 30 segundos gastos na página da Web</td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1, WP2 com acionador "Tempo na página" de 30 segundos</p>
        <p>V1 visita WP1, WP2</p>
      </td>
      <td>
        <p>D1 será resolvido, mas não será acionado para V1</p>
        <p>Após 30 segundos, D1 será exibido/acionado para V1</p>
      </td>
      <td>A contagem de acionadores de D1 será aumentada em 1 somente após mais de 30 segundos gastos na página da Web</td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1 com acionador "porcentagem de rolagem" de 50</p>
        <p>V1 visita WP1</p>
      </td>
      <td>
        <p>D1 será resolvido, mas não será acionado para V1</p>
        <p>Depois de rolar 50%, D1 será exibido/acionado para V1</p>
      </td>
      <td>A contagem de acionadores de D1 será aumentada em 1 somente depois da rolagem de 50%</td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1 com prioridade 1 e acionador "Tempo na página" de evento de 30 segundos</p>
        <p>D2 direcionado para WP1 com prioridade 2 e "porcentagem de rolagem de página" de evento de 50</p>
        <p>V1 visita WP1, depois de 10 segundos V1 visita WP2, V1 visita WP1</p>
      </td>
      <td>
        <p>No WP1, D1 será resolvido, mas não será acionado para V1</p>
        <p>No WP2, D2 será resolvido, mas não será acionado para V1</p>
        <p>No WP1, D1 será resolvido e após 20 segundos D1 será acionado para V1</p>
      </td>
      <td>A contagem de acionadores de D1 será aumentada em 1 somente após 30 segundos</td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1 com acionador "Tempo no site" de 1 minuto</p>
        <p>V1 visita WP1 por 1 minuto e mostra D1, mas não envolve</p>
        <p>A V1 fecha o WP1 e retorna ao WP1 2 dias depois</p>
      </td>
      <td>
        <p>D1 será exibido automaticamente para V1, pois eles já atenderam aos critérios de acionador durante a sessão anterior</p>
        <p>A mesma lógica será aplicada ao "Tempo na página" e à "porcentagem de rolagem da página"</p>
      </td>
      <td>
        <p>A contagem de acionadores de D1 será aumentada em 1</p>
        <p>Após o retorno, nenhuma ação a ser tomada</p>
      </td>
    </tr>
  </tbody>
</table>

