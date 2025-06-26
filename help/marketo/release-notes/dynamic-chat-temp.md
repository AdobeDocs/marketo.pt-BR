---
description: Notas de versão do Dynamic Chat - Documentação do Marketo - Documentação do produto
title: Notas de versão do Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: ce7142e471271dfb33b265e226b67bcc3b35594b
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 4%

---

# Notas de versão do Dynamic Chat {#dynamic-chat-release}

As versões do Adobe Dynamic Chat operam em um modelo de entrega contínua que permite uma abordagem mais escalável para a implantação de recursos. Às vezes, há várias versões em um mês, portanto, verifique regularmente para obter as informações mais atualizadas.

A página de Notas de Versão padrão do Marketo Engage [pode ser encontrada aqui](/help/marketo/release-notes/current.md){target="_blank"}.

## Versão de junho de 2025 {#june-25-release}

### Renovação da Lógica de Roteamento {#routing-logic-revamp}

Renovamos a lógica de roteamento de chat ao vivo no Dynamic Chat para garantir um comportamento de envolvimento mais inteligente e previsível em todos os tipos de roteamento (Conta, Personalizado, Equipe e Round Robin). A nova lógica simplifica os fluxos de roteamento e melhora o tratamento de fallback quando os agentes estão indisponíveis.

#### Principais melhorias no comportamento de roteamento

* **Até duas tentativas de envolvimento por sessão**

   * O sistema tentará se conectar com no máximo dois agentes, mas estritamente dentro da regra de roteamento principal.

   * Se um agente estiver disponível, mas não responder (por exemplo, recusar ou perder), o sistema tentará um segundo agente do mesmo pool.

   * A lógica de fallback (como Round Robin) só será ativada se nenhum agente elegível for encontrado durante a resolução inicial — para não tentar novamente após uma falha no engajamento.

* **Comportamento Específico da Regra de Roteamento**

_&#x200B;**Roteamento de conta**&#x200B;_

Se o domínio de email de um visitante for mapeado para uma Conta conhecida, o agente mapeado sempre será priorizado.

Se o agente estiver disponível, o chat será roteado diretamente para ele.

Se o agente não estiver disponível, o sistema:

Não tenta outro agente, mesmo se Round Robin estiver habilitado como fallback.

Em vez disso, ele:

Mostra o calendário de reuniões do agente mapeado (se estiver habilitado) ou

Retorna a uma mensagem padrão (pior caso).

A regra de roteamento no nível do cartão (por exemplo, Equipe, Personalizado) só será considerada se o Roteamento de conta não for elegível (nenhum domínio ou agente correspondente).

_&#x200B;**Roteamento personalizado/de equipe**&#x200B;_

Essas regras podem retornar vários agentes qualificados.

Se o primeiro agente disponível não interagir, o sistema tentará mais um agente da mesma lista.

O fallback Round Robin não é acionado apenas porque um agente não respondeu.

Se nenhum dos agentes interagir:

O sistema mostra o calendário do agente da primeira tentativa (se ativado) ou

Exibe a mensagem de fallback padrão.

_&#x200B;**Roteamento Round Robin**&#x200B;_

Quando usado como uma regra de roteiro principal, o sistema:

Tenta engajar o primeiro agente disponível do pool round robin.

Se o primeiro não responder, ele tentará novamente com o próximo melhor agente qualificado.

Se Round Robin for usado como fallback, ele será ativado somente se nenhum agente for resolvido a partir da regra principal.

**Fluxo de experiência do visitante**

O sistema verifica se o Roteamento de Conta é aplicável.

Se sim e o agente estiver disponível → se conecta imediatamente.

Se não for elegível ou o agente não estiver disponível → prosseguirá para a regra de roteamento no nível da placa.

A regra de roteamento no nível do cartão (Personalizada, Equipe, Round Robin) é avaliada.

A disponibilidade dos agentes qualificados é verificada (permissões, status).

O sistema envolve um agente e, se necessário, tenta um segundo agente da mesma regra.

Se nenhum engajamento for bem-sucedido → a lógica de fallback for aplicada:

Fallback de calendário (se ativado) ou

Mensagem padrão.

O fallback de Round Robin só é considerado quando nenhum agente elegível for encontrado na regra de roteamento principal, e não quando os agentes individuais não responderem.

**Casos de uso**

Roteamento de Conta

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Exemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>O domínio do visitante mapeia para uma conta; o agente mapeado tem o chat ao vivo ativado e está disponível</td>
    <td>O chat se conecta diretamente ao agente mapeado</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>O agente mapeado não está disponível, o fallback Round Robin está habilitado</td>
    <td>O sistema seleciona um agente disponível por meio do Round Robin e os envolve </td>
  </tr>
  <tr>
    <td>Nenhum agente de fallback</td>
    <td>O agente mapeado está indisponível, sem fallback de Round Robin; a reserva de reunião está habilitada</td>
    <td>O sistema mostra o calendário do agente mapeado ou exibe uma mensagem de fallback padrão</td>
  </tr>
</tbody></table>

Roteamento personalizado

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Exemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>Nenhum agente de fallback</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
</tbody></table>

Roteamento da equipe

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Exemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>Nenhum agente de fallback</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
</tbody></table>

Roteamento Round Robin

<table><thead>
  <tr>
    <th>Tipo</th>
    <th>Exemplo</th>
    <th>Resultado</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
  <tr>
    <td>Nenhum agente de fallback</td>
    <td>TEXTO</td>
    <td>TEXTO</td>
  </tr>
</tbody></table>

### Notificação de Pulso {#pulse-notification}

Sempre que um visitante solicita conexão com um agente, hoje fornecemos ao agente notificações no aplicativo e do navegador, mas os agentes geralmente não veem esses bate-papos.

* Agora, o Live Agent receberá notificações por email, Slack, Inapp e do navegador quando um novo visitante estiver interessado em conversar

* O conteúdo para notificação de pulso pode ser o mesmo que usamos hoje para notificação no aplicativo e no navegador

O comportamento deve ser o mesmo que o atual para que o agente aceite quando vários agentes aceitarem.
