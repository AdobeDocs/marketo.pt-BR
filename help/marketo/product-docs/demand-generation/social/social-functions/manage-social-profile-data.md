---
unique-page-id: 2950578
description: Gerenciar dados do Perfil social - Documentos do marketing - Documentação do produto
title: Gerenciar dados do Perfil social
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# Gerenciar dados de Perfil do Social {#manage-social-profile-data}

Quando alguém interage com um aplicativo social Marketo [ou autoriza sua rede social a preencher previamente um formulário Marketo com [formulário social fill](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), o Marketo captura todos os dados disponíveis de seu perfil social. ](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) Você pode visualização essas informações na página [Detalhes da pessoa](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page) ou adicioná-las como uma coluna em uma [visualização personalizada de uma lista inteligente](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List).

O preenchimento de formulários sociais e os aplicativos sociais capturam conjuntos de campos ligeiramente diferentes; consulte a seção para cada um abaixo.

>[!NOTE]
>
>**Disponibilidade**
>
>Nem todos os clientes adquiriram essa funcionalidade. Entre em contato com seu representante de vendas para obter detalhes.

## Capturado pelo aplicativo social {#captured-via-social-app}

Dependendo das configurações de privacidade da rede e do usuário, um ou mais desses campos são recuperados:

>[!NOTE]
>
>As informações adicionais das redes sociais são exibidas na página Detalhes da pessoa cerca de cinco minutos após a autorização da pessoa.

## Do Twitter: {#from-twitter}

* Nome (analisado a partir do Nome de exibição)
* Sobrenome (analisado a partir do Nome de exibição)
* URL da foto do perfil
* URL da página do perfil
* Alcance social (número de seguidores)

>[!NOTE]
>
>Aplicativos sociais não buscam o endereço de email da pessoa.

## Do Facebook: {#from-facebook}

* Nome
* Sobrenome
* URL do perfil
* URL da foto do perfil
* Gênero
* Alcance social (número de amigos)

### Capturado por meio do preenchimento do formulário social {#captured-via-social-form-fill}

Dependendo das configurações de privacidade da rede e do usuário, um ou mais desses campos são recuperados:

>[!CAUTION]
>
>Os dados capturados pelo preenchimento do formulário social substituem os campos correspondentes, a menos que você [bloqueie atualizações desses campos no nível do formulário](../../../../product-docs/administration/field-management/block-updates-to-a-field.md).

## Do Twitter: {#from-twitter-1}

* Nome (analisado a partir do Nome de exibição)
* Sobrenome (analisado a partir do Nome de exibição)
* Email

## Do Facebook: {#from-facebook-1}

* Nome
* Sobrenome
* Email
* Data de nascimento
* Cargo
* Empresa

>[!NOTE]
>
>O preenchimento do formulário social captura o endereço de email *somente* se a pessoa inseri-lo no formulário. Se você precisar do endereço de email, [torne-o um campo obrigatório em seu formulário](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Para capturar essas informações de formulários, ative [preenchimento de formulário social](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).

>[!NOTE]
>
>**Mergulho profundo**
>
>Saiba mais sobre como trabalhar com formulários no aprofundamento [Forms](http://docs.marketo.com/display/docs/forms).

