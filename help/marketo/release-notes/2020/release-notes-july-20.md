---
unique-page-id: 45416698
description: Notas de versão - 20 de julho de 2010 - Documentos do Marketing - Documentação do produto
title: Notas de versão - julho de 2020
translation-type: tm+mt
source-git-commit: b33f5ed707a1377daad51191cc6dd9f093138258
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---


# Notas de versão: Jul. 20 {#release-notes-july}

Os seguintes recursos estão incluídos na versão de 20 de julho. Verifique sua edição de marketing para ver a disponibilidade de recursos.

>[!AVAILABILITY]
>
>Observe que, dependendo do seu pacote atual, os itens com uma estrela ( ![(star)](assets/star-yellow.svg)) podem exigir a compra de um complemento de valor. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestraisOs seguintes recursos serão lançados em 31_** de julho de 2020 ****.

## Administração {#administration}

* **[Exportação &quot;Usada por&quot; no Gerenciamento](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)** de campo: Agora, os administradores podem exportar todos os links de ativos &quot;Usados por&quot; para um campo selecionado em um arquivo CSV. Essa melhoria pode ajudar administradores e não administradores na limpeza de campos não utilizados. Além disso, os ativos agora podem ser abertos em uma nova guia ou janela do navegador.

## Marketing baseado em conta {#account-based-marketing}

![(estrela)](assets/star-yellow.svg)

* **Interface do usuário atualizada para a criação de perfil** da conta: Simplifique a criação da lista da conta do público alvo na criação do perfil da conta com etapas simplificadas, todas em uma única tela.

<br> 

**_Lançamento no Trimestre_**

Os seguintes recursos estão em um ciclo não trimestral e serão lançados nos próximos meses.

* **Serviço** Forms: Estamos introduzindo uma validação mais forte da sintaxe do campo de formulário e a capacidade de bloquear padrões de bot comuns com novos domínios protegidos para recursos Landing page. Bloquear padrões do robô pode reduzir o envio de formulários de spam e melhorar a qualidade do banco de dados.
* **Aumento do limite** de tamanho de URI da API de ativos: O limite de tamanho do URI (identificador de recurso uniforme) está sendo aumentado de 8 KB para 65 KB antes da remoção do parâmetro &quot;_method&quot;. Ao executar sequências de caracteres longas de query, esse aumento do limite de tamanho permitirá que os dados sejam transmitidos mais facilmente. A remoção do parâmetro &quot;_method&quot; faz parte de uma próxima atualização de segurança.

## Insight de vendas {#sales-insight}

![(estrela)](assets/star-yellow.svg)

* **[Insight de vendas ativado para clientes com integração](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)  não nativa do Salesforce CRM (Beta)**: Clientes Marketo Engage com integrações não nativas do Salesforce CRM agora podem usar o Sales Insight para ajudar suas equipes de vendas a entender, priorizar e interagir com os clientes potenciais mais envolvidos e oportunidades para permitir vendas inteligentes e negócios mais rápidos.

## Conexão de vendas {#sales-connect}

![(estrela)](assets/star-yellow.svg)

* **[Consentimento de duas partes aprimorado para chamadas de vendas:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** os administradores agora têm maior controle sobre as configurações de gravação de chamadas. [Ative ](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) gravações de chamadas com confiança de que você esteja em conformidade com a lei de consentimento de duas partes. Automatize a notificação da chamada que está sendo gravada e ative os clipes de áudio a serem reproduzidos antes da chamada.

<br> 

## Anúncios e desaprovações {#announcements-deprecations}

* **Remoção** do parâmetro &quot;_method&quot; da API de ativos: Após setembro de 2020, os pontos finais da API de ativos não aceitarão mais &quot;_method&quot; para passar os Parâmetros de Query em um corpo de POST para ignorar as limitações de comprimento de URI. Para acomodar solicitações que exigem esse parâmetro, os limites de URI para APIs de ativos serão aumentados de 8 KB para 65 KB.
* **[Chumbo](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** associado Munchkin: Com esta versão do Munchkin JavaScript Client, versão 159, começaremos a desaprovação do método Munchkin Associate Lead. Se chamado, você receberá um aviso indicando que o método será removido em uma versão futura. Depois de removido, o método não estará mais funcional e as tentativas de usá-lo falharão. Os clientes do Marketo Engage que utilizaram esse método recentemente serão notificados individualmente de sua utilização.
* **Suporte para o Internet Explorer**: Como anunciado anteriormente, o suporte ao Marketo Engage para o Internet Explorer 11 termina em 31  **de julho de 2020**. Continuaremos a oferecer suporte ao Google Chrome, Mozilla Firefox, Apple Safari e Microsoft Edge.
* **Experiência** padrão do Sky: A opção para administradores ou usuários definirem o Marketo Sky como a experiência padrão será removida nesta versão como preparação para uma atualização da experiência do usuário principal. Mais detalhes sobre a atualização da experiência primária, programada para o final deste ano, estarão disponíveis em julho. Os usuários que definiram o Marketo Sky como sua experiência padrão, ou que receberam acesso ao Marketo Sky, podem continuar acessando o Marketo Sky a partir de um bloco no home page My Marketo.
* **Suporte** a EdgeHTML (não Chroium) do Microsoft Edge: O Marketo Engage não oferecerá mais suporte às versões EdgeHTML do Microsoft Edge no final de 2020. A partir de 1º de janeiro de 2021, ofereceremos suporte apenas à versão mais recente do Microsoft Edge para Chromo.
