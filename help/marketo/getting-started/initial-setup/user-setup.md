---
description: Antes de se aprofundar na nova instância do Marketo Engage, você precisa concluir algumas etapas básicas para o uso contínuo do recurso. Essas etapas incluem configurar uma conta de usuário, configurar o suporte de admin e assinar as atualizações contínuas do sistema.
short-description: Depois de concluir as etapas de configuração iniciais, saiba como estabelecer elementos fundamentais para garantir o uso contínuo do recurso.
title: Lista de verificação de configuração do usuário
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 7%

---

# Lista de verificação de configuração do usuário {#user-setup-checklist}

Agora que você concluiu todas as [etapas iniciais de configuração](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"}, é hora de estabelecer alguns elementos fundamentais para garantir um uso contínuo e sem problemas. Isso estabelecerá a base para sua jornada com o Marketo Engage e ajudará você a aproveitar ao máximo seus recursos. Vamos começar!

>[!NOTE]
>
>Você também pode baixar esta lista de verificação, [juntamente com uma lista de práticas recomendadas](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) para sua nova instância, e verificar as etapas conforme você avança.

## Marketo Engage no Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

Suas novas assinaturas do Marketo Engage estão integradas ao [Adobe Identity Management System (IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=pt-BR). Prossiga para a seguinte análise do gerenciamento de usuários no Adobe Admin Console.

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administração de produtos de assinatura e Marketo Engage</td>
    <td><li>Confirme se você recebeu uma função de Administrador de produto do Adobe pelo Administrador do sistema da organização da Adobe.</li>
    <ul>
    <li>Entre em contato com a equipe de conta da Adobe (seu Gerente de conta) ou envie um email para <code>marketocares@marketo.com</code> para descobrir quem na sua organização tem os privilégios de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=pt-BR">Administrador do Sistema do Adobe Admin Console</a>.</li></ul>
    <li>Aceite o convite do "Administrador de produto do Marketo Engage" para ativar seu Adobe ID. O <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=pt-BR#create-a-product-profile">email de boas-vindas</a> é enviado quando a função é atribuída na Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Perfis de produto</td>
    <td><li>Atribua todos os usuários desejados ao <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Perfil de Produto</a> do Marketo Engage no Adobe Admin Console.</li>
    <ul>
    <li>Não é possível atribuir funções de usuários em Marketo Engage &gt; Admin &gt; Usuários e funções antes de adicioná-las a um Perfil de produto.</li>
    <li>Cada assinatura será um Perfil de produto independente. Se um usuário indesejado for adicionado a vários perfis de produto (por exemplo, sandbox de produção e teste), você deverá excluir o usuário de todos os perfis de produto. Caso contrário, eles ainda terão acesso ao Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Usuários</td>
    <td><li>Crie uma política sobre quando <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html?lang=pt-BR">criar um usuário</a>.</li> <li>Crie uma política sobre quando remover usuários.</li>
    <p><img src="assets/note-icon.png" alt="ícone de nota"> NOTA: você precisa ser um administrador do sistema para remover usuários.
    <li>Determine quem deve ter <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=pt-BR">permissões de Administrador do Sistema do Adobe e Administrador do Produto Marketo Engage.</a> <li><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Adicione usuários</a> ao Perfil de Produto desejado.</li>
    <li>Crie um usuário de API para cada caso de uso de API.</li></td>
  </tr>
  <tr>
    <td>API de gerenciamento de usuários (se aplicável)</td>
    <td><li>Use a <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">API de Gerenciamento de Usuários do Adobe</a> para convidar, atualizar e excluir usuários.</li>
    <li>Use a <a href="https://developer.adobe.com/umapi/">API de Gerenciamento de Usuários do Adobe</a> para adicionar ou remover funções (por exemplo, Administradores, Administradores de Suporte, Desenvolvedores).</li>
    </td>
  </tr>
  <tr>
    <td>Administrador de suporte ao produto</td>
    <td><li>Para <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=pt-BR#create-a-support-ticket-with-admin-console">enviar um tíquete de suporte no Adobe Admin Console</a>, você precisa ter a função de 'Administrador de Suporte do Produto' atribuída por um Administrador do Sistema às assinaturas que você gerencia. Somente um Administrador do Sistema em sua organização pode <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html?lang=pt-BR#assign-the-support-admin-role">atribuir a você esta função</a>.</li>
    <li>Você pode ter recebido um email do Administrador do sistema informando que você é o Administrador de suporte da sua assinatura do Marketo Engage. Em caso afirmativo, clique em <a href="https://experienceleague.adobe.com/pt-br/docs/customer-one/using/home#assign-the-support-admin-role">'Introdução'</a> no email para ingressar na organização.</li>
    <li>Determine os contatos apropriados (com pelo menos um contato de backup) e peça ao administrador do sistema que atribua a função de administrador de suporte do produto de acordo.</li></td>
  </tr>
</tbody>
</table>

## Configuração do Dynamic Chat no Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

Para usar o [Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html?lang=pt-BR), o canal nativo de automação de conversas no Marketo Engage, prossiga com a configuração de permissões do usuário seguindo as etapas abaixo no [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}.

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
    <td><li>Confirme se você recebeu uma função de Administrador de produto do Adobe pelo Administrador do sistema da organização da Adobe.</li>
    <ul><li>Entre em contato com a equipe de conta da Adobe (seu Gerente de conta) ou envie um email para <code>marketocares@marketo.com</code> para descobrir quem na sua organização tem os privilégios de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html?lang=pt-BR">Administrador do Sistema do Adobe Admin Console</a>.</li></ul>
    <li>Aceite o convite de <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=pt-BR">'Administrador de produto do Dynamic Chat'</a>. O <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html?lang=pt-BR">email de boas-vindas</a> é enviado quando o Dynamic Chat é habilitado na sua instância do Marketo Engage e você é designado como um Administrador do Sistema.</li></td>
  </tr>
  <tr>
    <td>Perfis de produto</td>
    <td><li>Atribua todos os usuários desejados ao Perfil de produto do Dynamic Chat no Adobe Admin Console.</li>
    <ul>
    <li>Se um usuário indesejado for adicionado a vários Perfis de produto, você deverá excluir o usuário de todos os perfis de produto. Caso contrário, eles ainda terão acesso ao Dynamic Chat.</li>
    <li>Você pode <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">editar Perfis de Produtos no Dynamic Chat</a> e criar um perfil personalizado com um conjunto personalizado de <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">permissões disponíveis em sua assinatura</a>.</li></td>
  </tr>
  <tr>
    <td>Usuários</td>
    <td><li>Crie uma política sobre quando adicionar e remover um usuário do chat.</li>
    <li>Crie uma política sobre quem deve ter <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">permissões de Administrador de Produto do Adobe Dynamic Chat.</a></li>
    <li><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Adicione usuários ao Perfil de Produto desejado</a>.</li></td>
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
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Inscrever-se para obter atualizações do Adobe Marketo Engage Status</a>.</li></td>
  </tr>
  <tr>
    <td>Notificações</td>
    <td><li><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Assine as notificações de administrador</a> para ver problemas críticos, como erros nas Campanhas Inteligentes e problemas críticos encontrados na sincronização do CRM.</li></td>
  </tr>
</tbody>
</table>

<p>

Agora que sua conta do Marketo Engage está pronta para uso, revise nossa seção [Práticas recomendadas para uma nova instância do Marketo Engage](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"} para obter o máximo de seu investimento e se preparar para o sucesso a longo prazo.
