---
description: Lista de verificação de configuração antecipada - Documentação do Marketo - Documentação do produto
title: Lista de verificação de configuração antecipada
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 1%

---

# NOVA ÁREA: Lista de verificação de configuração antecipada {#early-setup-checklist}

Texto de introdução.

## Marketo Engage no Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administrador de assinatura e produto Marketo Engage </td>
    <td><li>Confirme se você recebeu uma função de Administrador de produto do Adobe pelo Administrador de sistema da organização Adobe.</li>  
    <ul>
    <li>Contato <a href="https://helpx.adobe.com/contact.html">Atendimento ao cliente Adobe</a> para descobrir quem na sua organização possui <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Administrador de sistema do Adobe Admin Console</a> privilégios.</li></ul>
    <li>Aceite o convite do "Administrador de produto do Marketo Engage" para ativar seu Adobe ID. A variável <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">email de boas-vindas</a> é enviado quando a função é atribuída na Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Perfis de produto</td>
    <td><li>Atribuir todos os usuários apropriados ao Marketo Engage <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Perfil do produto</a> no Adobe Admin Console.</li>
    <ul>
    <li>Não é possível atribuir funções de usuários no Marketo Engage/Admin/Usuários e funções antes de adicioná-los a um Perfil de produto.</li>
    <li>Cada assinatura será um Perfil de produto independente. Se um usuário indesejado for adicionado a vários perfis de produto (por exemplo, sandbox de produção e teste), você deverá excluir o usuário de todos os perfis de produto. Caso contrário, eles ainda terão acesso ao Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Usuários</td>
    <td><li>Criar uma política sobre quando fazer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">criar um usuário</a>.</li> <li>Crie uma política sobre quando remover usuários.</li>
    <li>Determine quem deveria ter <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Permissões de administrador de sistema do Adobe e administrador de produto do Marketo Engage.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Adicionar usuários</a> ao Perfil do produto desejado.</li>
    <li>Crie um usuário de API para cada caso de uso de API.</li></td>
  </tr>
  <tr>
    <td>Administrador de suporte ao produto </td>
    <td><li>Para <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">enviar um tíquete de suporte no Adobe Admin Console</a>, você precisa ter a função de ‘Administrador de suporte do produto’ atribuída por um Administrador do sistema às assinaturas que você gerencia. Somente um administrador do sistema em sua organização pode <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">atribuir a você esta função</a>.</li>
    <li>Você pode ter recebido um email do Administrador do sistema informando que você é o Administrador de suporte da sua assinatura do Marketo Engage. Em caso afirmativo, clique em <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">'Introdução' no email</a> para ingressar na organização.</li>
    <li>Determine os contatos apropriados (com pelo menos um contato de backup) e faça com que o administrador do sistema atribua antecipadamente a função de administrador de suporte do produto.</li></td>
  </tr>
</tbody>
</table>

## Configuração do Dynamic Chat no Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

TEXTO

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Subscrição e administrador de produto do Dynamic Chat (se aplicável) </td>
    <td><li>Confirme se você recebeu uma função de Administrador de produto do Adobe pelo Administrador de sistema da organização Adobe. Contato <a href="https://helpx.adobe.com/contact.html">Atendimento ao cliente Adobe</a> para descobrir quem na sua organização tem privilégios de administrador no console.</li>
    <li>Aceitar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">o convite 'Dynamic Chat Product Admin'</a>. A variável <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">email de boas-vindas</a> é enviado quando o Dynamic Chat está ativado na sua instância Marketo Engage e você é designado como um Administrador do sistema.</li></td>
  </tr>
  <tr>
    <td>Perfis de produto </td>
    <td><li>Atribua todos os usuários apropriados a um Perfil de produto do Dynamic Chat no Adobe Admin Console.</li> 
    <ul>
    <li>Se um usuário indesejável for adicionado a vários perfis de produto, você deverá excluir o usuário de todos os perfis de produto. Caso contrário, eles ainda terão acesso ao Dynamic Chat.</li>
    <li>Você pode <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">editar perfis de produto no Dynamic Chat</a> e criar um perfil personalizado com um conjunto personalizado de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">permissões disponíveis em sua assinatura</a>.</li></td>
  </tr>
  <tr>
    <td>Usuários </td>
    <td><li>Crie uma política sobre quando adicionar e remover um usuário do chat.</li>
    <li>Criar uma política sobre quem deve ter <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Permissões de administrador de produto do Adobe Dynamic Chat.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Adicione usuários ao Perfil de produto desejado</a>.</li></td>
  </tr>
</tbody>
</table>

## Configurar atualizações e comunicações contínuas do sistema

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Atualizações de status do Adobe Marketo </td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Inscrever-se para obter atualizações de status do Adobe Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Notificações </td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Assinar notificações de administrador</a> para problemas críticos, como erros nas Campanhas inteligentes e problemas críticos encontrados na sincronização do CRM.</li></td>
  </tr>
</tbody>
</table>
