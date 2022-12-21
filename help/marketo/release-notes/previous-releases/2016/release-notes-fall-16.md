---
unique-page-id: 11384018
description: Notas de versão - Último trimestre de 2016 - Documentos da Marketo - Documentação do produto
title: Notas de versão - Último trimestre de 2016
exl-id: da935951-162e-426c-acf2-12c55ff706b4
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 2%

---

# Notas de versão: outono de 16 {#release-notes-fall}

Os recursos a seguir estão incluídos na versão lançada no último trimestre de 160. Verifique sua edição do Marketo para ver a disponibilidade dos recursos. Clique nos links de título para exibir os artigos detalhados de cada recurso.

## Conteúdo preditivo no email {#predictive-content-in-email}

Há uma nova experiência do usuário para que nosso aplicativo de Conteúdo preditivo rastreie, gerencie e recomende seu conteúdo por meio de nosso aprendizado de máquina e algoritmos preditivos na Web e nos canais de email.

>[!NOTE]
>
>Todos os clientes com o módulo Predictive serão ativados até 10 de janeiro.

![](assets/shafe.png)

Agora você pode adicionar conteúdo preditivo ao seu email. Quando o email é aberto, o recipient recebe automaticamente conteúdo relevante e recomendado que ajuda a aumentar a participação e as conversões do conteúdo.

![](assets/predictive.png)

## [Conversões off-line do Facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md) {#facebook-offline-conversions}

Com a integração do Facebook Offline Conversions , os dados de conversão no Marketo (para leads de anúncios) são automaticamente enviados de volta ao Facebook para que sua equipe de publicidade possa otimizar melhor seus gastos com anúncios. Neste Relatório do Facebook Ad Manager, as conversões offline são destacadas.

![](assets/facebook.png)

## [ID universal](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md) {#universal-id}

Uma ID universal permite que você acesse várias assinaturas do Marketo com um único logon e alterne entre assinaturas rapidamente. Você pode usar um único perfil de comunidade para todas as suas assinaturas.

![](assets/image2016-11-3-15-3a10-3a16.png)

>[!NOTE]
>
>Entre em contato com o Suporte da Marketo para ativar esse recurso.

## Aprimoramentos de marketing baseado em conta do Marketo {#marketo-account-based-marketing-enhancements}

Agora, é possível atribuir equipes de conta a contas nomeadas no Marketing Baseado em Conta (ABM), por exemplo, proprietário da conta, representante de desenvolvimento de vendas, representante de desenvolvimento de negócios e gerente de sucesso do cliente. Você também pode criar listas de conta específicas do proprietário da conta e enviar relatórios ABM semanais personalizados para a equipe de conta.

![](assets/account-team-11-15-16.png)

**API REST**

Essa versão também permite gerenciar atributos de conta nomeados e pontuações de contas no ABM usando a API REST do Marketo. Para obter mais detalhes sobre as operações da API, visite o [Site de desenvolvedores do Marketo](https://developers.marketo.com/rest-api/lead-database/named-accounts).

## [Melhorias da trilha de auditoria](/help/marketo/product-docs/administration/audit-trail/change-details-in-audit-trail.md) {#audit-trail-enhancements}

A trilha de auditoria fornece um histórico abrangente das alterações feitas na sua assinatura do Marketo. Adicionamos recursos de rastreamento adicionais para programas, além de descobrir detalhes importantes de alterações para campanhas inteligentes, listas inteligentes e alterações feitas a usuários e funções.

## [Novas permissões](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md) {#new-permissions}

**Tornar e-mail operacional**

Foram-se os dias em que você teve de se preocupar com o envio de emails transacionais para pessoas no seu banco de dados que cancelaram a assinatura. Agora você pode especificar quais usuários podem tornar um email operacional ou editar emails operacionais.

**Editar restrições de campanha**

Por que definir [restrições de campanha](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) se você não pode aplicá-las? Ao definir Configurações de limite de campanha para restringir o número de pessoas no banco de dados que podem ser alvos de uma única campanha, agora é possível restringir quais usuários podem substituir essas configurações ao agendar uma campanha.

## [Som para notificações por push móveis](/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md) {#sound-for-mobile-push-notifications}

Forneça mais riqueza à notificação por push do iOS, ativando o som. Esse novo recurso permite que você acione um som quando a Notificação por push for exibida no dispositivo móvel.

>[!NOTE]
>
>* Os proprietários de dispositivos podem optar por impedir a reprodução de sons nas configurações do dispositivo, e os desenvolvedores de aplicativos podem fornecer aos proprietários de dispositivos opções no aplicativo para impedir a reprodução de sons.
>* Os sons são reproduzidos automaticamente quando uma Notificação por push é exibida em um dispositivo Android.


![](assets/sound-for-push-notifications.png)

## [Insight de vendas compatível com a criptografia do Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) {#sales-insight-compatible-with-salesforce-encryption}

O Market Sales Insight agora é compatível com o Salesforce Shield Encryption. Todos os clientes do Sales Insight devem atualizar para esse pacote gerenciado mais recente (versão 1.4359.2), que é [disponível no Appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO).

## [APIs de contas nomeadas](https://developers.marketo.com/rest-api/lead-database/named-accounts/) {#named-accounts-apis}

Com esta versão, os usuários do Marketo ABM podem gerenciar contas nomeadas por meio da API de contas nomeadas. Os usuários podem criar, atualizar e excluir contas nomeadas, bem como ler e atualizar as pontuações da conta nomeada ABM.

## [Suporte à API do Editor de email v2.0](https://developers.marketo.com/rest-api/assets/emails/) {#email-editor-v-api-support}

Gerencie variáveis e módulos para emails no formato v2.0 usando a API REST do Marketo.

## [Alterações na Sincronização do Marketo Salesforce](https://nation.marketo.com/docs/DOC-3840) {#changes-to-marketo-salesforce-sync}

A integração do Salesforce da Marketo está evoluindo para melhorar a forma como os campos do Marketo são sincronizados com o Salesforce. Agora, em vez de ter que sincronizar um grande grupo de campos que pode ser ou não necessário, você pode escolher e escolher quais campos deseja incluir. Consulte nossa documentação aqui para obter mais informações: [https://nation.marketo.com/docs/DOC-3840](https://nation.marketo.com/docs/DOC-3840).
