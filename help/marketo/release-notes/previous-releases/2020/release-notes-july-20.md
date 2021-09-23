---
unique-page-id: 45416698
description: Notas de versão - 20 de julho - Documentos da Marketo - Documentação do produto
title: Notas de versão - julho de 2020
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Notas de versão: Julho de 20 {#release-notes-july}

Os seguintes recursos estão incluídos na versão de julho de 2020. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Observe que, dependendo do seu pacote atual, os itens com uma estrela ( ![(star)](assets/yellow-star.png)) podem exigir a compra de um complemento de valor. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestraisOs seguintes recursos serão lançados em 31_** de julho de 2020 ****.

## Administração {#administration}

* **[Exportar &quot;Usado por&quot; no gerenciamento](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)** de campo: Agora, os administradores podem exportar todos os links de ativos &quot;Usados por&quot; para um campo selecionado em um arquivo CSV. Esse aprimoramento pode ajudar administradores e não administradores na limpeza de campos não utilizados. Além disso, agora os ativos podem ser abertos em uma nova guia ou janela do navegador.

## Marketing baseado em contas {#account-based-marketing}

![(estrela)](assets/yellow-star.png)

* **Interface do usuário atualizada para Criação de perfil** da conta: Simplifique a criação da lista de contas de destino em Criação de perfil da conta com etapas simplificadas, tudo em uma única tela.

<br> 

**_Lançamento em todo o trimestre_**

Os seguintes recursos estão em um ciclo não trimestral e serão lançados nos próximos meses.

* **Serviço** Forms: Estamos introduzindo uma validação mais forte da sintaxe do campo de formulário e a capacidade de bloquear padrões de bot comuns com novos domínios protegidos para recursos de Páginas de aterrissagem. Bloquear padrões de bot pode reduzir envios de formulários de spam e melhorar a qualidade do seu banco de dados.

>[!NOTE]
>
>A implementação completa da validação aprimorada da sintaxe do campo de formulário foi adiada para depois da versão de janeiro de 2021.

* **Aumento do limite** de tamanho do URI da API de ativos: O limite de tamanho do URI (identificador de recurso uniforme) está sendo aumentado de 8 KB para 65 KB antes da remoção do parâmetro &quot;_method&quot;. Ao executar longas sequências de consulta, esse aumento do limite de tamanho permitirá que os dados sejam transmitidos com mais facilidade. A remoção do parâmetro &quot;_method&quot; faz parte de uma atualização de segurança futura.

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **[Insight de vendas ativado para clientes com integração](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)  de CRM não nativa do Salesforce (Beta)**: Os clientes do Marketo Engage com integrações não nativas do Salesforce CRM agora podem usar o Sales Insight para ajudar suas equipes de vendas a entender, priorizar e interagir com os clientes potenciais mais envolvidos e oportunidades para permitir vendas inteligentes e ofertas mais rápidas.

## SalesConnect {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **[Consentimento de duas partes aprimorado para chamadas de vendas:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** os administradores agora têm maior controle sobre as configurações de gravação de chamadas. [Habilite ](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) registros de chamadas com confiança de que você esteja em conformidade com a lei de consentimento de duas partes. Automatize a notificação da chamada que está sendo gravada e ative os clipes de áudio a serem reproduzidos antes da chamada.

<br> 

## Anúncios e desaprovações {#announcements-deprecations}

* **Remoção** do parâmetro &quot;_method&quot; da API de ativos: Após setembro de 2020, os endpoints da API de ativos não aceitarão mais &quot;_method&quot; para transmitir os Parâmetros de consulta em um corpo do POST para ignorar as limitações de comprimento do URI. Para acomodar solicitações que exigiram esse parâmetro, os limites de URI para APIs de ativos serão aumentados de 8 KB para 65 KB.
* **[Líder](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)** da Associação Munchkin: Com esta versão do Munchkin JavaScript Client, versão 159, começaremos a descontinuação do método Munchkin Associate Lead. Se chamado, você receberá um aviso indicando que o método será removido em uma versão futura. Depois de removido, o método não estará mais funcional e as tentativas de usá-lo apresentarão falha. Os clientes do Marketo Engage que utilizaram esse método recentemente serão notificados individualmente sobre seu uso.
* **Suporte para Internet Explorer**: Conforme anunciado anteriormente, o suporte do Marketo Engage para o Internet Explorer 11 termina em 31  **de julho de 2020**. Continuaremos a oferecer suporte ao Google Chrome, Mozilla Firefox, Apple Safari e Microsoft Edge.
* **Experiência** padrão do Sky: A opção para administradores ou usuários definirem o Marketo Sky como a experiência padrão será removida nesta versão em preparação para uma atualização da experiência do usuário principal. Mais detalhes sobre a atualização da experiência principal, programada para o final deste ano, estarão disponíveis em julho. Os usuários que definiram o Marketo Sky como sua experiência padrão ou que receberam acesso ao Marketo Sky podem continuar a acessar o Marketo Sky de um bloco na página inicial Minha Marketo.
* **Suporte** ao EdgeHTML (não Chromium) Microsoft Edge: O Marketo Engage não será mais compatível com as versões EdgeHTML do Microsoft Edge no final de 2020. A partir de 1º de janeiro de 2021, ofereceremos suporte somente à versão mais recente do Chromium do Microsoft Edge.
