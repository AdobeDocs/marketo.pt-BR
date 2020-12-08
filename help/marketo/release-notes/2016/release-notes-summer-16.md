---
unique-page-id: 11380218
description: Notas de versão - Verão de 16 - Documentos do Marketo - Documentação do produto
title: Notas de versão - Verão de 16
translation-type: tm+mt
source-git-commit: efadb7eb3845012c273e1a60f9cd98ac884eb543
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---


# Notas de versão: Verão de 16 {#release-notes-summer}

Os seguintes recursos estão incluídos na versão do verão de 16. Verifique sua edição de marketing para ver a disponibilidade de recursos. Clique nos links de título para artigos detalhados de visualização para cada recurso.

## [Marketing baseado em conta](http://docs.marketo.com/display/docs/account+based+marketing) {#account-based-marketing}

O Marketing baseado em conta de marketing fornece todos os recursos básicos em uma única plataforma unificada:

* **Público alvo** - Detecção de conta, Correspondência de cliente a conta e Listas de conta nomeada
* **Envolvimento** - Personalização baseada em conta, envolvimento entre canais e Workflows específicos da conta
* **Medida** - insights em nível de conta e Lista, Pontuação de envolvimento de conta e Impacto de pipeline e receita

![](assets/abm-5-acme.png)

>[!NOTE]
>
>O ABM está disponível como um complemento para sua subscrição de marketing, portanto entre em contato com seu representante de vendas para que ele seja implementado.

## [Trilha de auditoria](http://docs.marketo.com/display/docs/audit+trail) {#audit-trail}

A trilha de auditoria fornece um histórico abrangente das alterações feitas na sua subscrição de marketing. Isso criará responsabilidade entre usuários e administradores, ajudará a identificar a causa do comportamento inesperado e fornecerá a segurança de saber quem está fazendo o quê e quando. Essas informações estarão disponíveis a qualquer momento e poderão ser usadas para responder a perguntas como:

* O que aconteceu com esse ativo ou configuração e quem o atualizou pela última vez?
* O que o usuário X está aprontando?
* Quem está entrando em nossa conta?

![](assets/audit-trail.png)

## [Integração do Marketing-Vibes SMS LaunchPoint](http://docs.marketo.com/display/docs/vibes+sms+messages) {#marketo-vibes-sms-launchpoint-integration}

Crie facilmente mensagens SMS diretamente no Marketo. Personalize e público alvo sua mensagem usando seus dados avançados de marketing e monitore facilmente seu desempenho usando o painel de mensagens SMS.

>[!NOTE]
>
>Este recurso exige que você tenha uma conta Vibes SMS existente.

![](assets/vibes-sms2.png)

## [Aprimoramentos do Email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md) {#email-enhancements}

**Variáveis no nível do módulo**

Anteriormente, todas as variáveis especificadas em Modelos do Email 2.0 eram &quot;globais&quot; no escopo. Ao usar variáveis dentro de módulos, isso nem sempre é desejável se você planeja usar várias instâncias do módulo. Com esta versão, as variáveis agora podem ser especificadas como &quot;nível de módulo&quot;, o que permite indicar que o usuário deve ser capaz de definir valores únicos para cada módulo em que são usadas.

![](assets/module-level-variables.png)

**Atualizações de sintaxe**

* Agora você pode usar &quot;mktoAddByDefault&quot; em módulos especificados em Modelos de e-mail 2.0 para indicar quais módulos devem ser exibidos em novos e-mails por padrão. Isso é muito mais conveniente se você estiver criando um modelo de email com um grande número de módulos.
* Em elementos de imagem, agora é possível especificar se as propriedades &quot;height&quot; e &quot;width&quot; do elemento `<img>` HTML subjacente devem ser bloqueadas ou editáveis para o usuário final. mktoLockImgSize=&quot;true&quot; fará com que a altura/largura sejam bloqueadas (mesmo que a imagem seja alterada). Da mesma forma, mktoLockImgStyle=&quot;true&quot; fará com que a propriedade &quot;style&quot; seja bloqueada.

**Pesquisa de código**

Use a nova funcionalidade de pesquisa para localizar e substituir conteúdo com eficiência no código do seu email. Essa funcionalidade também está disponível no editor de modelo de e-mail.

![](assets/2nd-screenshot.png)

**Suporte a token em elementos de imagem**

Tokens agora podem ser usados na área &quot;URL externo&quot; da experiência de inserção de imagem! Caso tenha especificado imagens com `{{my.tokens}}`, agora é possível fazer referência a esses tokens no Editor de email 2.0. Observe que a imagem ainda aparecerá quebrada na tela do Editor de email 2.0. Mas você verá eles renderizados na Pré-visualização e Enviar amostra antes de enviar seu email.

## [Vários domínios de marca](http://docs.marketo.com/display/docs/add+multiple+branding+domains) {#multiple-branding-domains}

Foram-se os dias em que os links de tracking de email só podiam ser marcados com um único domínio de marca. Agora você pode adicionar vários domínios de marca para inspirar a confiança do consumidor, criar uma aparência mais simplificada para se concentrar na marca, melhorar a capacidade de entrega de e-mail e escolher, por e-mail, qual domínio de marca usar para cada link de rastreamento de e-mail.

![](assets/multiple-branding-domains.png)

## [Tokens de programa](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) {#program-tokens}

Criamos um novo tipo de token para programas. Agora é possível renderizar Nome, Descrição e ID do Programa em ativos e etapas de fluxo de campanha inteligente.

![](assets/program-tokens.png)

## [Chave da empresa](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/authorize-the-marketo-outlook-plugin.md) {#enterprise-key}

Exigir que cada pessoa em sua equipe de vendas instale nosso Plug-in de insight de vendas para Outlook pode ser chato. Introduzimos uma nova maneira de instalar remotamente o plug-in para Outlook usando uma chave corporativa. Envie à sua equipe de TI sua chave exclusiva encontrada na seção Marketing Sales Insight do Administrador e permita que ela faça o resto.

![](assets/enterprise-key.png)

## [Campanhas de personalização da Web](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md) {#web-personalization-campaigns}

Especifique um atraso para que as campanhas da Web reajam em seu site.

![](assets/dialog-campaign-delay.png)

## [Análise de conteúdo e Recommendations Export](/help/marketo/product-docs/web-personalization/understanding-web-personalization/understanding-content-analytics.md) {#content-analytics-and-recommendations-export}

Dados offline de análise de conteúdo de visualização e recomendações.

## [Suporte à API para o Editor de e-mail 2.0](http://developers.marketo.com/documentation/asset-api/) {#api-support-for-email-editor}

As APIs de ativos pré-existentes, anteriormente compatíveis apenas com e-mails e modelos v1.0, agora estão ativadas para ativos de e-mail v2.0.

## [Site de desenvolvedores de marketing](http://developers.marketo.com/) {#marketo-developers-site}

Novo e melhorado!

## [Configurações de privacidade](/help/marketo/product-docs/administration/settings/understanding-privacy-settings.md) {#privacy-settings}

Os profissionais de marketing podem usar configurações de privacidade para decidir se devem ou não rastrear visitantes usando os recursos Munchkin e Web Personalization. O nível de rastreamento é controlado usando a configuração Não rastrear do navegador, um cookie de opção de não participação ou um IP não específico. Esses métodos podem afetar o valor e a funcionalidade do Marketo em áreas específicas, mas se o comerciante não alterar nada, a funcionalidade do Marketo permanecerá a mesma.

Este recurso será lançado aos clientes gradualmente ao longo de um período de seis semanas. Se você precisar disso imediatamente, entre em contato com o suporte da Marketo.
