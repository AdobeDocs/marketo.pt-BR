---
description: Visão geral do cancelamento de inscrição - Documentação do Marketo - Documentação do produto
title: Visão geral do cancelamento de inscrição
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Visão geral do cancelamento de inscrição {#unsubscribe-overview}

É cada vez mais importante que as organizações estejam em conformidade com as leis de privacidade de email. Para ajudar nisso, fizemos algumas melhorias na nossa experiência de cancelamento de inscrição.

* Links de cancelamento de inscrição são colocados em todos os emails enviados do Marketo Sales e do Salesforce (isso não se aplica a emails personalizados enviados do Outlook ou do Gmail)
* Administradores podem editar mensagens de cancelamento de inscrição para toda a equipe
* As informações de cancelamento de inscrição são armazenadas em PDV
* Os cancelamentos de assinatura podem ser feitos manualmente: Link clicado, Sincronização do Salesforce e Rejeição
* Nova página de aterrissagem do link de cancelamento de inscrição

## Página de aterrissagem do link de cancelamento de inscrição {#unsubscribe-link-landing-page}

Quando uma pessoa clica no link para cancelar inscrição, ela é direcionada a uma página de aterrissagem de cancelamento de inscrição, onde é possível selecionar o que gostaria de cancelar a inscrição e por quê.

![](assets/unsubscribe-overview-1.png)

Essas informações serão salvas na exibição de detalhes da pessoa para exibição posterior.

## Cancelar inscrição do grupo {#unsubscribe-group}

Veja e gerencie todas as pessoas que cancelaram sua inscrição em um único local.

![](assets/unsubscribe-overview-2.png)

Use a barra de pesquisa para procurar pessoas não inscritas.

![](assets/unsubscribe-overview-3.png)

Se você for um administrador, acesse o grupo de cancelamento de inscrição para filtrar por Cancelamentos de inscrição de conta e ver todas as cancelamentos de inscrição coletadas no banco de dados de pessoas.

![](assets/unsubscribe-overview-4.png)

## Cancelar inscrição no cartão de histórico {#unsubscribe-history-card}

O Cartão de histórico Cancelar inscrição ajuda administradores e usuários a obter informações contextuais sobre o histórico de cancelamento de inscrição de seus contatos. Navegue até a guia Pessoas e selecione uma pessoa. Está na parte inferior da guia Sobre na Exibição de detalhes da pessoa.

>[!NOTE]
>
>Só haverá um cartão de Histórico de Cancelamento de Inscrição se a pessoa tiver _assinado novamente_ em algum momento.

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Data</strong></td> 
   <td><p>Mostra a data em que ocorreu o cancelamento de inscrição/reinscrição.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Detalhes</strong></td> 
   <td><p>Assinar novamente: um administrador do Sales Connect removeu manualmente o cancelamento de assinatura do registro de contato. Ela também pode mostrar alguns detalhes relacionados ao motivo pelo qual o contato teve a assinatura cancelada.</p><p>Cancelar inscrição: a inscrição do contato foi cancelada.</p></td> 
  </tr> 
  <tr> 
   <td><strong>Origem</strong></td> 
   <td><p>Sincronização do Salesforce: o cancelamento de inscrição foi capturado por uma sincronização do Salesforce.</p><p>Manual: o usuário clicou no botão Cancelar inscrição para recusar.</p><p>Link clicado: o destinatário de um email clicou no link de cancelamento de inscrição.</p><p>"Nome do administrador": o nome de um administrador será exibido quando a ação for reinscrever contatos. Isso informa aos usuários quem removeu o cancelamento de inscrição.</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Personalizar Mensagem do Link de Cancelamento de Inscrição](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
