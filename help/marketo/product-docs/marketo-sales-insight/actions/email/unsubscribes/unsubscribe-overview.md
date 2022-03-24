---
description: Visão geral de cancelamento de assinatura - Documentação do Marketo - Documentação do produto
title: Visão geral do cancelamento de inscrição
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Visão geral do cancelamento de inscrição {#unsubscribe-overview}

Está se tornando cada vez mais importante que as organizações estejam em conformidade com as leis de privacidade de e-mails. Para ajudar nisso, fizemos algumas melhorias na nossa experiência de cancelamento de assinatura.

* Links de cancelamento de inscrição são colocados em todos os emails enviados do Marketo Sales e Salesforce (isso não se aplica a emails personalizados enviados do Outlook ou Gmail)
* Administradores podem editar mensagens de cancelamento de inscrição de toda a equipe
* As informações de cancelamento de inscrição são armazenadas no PDV
* Cancelamentos de assinatura podem ser feitos manualmente: Link clicado, Sincronização do Salesforce e Rejeição
* Nova landing page de link de cancelamento de assinatura

## Cancelar assinatura da página de aterrissagem do link {#unsubscribe-link-landing-page}

Quando uma pessoa clica no link de cancelamento de subscrição, ela é levada a uma landing page de cancelamento de assinatura, onde pode selecionar o que ela gostaria de cancelar a assinatura e por quê.

![](assets/unsubscribe-overview-1.png)

Essas informações serão salvas na exibição de detalhes da pessoa para visualização posterior.

## Cancelar assinatura do grupo {#unsubscribe-group}

Veja e gerencie todas as pessoas sem assinatura em um único lugar.

![](assets/unsubscribe-overview-2.png)

Use a barra de pesquisa para procurar qualquer pessoa que não tenha assinado.

![](assets/unsubscribe-overview-3.png)

Se você for um administrador, poderá acessar o grupo de cancelamento de inscrição para filtrar por Cancelamento de Conta e ver todos os cancelamentos de assinatura que foram coletados no banco de dados de pessoas.

![](assets/unsubscribe-overview-4.png)

## Cancelar assinatura do cartão do histórico {#unsubscribe-history-card}

O Cartão do Histórico de Cancelamento de Inscrição ajuda administradores e usuários a obter informações contextuais sobre o histórico de cancelamento de inscrição de seus contatos. Navegue até a guia Pessoas e selecione uma pessoa. Está na parte inferior da guia Sobre na Exibição de detalhes da pessoa.

>[!NOTE]
>
>Só haverá um cartão Cancelar inscrição no Histórico se a pessoa tiver _resubscrid_ em algum momento.

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Data</strong></td> 
   <td><p>Mostra a data em que o cancelamento de inscrição/reinscrição ocorreu.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Detalhes</strong></td> 
   <td><p>Subscrever: Um administrador do Sales Connect removeu manualmente a assinatura do registro de contato. Também pode mostrar alguns detalhes relacionados ao porquê da unsubscription do contato.</p><p>Cancelar assinatura: A assinatura do contato foi cancelada.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Fonte</strong></td> 
   <td><p>Sincronização Salesforce: O cancelamento de inscrição foi capturado por uma sincronização do Salesforce.</p><p>Manual: O usuário clicou no botão cancelar inscrição para recusar.</p><p>Link clicado: O destinatário de um email clicou no link de cancelamento de inscrição.</p><p>"Nome do administrador": O nome de um administrador será exibido quando a ação for reinscrever os contatos. Isso permite que os usuários saibam quem removeu a assinatura.</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Personalizar mensagem de link de cancelamento de assinatura](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
