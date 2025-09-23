---
description: Visão geral do Adobe Identity Management - Documentação do Marketo - Documentação do produto
title: Visão geral do Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 2%

---

# Visão geral do Adobe Identity Management {#adobe-identity-management-overview}

Todas as novas assinaturas do Adobe Marketo Engage (31 de julho de 2023 ou posterior) são integradas ao Adobe Identity Management System. Atualmente, as assinaturas do Marketo Engage existentes estão sendo migradas para o Adobe Identity Management System após qualquer evento de vendas, que inclui renovações, eventos de recontratação e/ou adendos. As migrações fora de um evento de vendas são compatíveis a partir de outubro de 2024. Os administradores do Marketo receberão uma notificação com 2 a 4 semanas de antecedência se houver planos de que sua assinatura seja migrada para fora de um evento de vendas.

>[!NOTE]
>
>O Suporte da Marketo não pode fornecer atualizações relacionadas à migração do Adobe IMS. A equipe de conta da Adobe entrará em contato com a linha do tempo estimada nos próximos meses. Para obter mais informações, consulte [este artigo](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"} e as [Perguntas frequentes](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

Para assinaturas integradas à identidade do Adobe, o Adobe Admin Console é usado para gerenciamento de usuários. Conceitos relacionados à identidade, como Logon único, também são gerenciados no Admin Console.

* Encontre mais informações sobre a [Adobe Admin Console](https://helpx.adobe.com/br/enterprise/using/admin-console.html){target="_blank"}.
* Encontre mais informações sobre [como configurar sua organização da Adobe relacionada à sua assinatura do Marketo](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Se você quiser implementar o Logon único e sua assinatura tiver sido integrada à Adobe Identity sem o SSO implementado na Organização da Adobe, envie um tíquete para o [Suporte da Marketo](https://nation.marketo.com/){target="_blank"} e especifique o tópico como &quot;Marketo no Admin Console, implementando o SSO&quot;.

## Níveis de perfil {#profile-levels}

As assinaturas do Adobe Marketo Engage integradas ao Sistema Adobe Identity Management são compatíveis com vários perfis. A seguir estão os tipos de perfis de usuário relevantes nessa integração.

<table>
 <tr>
  <td><strong>Administrador de sistema do Adobe Admin Console</strong></td>
  <td>Responsável pela configuração de conceitos de identidade para a organização da Adobe e o produto Marketo Engage na Adobe Admin Console. Função concedida na configuração da organização da Adobe.</td>
 </tr>
 <tr>
  <td><strong>Administrador de produto do Adobe Admin Console</strong></td>
  <td>Responsável por conceder aos usuários o direito ao produto Marketo Engage na Adobe Admin Console. Função concedida no Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Administrador do perfil de produto do Adobe Admin Console</strong></td>
  <td>Responsável por administrar usuários em um perfil de produto. Eles não podem gerenciar usuários fora desse perfil específico. Um administrador de perfil de produto não tem acesso ao aplicativo do Marketo, a menos que seja adicionado ao perfil do produto como um usuário. Sua função ainda seria um usuário padrão (espaço de trabalho padrão se houver mais de um espaço de trabalho).
</td>
 </tr>
 <tr>
  <td><strong>Administrador do Marketo Engage</strong></td>
  <td>Uma pessoa que recebeu acesso ao Marketo Engage com privilégios Administrativos. Função concedida no Marketo Engage, não no Adobe Admin Console (aparece apenas como "Administrador" no modal <b>Editar usuário</b>).</td>
 </tr>
 <tr>
  <td><strong>Usuário do Marketo Engage</strong></td>
  <td>Uma pessoa que recebeu acesso ao Marketo Engage. Sem privilégios administrativos.</td>
 </tr>
</table>

## Perguntas frequentes {#faq}

As Perguntas Frequentes [podem ser encontradas aqui](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Instalação do Administrador](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Adicionar ou remover um administrador de produto](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Adicionar ou remover um usuário](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
