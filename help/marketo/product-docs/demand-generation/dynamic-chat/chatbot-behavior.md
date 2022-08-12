---
description: Comportamento do chatbot - Documentos do Marketo - Documentação do produto
title: Comportamento do chatbot
hide: true
hidefromtoc: true
source-git-commit: 4ec9338bec2e0255eab4304da74464dd47ffae24
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Comportamento do chatbot {#chatbot-behavior}

A seguir estão diferentes cenários possíveis que descrevem o comportamento esperado do Chatbot para o visitante em cada um.

<table>
  <tbody>
    <tr>
      <th>Abreviação</th>
      <th>Detalhes</th>
    </tr>
    <tr>
      <td>D1, D2, D3, etc.</td>
      <td>Representa várias caixas de diálogo, onde D1 é a caixa de diálogo 1</td>
    </tr>
    <tr>
      <td>P1, P2, P3, etc.</td>
      <td>Representa as prioridades da caixa de diálogo em que P1 é a prioridade mais alta</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3, etc.</td>
      <td>Representa várias páginas da Web, onde WP1 é a primeira página da Web</td>
    </tr>
    <tr>
      <td>V1, V2, V3, etc.</td>
      <td>Representa vários visitantes de página da Web, onde V1 é o visitante um</td>
    </tr>
   </tbody>
</table>

## Cenários {#scenarios}

<table>
  <tr>
      <th>Cenário</th>
      <th>Comportamento de chatbot esperado</th>
      <th>Ação de backend</th>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>Visitas V1 WP1</p>
      </td>
      <td>
        <p>D1 deve ser resolvido para V1 </p>
      </td>
      <td>A contagem de acionadores para D1 deve ser aumentada em 1</td>
    </tr>
    <tr background: #CCCCCC>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>Visitas V1 WP1</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 deve ser resolvido para V1</p>
        <p>Após a atualização, D1 deve ser resolvido novamente</p>
      </td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>Após a atualização, nenhuma alteração no acionador D1 ou na contagem de engajamento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1, mas não respondeu </p>
      </td>
      <td>D1 deve ser resolvido para V1</td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>Nenhuma alteração na contagem de envolvimento de D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1 e fornece a primeira resposta  </p>
      </td>
      <td>D1 deve ser resolvido para V1</td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>A contagem de engajamento para D1 deve ser aumentada em 1 </p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1 e fornece a primeira resposta</p>
        <p>V1 atualiza WP1  </p>
      </td>
      <td>
        <p>D1 deve ser resolvido para V1</p>
        <p>Após a atualização, D1 deve ser continuado</p>
      </td>
      <td>
        <p>A contagem de acionadores e de envolvimento para D1 deve ser aumentada em 1 </p>
        <p>Após a atualização, nenhuma alteração será alterada para qualquer contagem</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1, se envolve com o chatbot e completa D1</p>
        <p>V1 atualiza WP1  </p>
      </td>
      <td>
        <p>D1 deve ser resolvido para V1</p>
        <p>Após a atualização, nenhuma caixa de diálogo ou caixa de diálogo seguinte deverá ser resolvida para V1</p>
      </td>
      <td>
        <p>A contagem de acionadores, a contagem de engajamento e a contagem concluída para D1 devem ser aumentadas em 1 </p>
        <p>Após a atualização, nenhuma caixa de diálogo ou caixa de diálogo seguinte deverá ser resolvida</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1, WP2</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1, mas não respondeu </p>
        <p>V1 visitas WP2</p>
      </td>
      <td>
        <p>A visita à página WP1, D1 deve ser resolvida para V1</p>
        <p>A visita à página WP2, D1 deve ser resolvida para V2</p>
      </td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>No WP2, nenhuma alteração na contagem de acionadores D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1, WP2</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1 e está envolvido</p>
        <p>V1 visitas WP2</p>
      </td>
      <td>
        <p>A visita à página WP1, D1 deve ser resolvida para V1</p>
        <p>A visita à página WP2, D1 deve ser resolvida para V1</p>
      </td>
      <td>
        <p>A contagem de acionadores e de envolvimento para D1 deve ser aumentada em 1 </p>
        <p>No WP2, nenhuma alteração em qualquer contagem</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>D2 destinado apenas ao WP2</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1 e fornece a primeira resposta</p>
        <p>V1 visitas WP2</p>
      </td>
      <td>
        <p>D1 deve ser resolvido no WP1</p>
        <p>D1 deve continuar para V1 no WP2</p>
      </td>
      <td>
        <p>A contagem de acionadores e de envolvimento para D1 deve ser aumentada em 1 </p>
        <p>Nenhuma alteração na contagem de acionadores ou de envolvimento de D2</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>D2 destinado apenas ao WP2</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1, mas não respondeu </p>
        <p>V1 visitas WP2</p>
      </td>
      <td>D1 deve ser resolvido no WP1<br/>D2 deve ser resolvido no WP2</td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>A contagem de acionadores para D2 deve ser aumentada em 1 </p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>D2 destinado apenas ao WP2</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1 e completa D1</p>
        <p>V1 visitas WP2</p>
      </td>
      <td>D1 deve ser resolvido no WP1 e no pós-conclusão<br/>D2 deve ser resolvido no WP2</td>
      <td>
        <p>O acionador, o envolvimento e a contagem concluída de D1 devem ser aumentados em 1 </p>
        <p>A contagem de acionadores para D2 deve ser aumentada em 1 </p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>D2 destinado apenas ao WP2</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1 e completa D1</p>
        <p>V1 visitas WP2</p>
        <p>Cliques V1 em D2 fornecem a primeira resposta </p>
      </td>
      <td>D1 deve ser resolvido no WP1 e no pós-conclusão<br/>D2 deve ser resolvido no WP2</td>
      <td>
        <p>O acionador, o envolvimento e a contagem concluída de D1 devem ser aumentados em 1 </p>
        <p>A contagem de acionador e envolvimento para D2 deve ser aumentada em 1 </p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1, mas não respondeu </p>
        <p>D1 não está publicado</p>
      </td>
      <td>D1 deve ser resolvido para V1</td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>Nenhuma alteração na contagem de envolvimento de D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1, mas não respondeu </p>
        <p>D1 não está publicado</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 deve ser resolvido para V1 pela primeira vez</p>
        <p>Após a atualização, nenhuma caixa de diálogo deve ser resolvida </p>
      </td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>Nenhuma alteração na contagem de envolvimento de D1</p>
        <p>Após a atualização, nenhuma alteração no acionador D1 ou na contagem de engajamento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 com D1 </p>
        <p>D1 não está publicado</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 deve ser resolvido para V1</p>
        <p>Após a atualização, D1 deve ser continuado </p>
      </td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>A contagem de engajamento D1 deve ser aumentada em 1</p>
        <p>Após a atualização, como D1 será continuado, nenhuma alteração no acionador ou na contagem de engajamento</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1, mas não respondeu </p>
        <p>D1 é publicado com novas alterações</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 deve ser resolvido para V1 pela primeira vez</p>
        <p>Após a atualização, a caixa de diálogo com novas alterações deve ser resolvida</p>
      </td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>Após a atualização, como D1 com novas alterações, mas sem mais alterações para acionar a contagem</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado apenas para WP1</p>
        <p>V1 visita WP1 primeira vez</p>
        <p>Cliques V1 em D1 fornece a primeira resposta </p>
        <p>D1 é publicado com novas alterações</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 deve ser resolvido para V1 pela primeira vez</p>
        <p>Após a atualização, a caixa de diálogo com as alterações antigas deve continuar</p>
      </td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>A contagem de engajamento para D1 deve ser aumentada em 1 </p>
        <p>Após a atualização, como o D1 antigo aparecerá, portanto, nenhuma alteração na contagem de acionadores</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 direcionado para WP1 com prioridade 1</p>
        <p>D2 destinado ao WP1 com prioridade 2 </p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1, mas não respondeu </p>
        <p>D1 não está publicado</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 deve ser resolvido para V1 pela primeira vez</p>
        <p>Após a atualização, D2 deve ser resolvido para V1</p>
      </td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>Após a atualização, a contagem de acionadores para D2 deve ser aumentada em 1 </p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1 com prioridade 1</p>
        <p>D2 destinado ao WP1 com prioridade 2 </p>
        <p>V1 visita WP1 primeira vez</p>
        <p>V1 clica em D1 e completa D1</p>
        <p>V1 atualiza WP1 e vê D2<br/>V1 clica em D2 e completa D2</p>
        <p>O profissional de marketing fez alterações em D1 e republicou</p>
        <p>V1 atualiza WP1</p>
      </td>
      <td>
        <p>D1 deve ser resolvido para V1 pela primeira vez</p>
        <p>Após a atualização, D2 deve ser resolvido para V1</p>
        <p>Depois de completar D1 e D2, independentemente das alterações ou republicação de D1, D2 não deve ser novamente indicada para V1</p>
      </td>
      <td>
        <p>O acionador, engajado, contagem concluída de D1 deve ser aumentado em 1 </p>
        <p>Atualizar depois que D2 for concluída, nenhuma ação será executada</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1 com acionador de "Tempo no Site" de 30 segundos</p>
        <p>Visitas V1 WP1</p>
      </td>
      <td>
        <p>D1 deve ser resolvido, mas não será acionado para V1 </p>
        <p>Após 30 segundos, D1 deve ser mostrado/acionado para V1</p>
      </td>
      <td>A contagem de acionadores para D1 deve ser aumentada em 1 somente após 30 segundos de tempo gasto</td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1, WP2 com acionador de "Tempo na página" de 30 segundos</p>
        <p>V1 visitas WP1, WP2</p>
      </td>
      <td>
        <p>D1 deve ser resolvido, mas não será acionado para V1 </p>
        <p>Após 30 segundos, D1 deve ser mostrado/acionado para V1</p>
      </td>
      <td>A contagem de acionadores para D1 deve ser aumentada em 1 somente após 30 segundos de tempo gasto</td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1 com acionador de "% de rolagem" de 50% </p>
        <p>Visitas V1 WP1</p>
      </td>
      <td>
        <p>D1 deve ser resolvido, mas não será acionado para V1 </p>
        <p>Após 50% de rolagem, D1 deve ser mostrado/acionado para V1</p>
      </td>
      <td>A contagem de acionadores para D1 deve ser aumentada em 1 somente após 50% de rolagem</td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1 com 1 prioridade e acionador de "Tempo na página" de evento de 30 segundos</p>
        <p>D2 direcionado para WP1 com prioridade 2 e "% de rolagem de página" de evento de 50%</p>
        <p>V1 visita WP1, após 10 segundos V1 visitas WP2, V1 visitas WP1</p>
      </td>
      <td>
        <p>No WP1, D1 deve ser resolvido, mas não será acionado para V1 </p>
        <p>No WP2, D2 deve ser resolvido, mas não será acionado para V1</p>
        <p>No WP1, D1 deve ser resolvido e, após 20 segundos, D1 deve ser acionado para V1 </p>
      </td>
      <td>A contagem de disparadores para D1 deve ser aumentada em 1 somente após 30 segundos</td>
    </tr>
    <tr>
      <td>
        <p>D1 direcionado para WP1 com acionador de "Tempo no Site" de 1 minuto</p>
        <p>V1 visita WP1 por 1 minuto e é mostrado D1, mas não envolve</p>
        <p>V1 fecha o WP1 e volta ao WP1 2 dias depois</p>
      </td>
      <td>
        <p>D1 deve ser exibido automaticamente para V1, pois já atenderam aos critérios de acionamento durante a sessão anterior</p>
        <p>A mesma lógica deve se aplicar ao "Tempo na página" e à "porcentagem de rolagem da página"</p>
      </td>
      <td>
        <p>A contagem de acionadores para D1 deve ser aumentada em 1 </p>
        <p>Após o regresso, nenhuma ação deve ser tomada</p>
      </td>
    </tr>
  </tbody>
</table>
