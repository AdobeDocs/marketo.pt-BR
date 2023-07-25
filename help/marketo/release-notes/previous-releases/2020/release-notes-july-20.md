---
unique-page-id: 45416698
description: Notas de versão - 20 de julho - Documentação do Marketo - Documentação do produto
title: Notas de versão - julho de 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Notas de versão: julho de 20 {#release-notes-july}

Os seguintes recursos estão incluídos na versão de 20 de julho. Verifique a edição do Marketo quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Observe que, dependendo do pacote atual, os itens têm uma estrela ( ![(estrela)](assets/yellow-star.png)) pode exigir a compra de um complemento de valor. Entre em contato com o representante da Marketo Engage para obter mais informações.

**_Versões trimestrais_** Os seguintes recursos serão lançados em **31 de julho de 2020**.

## Administração {#administration}

* **[Exportação &quot;Usado por&quot; no Gerenciamento de campo](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: agora os administradores podem exportar todos os links de ativos &quot;Usados por&quot; de um campo selecionado para um arquivo CSV. Esse aprimoramento pode ajudar administradores e não administradores a limpar campos não utilizados. Além disso, os ativos agora podem ser abertos em uma nova guia ou janela do navegador.

## Marketing baseado em contas {#account-based-marketing}

![(estrela)](assets/yellow-star.png)

* **Atualização da interface do usuário para criação de perfil da conta**: simplifique a criação da lista de contas de destino na Criação de perfil da conta com etapas simplificadas, tudo em uma única tela.

<br> 

**_Lançamento durante todo o trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

* **Serviço Forms**: estamos introduzindo uma validação mais robusta de sintaxe de campo de formulário e a capacidade de bloquear padrões de bot comuns com novos Domínios protegidos para recursos de Páginas iniciais. O bloqueio de padrões de bot pode reduzir os envios de spam e melhorar a qualidade do banco de dados.

>[!NOTE]
>
>A implantação completa da validação aprimorada da sintaxe do campo de formulário foi adiada até depois da versão de janeiro de 2021.

* **Aumento do limite de tamanho do URI da API de ativos**: o limite de tamanho do identificador de recurso uniforme (URI) está sendo aumentado de 8 KB para 65 KB antes da remoção do parâmetro &quot;_method&quot;. Ao executar sequências de consulta longas, esse aumento do limite de tamanho permitirá que os dados sejam transmitidos mais facilmente. A remoção do parâmetro &quot;_method&quot; faz parte de uma atualização de segurança futura.

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **[Sales Insight ativado para clientes com integração do Salesforce CRM não nativa](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**: os clientes do Marketo Engage com integrações não nativas do Salesforce CRM agora podem usar o Sales Insight para ajudar suas equipes de vendas a entender, priorizar e interagir com os clientes potenciais e oportunidades mais engajados, permitindo vendas inteligentes e ofertas mais rápidas.

## SalesConnect {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **[Consentimento avançado de duas partes para chamadas de vendas:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Os administradores agora têm maior controle sobre as configurações de gravação de chamada. [Habilitar gravações de chamadas](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) com a certeza de que você está em conformidade com a lei de consentimento de duas partes. Automatize a notificação da chamada que está sendo gravada e ative os clipes de áudio que serão reproduzidos antes da chamada.

<br> 

## Anúncios e desaprovações {#announcements-deprecations}

* **Remoção do parâmetro &quot;_method&quot; da API de ativo**: a partir de setembro de 2020, os endpoints da API de ativos não aceitarão mais &quot;_method&quot; para transmitir os Parâmetros de consulta em um corpo de POST para ignorar as limitações de comprimento de URI. Para acomodar solicitações que exigem esse parâmetro, os limites de URI para APIs de ativos serão aumentados de 8 KB para 65 KB.
* **[Líder associado do Munchkin](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: com esta versão do cliente JavaScript Munchkin, versão 159, iniciaremos a desativação do método de lead associado Munchkin. Se chamado, você receberá um aviso indicando que o método será removido em uma versão futura. Depois de removido, o método não estará mais funcional e as tentativas de usá-lo falharão. Os clientes do Marketo Engage que utilizaram esse método recentemente serão notificados individualmente sobre seu uso.
* **Suporte para Internet Explorer**: Conforme anunciado anteriormente, o suporte ao Marketo Engage para o Internet Explorer 11 termina em **31 de julho de 2020**. Continuaremos a oferecer suporte ao Google Chrome, Mozilla Firefox, Apple Safari e Microsoft Edge.
* **Experiência Padrão do Céu**: a opção para administradores ou usuários definirem o Marketo Sky como experiência padrão será removida nesta versão como preparação para uma atualização da experiência do usuário principal. Mais detalhes sobre a atualização da experiência principal, programada para o final deste ano, estarão disponíveis em julho. Os usuários que definiram o Marketo Sky como sua experiência padrão ou que receberam acesso ao Marketo Sky, podem continuar a acessar o Marketo Sky de um bloco na página inicial do My Marketo.
* **Suporte EdgeHTML (não Chromium) do Microsoft Edge**: o Marketo Engage não será mais compatível com as versões EdgeHTML do Microsoft Edge no final de 2020. A partir de 1º de janeiro de 2021, ofereceremos suporte somente à versão mais recente do Chromium do Microsoft Edge.
