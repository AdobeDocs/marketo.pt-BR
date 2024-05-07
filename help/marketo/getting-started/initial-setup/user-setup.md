---
description: Antes de mergulhar na nova instância do Marketo Engage, você precisará concluir algumas etapas fundamentais para o uso contínuo. Essas etapas incluem a configuração da conta do usuário, a configuração do administrador de suporte e a assinatura de atualizações de sistema em andamento.
title: Lista de verificação de configuração do usuário
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 7805983cdaff0b99a38aefc2c2467b53f3386da3
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Lista de verificação de configuração do usuário {#user-setup-checklist}

Agora que você concluiu todas as [etapas iniciais de configuração](/help/marketo/getting-started/initial-setup/setup-steps.md), é hora de estabelecer alguns elementos fundamentais para garantir um uso contínuo e sem problemas. Isso estabelecerá a base para sua jornada com o Marketo Engage e ajudará você a aproveitar ao máximo seus recursos. Vamos começar!

>[!NOTE]
>
>Você também pode baixar essa lista de verificação, [junto com uma lista de práticas recomendadas](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) para a nova instância e confira as etapas conforme avança.

## Marketo Engage no Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

Suas novas assinaturas do Marketo Engage são integradas no [Sistema Adobe Identity Management (IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html). Prossiga para a seguinte análise do gerenciamento de usuários no Adobe Admin Console.

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administrador de assinatura e produto Marketo Engage</td>
    <td><li>Confirme se você recebeu uma função de Administrador de produto do Adobe pelo Administrador de sistema da organização Adobe.</li>  
    <ul>
    <li>Contato <a href="https://helpx.adobe.com/contact.html">Atendimento ao cliente Adobe</a> para descobrir quem na sua organização possui <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Administrador de sistema do Adobe Admin Console</a> privilégios.</li></ul>
    <li>Aceite o convite do "Administrador de produto do Marketo Engage" para ativar seu Adobe ID. A variável <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">email de boas-vindas</a> é enviado quando a função é atribuída na Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Perfis de produto</td>
    <td><li>Atribuir todos os usuários desejados ao Marketo Engage <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Perfil do produto</a> no Adobe Admin Console.</li>
    <ul>
    <li>Não é possível atribuir funções de usuários em Marketo Engage &gt; Admin &gt; Usuários e funções antes de adicioná-los a um Perfil de produto.</li>
    <li>Cada assinatura será um Perfil de produto independente. Se um usuário indesejado for adicionado a vários perfis de produto (por exemplo, sandbox de produção e teste), você deverá excluir o usuário de todos os perfis de produto. Caso contrário, eles ainda terão acesso ao Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Usuários</td>
    <td><li>Criar uma política sobre quando fazer <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">criar um usuário</a>.</li> <li>Crie uma política sobre quando remover usuários.</li>
    <li>Determine quem deveria ter <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Permissões de administrador de sistema do Adobe e administrador de produto do Marketo Engage.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Adicionar usuários</a> ao Perfil do produto desejado.</li>
    <li>Crie um usuário de API para cada caso de uso de API.</li></td>
  </tr>
  <tr>
    <td>API de gerenciamento de usuários (se aplicável)</td>
    <td><li>Use o <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">API de gerenciamento de usuários do Adobe</a> para convidar, atualizar e excluir usuários.</li>
    <li>Use o <a href="https://developer.adobe.com/umapi/">API de gerenciamento de usuários do Adobe</a> para adicionar ou remover funções (por exemplo, administradores, administradores de suporte, desenvolvedores).</li>
    </td>
  </tr>
  <tr>
    <td>Administrador de suporte ao produto</td>
    <td><li>Para <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">enviar um tíquete de suporte no Adobe Admin Console</a>, você precisa ter a função de ‘Administrador de suporte do produto’ atribuída por um Administrador do sistema às assinaturas que você gerencia. Somente um administrador do sistema em sua organização pode <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">atribuir a você esta função</a>.</li>
    <li>Você pode ter recebido um email do Administrador do sistema informando que você é o Administrador de suporte da sua assinatura do Marketo Engage. Em caso afirmativo, clique em <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">'Introdução'</a> no email para ingressar na organização.</li>
    <li>Determine os contatos apropriados (com pelo menos um contato de backup) e peça ao administrador do sistema que atribua a função de administrador de suporte do produto de acordo.</li></td>
  </tr>
</tbody>
</table>

## Configuração do Dynamic Chat no Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

Para usar [Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html), o canal nativo de automação de conversas no Marketo Engage, prossiga com a configuração de permissões do usuário, seguindo as etapas abaixo na [Adobe Admin Console](https://adminconsole.adobe.com/).

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Subscrição e administrador de produto do Dynamic Chat (se aplicável)</td>
    <td><li>Confirme se você recebeu uma função de Administrador de produto do Adobe pelo Administrador de sistema da organização Adobe. Contato <a href="https://helpx.adobe.com/contact.html">Atendimento ao cliente Adobe</a> para descobrir quem na sua organização tem privilégios de administrador no console.</li>
    <li>Aceite o <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">'Administrador de produto do Dynamic Chat'</a> convidar. A variável <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">email de boas-vindas</a> é enviado quando o Dynamic Chat está ativado na sua instância Marketo Engage e você é designado como um Administrador do sistema.</li></td>
  </tr>
  <tr>
    <td>Perfis de produto</td>
    <td><li>Atribua todos os usuários desejados ao Perfil de produto do Dynamic Chat no Adobe Admin Console.</li> 
    <ul>
    <li>Se um usuário indesejável for adicionado a vários perfis de produto, você deverá excluir o usuário de todos os perfis de produto. Caso contrário, eles ainda terão acesso ao Dynamic Chat.</li>
    <li>Você pode <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">editar perfis de produto no Dynamic Chat</a> e criar um perfil personalizado com um conjunto personalizado de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">permissões disponíveis em sua assinatura</a>.</li></td>
  </tr>
  <tr>
    <td>Usuários</td>
    <td><li>Crie uma política sobre quando adicionar e remover um usuário do chat.</li>
    <li>Criar uma política sobre quem deve ter <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Permissões de administrador de produto do Adobe Dynamic Chat.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Adicione usuários ao Perfil de produto desejado</a>.</li></td>
  </tr>
</tbody>
</table>

## Configurar atualizações e comunicações contínuas do sistema {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Atualizações de status do Adobe Marketo</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Inscrever-se para obter atualizações de status do Adobe Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Notificações</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Assinar notificações de administrador</a> para problemas críticos, como erros nas Campanhas inteligentes e problemas críticos encontrados na sincronização do CRM.</li></td>
  </tr>
</tbody>
</table>

<p>

Agora que sua conta Marketo Engage está pronta para ser ativada, consulte nossa [Práticas recomendadas para uma nova instância do Marketo Engage](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md) para obter o máximo do seu investimento e preparar-se para o sucesso a longo prazo.
