---
unique-page-id: 45416698
description: Notas de versão - 20 de julho - Documentação do Marketo - Documentação do produto
title: Notas de versão - julho de 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# Notas de versão: julho de 20 {#release-notes-july}

Os seguintes recursos estão incluídos na versão de 20 de julho. Verifique a edição do Marketo quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Observe que, dependendo do seu pacote atual, os itens com uma estrela ( ![(estrela)](assets/yellow-star.png)) podem exigir a compra de um complemento de valor. Entre em contato com seu representante da Marketo Engage para obter mais informações.

**_Versões Trimestrais_** Os seguintes recursos serão lançados em **31 de julho de 2020**.

## Administração {#administration}

* **[Exportação de &quot;Usado por&quot; no Gerenciamento de Campos](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: os administradores agora podem exportar todos os links de ativos de &quot;Usado por&quot; de um campo selecionado para um arquivo CSV. Esse aprimoramento pode ajudar administradores e não administradores a limpar campos não utilizados. Além disso, os ativos agora podem ser abertos em uma nova guia ou janela do navegador.

## Marketing baseado em contas {#account-based-marketing}

![(estrela)](assets/yellow-star.png)

* **Interface atualizada para Perfil de Conta**: simplifique a criação da sua lista de contas de destino no Perfil de Conta com etapas simplificadas, tudo em uma única tela.

<br> 

**_Liberando Durante o Trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

* **Serviço Forms**: estamos introduzindo uma validação mais forte de sintaxe de campo de formulário e a capacidade de bloquear padrões de bot comuns com novos Domínios Protegidos para recursos de Páginas de Aterrissagem. O bloqueio de padrões de bot pode reduzir os envios de spam e melhorar a qualidade do banco de dados.

>[!NOTE]
>
>A implantação completa da validação aprimorada da sintaxe do campo de formulário foi adiada até depois da versão de janeiro de 2021.

* **Limite de tamanho do URI da API de ativo aumentado**: o limite de tamanho do identificador de recurso uniforme (URI) está sendo aumentado de 8 KB para 65 KB antes da remoção do parâmetro &quot;_method&quot;. Ao executar sequências de consulta longas, esse aumento do limite de tamanho permitirá que os dados sejam transmitidos mais facilmente. A remoção do parâmetro &quot;_method&quot; faz parte de uma atualização de segurança futura.

## [!DNL Sales Insight] {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Habilitado para Clientes com  [!DNL Salesforce] Integração de CRM](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)** não nativa: os clientes da Marketo Engage com [!DNL Salesforce] integrações de CRM não nativa agora podem usar o [!DNL Sales Insight] para ajudar suas equipes de vendas a entender, priorizar e interagir com os clientes potenciais e oportunidades mais engajados para permitir vendas inteligentes e ofertas mais rápidas.

## [!DNL Sales Connect] {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **[Consentimento aprimorado de duas partes para chamadas de vendas:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** agora os administradores têm maior controle sobre as configurações de gravação de chamadas. [Habilite as gravações de chamadas](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) com a certeza de que você está em conformidade com a lei de consentimento dos dois participantes. Automatize a notificação da chamada que está sendo gravada e ative os clipes de áudio que serão reproduzidos antes da chamada.

<br> 

## Anúncios e desaprovações {#announcements-deprecations}

* **Remoção do parâmetro &quot;_method&quot; da API de ativos**: a partir de setembro de 2020, os pontos de extremidade da API de ativos não aceitarão mais &quot;_method&quot; para transmitir os Parâmetros de consulta em um corpo POST para ignorar as limitações de comprimento de URI. Para acomodar solicitações que exigem esse parâmetro, os limites de URI para APIs de ativos serão aumentados de 8 KB para 65 KB.
* **[[!DNL Munchkin] Associar cliente potencial](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: nesta versão do Munchkin JavaScript Client, versão 159, iniciaremos a desativação do método [!DNL Munchkin] Associar cliente potencial. Se chamado, você receberá um aviso indicando que o método será removido em uma versão futura. Depois de removido, o método não estará mais funcional e as tentativas de usá-lo falharão. Os clientes do Marketo Engage que utilizaram esse método recentemente serão notificados individualmente sobre seu uso.
* **Suporte para o Internet Explorer**: conforme anunciado anteriormente, o suporte do Marketo Engage para o Internet Explorer 11 termina em **31 de julho de 2020**. Continuaremos a oferecer suporte a [!DNL Google Chrome], [!DNL Mozilla Firefox],[!DNL &#x200B; Apple Safari] e [!DNL Microsoft Edge].
* **Experiência Padrão do Sky**: a opção para administradores ou usuários definirem [!DNL Marketo Sky] como a experiência padrão será removida nesta versão como preparação para uma atualização da experiência do usuário principal. Mais detalhes sobre a atualização da experiência principal, programada para o final deste ano, estarão disponíveis em julho. Os usuários que definiram [!DNL Marketo Sky] como sua experiência padrão, ou que receberam acesso a [!DNL Marketo Sky], podem continuar a acessar [!DNL Marketo Sky] de um bloco da home page do My Marketo.
* **Suporte a [!DNL Microsoft Edge] EdgeHTML (não Chromium)**: a Marketo Engage não oferecerá mais suporte a versões EdgeHTML do Microsoft Edge no final de 2020. A partir de 1º de janeiro de 2021, ofereceremos suporte somente à versão mais recente do Chromium do Microsoft Edge.
