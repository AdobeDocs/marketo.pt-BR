---
description: Notas de versão do Dynamic Chat - Documentos do Marketo - Documentação do produto
title: Notas de versão do Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
exl-id: 0a7e5cc9-f2a6-4721-bbdc-661249a2e2b6
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 68%

---

# Notas de versão do Dynamic Chat {#dynamic-chat-release}

As versões do Adobe Dynamic Chat operam em um modelo de entrega contínua, o que permite uma abordagem mais escalável para a implantação de recursos. Às vezes, há vários lançamentos em um mês, portanto, verifique regularmente para obter as informações mais atualizadas.

Para acessar a página de notas de versão padrão do Marketo Engage [clique aqui](/help/marketo/release-notes/current.md){target="_blank"}.

## Versão de junho de 2025 {#june-2025-release}

### Renovação da lógica de roteamento {#routing-logic-revamp}

Renovamos a lógica de roteamento de chat ao vivo no Dynamic Chat para garantir um comportamento de engajamento mais inteligente e previsível em todos os tipos de roteamento (Conta, Personalizado, Equipe e Round Robin). A nova lógica simplifica os fluxos de roteamento e melhora o tratamento de fallback quando os agentes estão indisponíveis.

#### Principais melhorias no comportamento de roteamento

* **Até duas tentativas de engajamento por sessão**

   * O sistema tenta se conectar com até dois agentes (no máximo), mas estritamente dentro da regra de roteamento principal.

   * Se um agente estiver disponível, mas não responder (por exemplo, recusar ou perder o bate-papo), o sistema tentará se conectar a um agente diferente do mesmo pool.

   * A lógica de fallback (como Round Robin) só será ativada se nenhum agente elegível for encontrado durante a resolução inicial, para que não seja realizada uma nova tentativa após uma falha no engajamento.

* **Comportamento específico da regra de roteamento**

_&#x200B;**Roteamento de conta**&#x200B;_

Se o domínio de email de um visitante for mapeado para uma conta conhecida, o agente mapeado sempre será priorizado.

Se o agente estiver disponível, o chat será roteado diretamente para ele.

Se o agente não estiver disponível, o sistema:

* Não tentará outro agente, mesmo se Round Robin estiver habilitado como fallback.

Em vez disso, ele:

* Mostra o calendário de reuniões do agente mapeado (se estiver habilitado) ou:
* Retornará a uma mensagem padrão (pior cenário).

A regra de roteamento no nível do cartão (por exemplo, Equipe, Personalizado) só será considerada se o Roteamento de conta não for elegível (nenhum domínio ou agente correspondente).

_&#x200B;**Roteamento personalizado/de equipe**&#x200B;_

Essas regras podem retornar vários agentes elegíveis.

Se o primeiro agente disponível não interagir, o sistema tentará mais um agente da mesma lista.

O fallback Round Robin não é acionado apenas porque um agente não responde.

Se nenhum dos agentes gerar engajamento:

* O sistema mostrará o calendário do agente da primeira tentativa (se habilitado),
-ou-
* Exibirá a mensagem de fallback padrão.

_&#x200B;**Roteamento Round Robin**&#x200B;_

Quando usado como uma regra de roteiro principal, o sistema:

* Tenta engajar o primeiro agente disponível do pool Round Robin.

* Se o primeiro agente não responder, ele tentará novamente com o segundo melhor agente elegível.

Se Round Robin for usado como fallback, ele será ativado somente se nenhum agente for resolvido a partir da regra principal.

_&#x200B;**Fluxo de experiência do visitante**&#x200B;_

O sistema verifica se o roteamento de conta deve ser aplicado.

* Se sim, e o agente estiver disponível, ele se conectará imediatamente.

* Se o agente não for elegível ou não estiver disponível, ele passará para a regra de roteamento no nível do cartão.

A regra de roteamento no nível da placa (Personalizada, Equipe, Round Robin) foi avaliada.

* A disponibilidade dos agentes elegíveis é verificada (permissões, status).

* O sistema aciona um agente e, se necessário, tenta um segundo agente da mesma regra.

* Se nenhum engajamento for bem-sucedido, a lógica de fallback será aplicada:

   * Fallback de calendário (se habilitado),
-ou-
   * Mensagem padrão.

O fallback de Round Robin só é considerado quando nenhum agente elegível é encontrado na regra de roteamento principal, não quando os agentes individuais não respondem.

##### Casos de uso {#use-cases}

_&#x200B;**Roteamento de conta**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Exemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>O domínio do visitante é mapeado em uma conta; o agente mapeado tem o chat ao vivo habilitado e disponível</td>
    <td>O chat se conecta diretamente ao agente mapeado</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>O agente mapeado não está disponível; o fallback Round Robin está habilitado</td>
    <td>O sistema seleciona um agente disponível por meio do Round Robin e os envolve </td>
  </tr>
  <tr>
    <td>Nenhum agente de fallback</td>
    <td>O agente mapeado está indisponível, sem fallback de Round Robin; a reserva de reunião está habilitada</td>
    <td>O sistema mostra um calendário do agente mapeado ou exibe uma mensagem de fallback padrão</td>
  </tr>
</tbody></table>

_&#x200B;**Roteamento personalizado**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Exemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>A lógica personalizada resolve uma lista de agentes. O primeiro agente está disponível e aceita o chat.</td>
    <td>O chat se conecta ao primeiro agente.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>A regra personalizada não resolve nenhum agente. Fallback Round Robin habilitado.</td>
    <td>O sistema seleciona um agente disponível por meio do Round Robin e os envolve.</td>
  </tr>
  <tr>
    <td>Nenhum agente de fallback</td>
    <td>Dois agentes resolvidos; nenhum aceita o chat, fallback definido como calendário de reuniões.</td>
    <td>Primeira tentativa: o calendário do agente é exibido ou a mensagem de fallback padrão é exibida.</td>
  </tr>
</tbody></table>

_&#x200B;**Roteamento de equipe**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Exemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>A equipe inclui agentes com chat ao vivo; o primeiro agente disponível aceita o chat.</td>
    <td>O chat se conecta a esse agente.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Nenhum agente de equipe disponível, e o recurso de fallback de Round Robin está habilitado.</td>
    <td>O sistema seleciona e se conecta com um agente do pool Round Robin.</td>
  </tr>
  <tr>
    <td>Nenhum agente de fallback</td>
    <td>Dois agentes disponíveis, mas nenhum gera engajamento; fallback de calendário habilitado.</td>
    <td>Primeira tentativa: o calendário do agente é exibido ou uma mensagem de fallback é acionada.</td>
  </tr>
</tbody></table>

_&#x200B;**Roteamento Round Robin**&#x200B;_

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Exemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Round Robin pool tem vários agentes; o segundo agente aceita bate-papo depois que o primeiro não aceita.</td>
    <td>O chat se conecta a um segundo agente.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Não há agentes disponíveis no pool de Round Robin; o calendário de reuniões está habilitado.</td>
    <td>O calendário é exibido para o primeiro agente na lista (se configurado) ou a mensagem de fallback é exibida.</td>
  </tr>
  <tr>
    <td>Nenhum agente de fallback</td>
    <td>Não há agentes disponíveis; o fallback está desabilitado.</td>
    <td>Uma mensagem de fallback estática é mostrada ao visitante.</td>
  </tr>
</tbody></table>

### Notificação de pulso {#pulse-notification}

Sempre que um visitante solicita conexão com um agente, fornecemos uma notificação no aplicativo e do navegador para o agente. Mas, às vezes, os agentes perdem esses chats.

Com esta versão, o agente ativo pode receber uma notificação por email, pelo Slack, pelo aplicativo ou pelo navegador quando um(a) novo(a) visitante tem interesse em conversar.

1. Na página inicial da Adobe Experience Cloud, clique no ícone Conta e selecione **Preferências**.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Role a tela para baixo até _Notificações_ e escolha as opções desejadas no Dynamic Chat.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>O conteúdo de uma notificação de pulso pode ser o mesmo que usamos para notificações do aplicativo e do navegador.
