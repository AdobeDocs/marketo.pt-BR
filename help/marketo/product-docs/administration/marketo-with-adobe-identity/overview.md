---
description: Visão geral - Documentação do Marketo - Documentação do produto
title: Visão geral
hide: true
hidefromtoc: true
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: 34860f7b0a94a142c3d29a225203a00c7fb3b79e
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Visão geral {#overview}

Se você tiver uma nova conta com o Adobe Marketo Engage (nova conta, não apenas uma nova instância para uma conta existente) a partir de 15 de fevereiro de 2022, ela poderá vir integrada ao sistema Adobe Identity Management, dependendo do pacote do produto comprado. Para saber se você tem, entre em contato com o administrador da Marketo ou com o gerente de sucesso do cliente da sua conta.

As assinaturas existentes do Marketo serão migradas para o Adobe Identity Management System a partir deste ano.

>[!NOTE]
>
>O Suporte da Marketo não poderá fornecer atualizações relacionadas à migração do Adobe IMS. O Gerente de sucesso do cliente entrará em contato com a linha do tempo estimada para os próximos meses.

## Níveis de perfil

As assinaturas do Adobe Marketo Engage incorporadas ao Adobe Identity Management System oferecem suporte a vários perfis. A seguir estão os tipos de perfis de usuário relevantes nesta integração.

<table>
 <tr>
  <td><strong>Administrador do sistema da Adobe Admin Console</strong></td>
  <td>Responsável pela configuração de conceitos de identidade para o Adobe org e o Marketo Engage product no Adobe Admin Console. Atribuição concedida na configuração da organização do Adobe.</td>
 </tr>
 <tr>
  <td><strong>Administrador de produto do Adobe Admin Console</strong></td>
  <td>Responsável por qualificar os usuários para o produto Marketo Engage no Adobe Admin Console. Atribuição concedida no Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administrador de produto do Marketo Engage</strong></td>
  <td>Uma pessoa a quem tenha sido concedido acesso a Marketo Engage com privilégios administrativos. Atribuição concedida no Marketo Engage, não no Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Usuário do Marketo Engage</strong></td>
  <td>Uma pessoa a quem foi dado acesso ao Marketo Engage. Sem privilégios administrativos.</td>
 </tr>
</table>

## Perguntas frequentes

**O que é Adobe Identity?**

O Adobe Identity Management System consiste em três componentes.

* Serviço de identidade do Adobe: Trata a autenticação e a validação do usuário final, incluindo a federação e o Single-Sign-On (SSO) em tempo de execução.

* Adobe Admin Console: O Admin Console fornece um local central para gerenciar direitos de Adobe em toda a organização. Ele lida com gerenciamento de usuários, serviço em nuvem, direito à licença de desktop, configuração de federação e fornece recursos de segurança para prevenção de perda de dados.

* API de gerenciamento de usuários do Adobe (UMAPI): Permite que as organizações gerenciem usuários e direitos corporativos na Adobe Admin Console no nível da API.

**Quando as assinaturas Marketo Engage existentes serão integradas ao IMS?**

As assinaturas existentes do Marketo serão migradas para o Adobe Identity Management System ainda este ano. O Suporte da Marketo não poderá fornecer atualizações relacionadas à migração do Adobe IMS. O Gerente de sucesso do cliente entrará em contato com a linha do tempo estimada para os próximos meses.

**Qual é a diferença entre um administrador de produto do Adobe e um administrador de Marketo Engage?**

* O Administrador de produto do Adobe é uma nova função na plataforma Marketo.
* A função Administrador de produto do Adobe é concedida aos usuários adicionados como Administrador de produto no Adobe Admin Console
* O Administrador de produto do Adobe é uma função somente leitura e não pode ser editado ou excluído do Marketo Engage.
* O Administrador de produto do Adobe tem os mesmos direitos e privilégios que um Administrador padrão do Marketo.
* A função de Marketo Engage Admin ainda é um Administrador e é concedida a um usuário no Marketo Engage.

**Há alguma alteração no suporte ao cliente da API de gerenciamento de usuários?**

Sim. Aqueles que foram integrados ao Adobe IMS não podem utilizar todas as APIs de gerenciamento de usuários do Marketo existentes. Para ações de convite, atualização e exclusão de usuários, o Adobe [APIs IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html) deve ser usada. Para o gerenciamento de funções, as APIs de gerenciamento de usuários do Marketo ainda se aplicam. Além disso, não há outras alterações no suporte ao cliente da API REST do Marketo.

**Com quem entramos em contato para obter suporte se formos integrados ao IMS?**

Siga o procedimento padrão para entrar em contato com o [Suporte Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

**As funções de usuário do Marketo (em espaços de trabalho) são gerenciadas no Adobe Admin Console?**

Nº O gerenciamento de Função do usuário (em espaços de trabalho) é concluído no Marketo Engage.

**Sou um Administrador do Marketo em uma assinatura integrada do IMS e não tenho acesso ao Admin Console. Como obtenho acesso?**

Qualquer sistema Adobe ou administrador de produto que tenha acesso ao Admin Console de sua organização pode conceder acesso a você. Se você não tem certeza de quem em sua organização tem privilégios de administrador no console, entre em contato com [Atendimento ao cliente do Adobe](https://helpx.adobe.com/contact.html).

**Como um Administrador adicionaria usuários ao Marketo Sales Connect?**

Embora haja um cartão de produto no Admin Console para Sales Connect, o Admin Console não deve ser usado para adicionar/gerenciar usuários. O link a seguir permitirá que Administradores gerenciem usuários por meio do Marketo Sales Connect: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**Onde posso obter mais informações sobre a Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**Ainda vou para a seção Admin no Marketo para fazer alterações na conta do usuário da minha conta?**

Não, você precisaria navegar para [account.adobe.com](https://account.adobe.com).

**Como isso funciona com a ID universal do Marketo?**

Os integrados à identidade do Adobe podem acessar todas as assinaturas habilitadas para IMS facilmente por meio do alternador de assinatura no produto.

**Isso funciona com SSO?**

Sim. A integração do Marketo com o Adobe IMS é compatível com usuários de ID universal e SSO. O SSO agora é orientado pelo Adobe IMS e é configurado no nível da organização na Adobe Admin Console. [Saiba mais aqui](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**Como a autorização do dispositivo funciona?**

No momento, o Adobe IMS não é compatível com nada como o recurso de autorização de dispositivo da Marketo.

**Ainda é possível usar o recurso &quot;Fazer logon na caixa de diálogo do usuário de convite&quot; para tornar o logon de um usuário exclusivo de seu email?**

Nº O fluxo de trabalho de Convite de usuário não está mais ativo quando uma assinatura é habilitada para IMS, portanto, o recurso não é mais válido. A identidade do Adobe requer que a identidade de um usuário seja orientada por seu email.

**Para o Adobe IMS, temos a opção de usar o Adobe ID, o Enterprise ID ou o Federated ID?**

Sim, você determina o tipo de identidade para ter o suporte da organização. Mais informações podem ser encontradas aqui: [Visão geral da identidade](https://helpx.adobe.com/enterprise/using/identity.html) e aqui: [Configurar identidade](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

>[!MORELIKETHIS]
>
>* [Configuração do administrador](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [Adicionar ou remover um administrador de produto](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [Adicionar ou remover um usuário](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

