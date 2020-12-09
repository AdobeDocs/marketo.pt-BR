---
unique-page-id: 2950578
description: Gerenciar dados do Perfil social - Documentos do marketing - Documentação do produto
title: Gerenciar dados do Perfil social
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---


# Gerenciar dados do Perfil social {#manage-social-profile-data}

Quando alguém interage com um aplicativo [](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)social Marketo ou autoriza sua rede social a preencher previamente um formulário Marketo com preenchimento [de formulário](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)social, o Marketo captura todos os dados disponíveis de seu perfil social. Você pode visualização essas informações na página [Detalhes da](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)pessoa ou adicioná-las como uma coluna em uma visualização [personalizada de uma lista](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List)inteligente.

>[!NOTE]
>
>**FYI**
>
>O Marketo agora está padronizando o idioma em todas as subscrições, portanto você pode ver o lead/lead na sua subscrição e a pessoa/pessoas em docs.marketo.com. Estes termos significam a mesma coisa. isso não afeta as instruções do artigo. Há outras mudanças também. [Saiba mais](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

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
>Os dados capturados pelo preenchimento do formulário social substituem os campos correspondentes, a menos que você [bloqueie atualizações para esses campos no nível](../../../../product-docs/administration/field-management/block-updates-to-a-field.md)do formulário.

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
>O preenchimento do formulário social captura o endereço de email *somente* se a pessoa o digitar no formulário. Se você precisar do endereço de email, [torne-o um campo obrigatório no formulário](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Para capturar essas informações dos formulários, ative o preenchimento [do formulário](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)social.

>[!NOTE]
>
>**Mergulho profundo**
>
>Saiba mais sobre como trabalhar com formulários no aprofundamento do [Forms](http://docs.marketo.com/display/docs/forms) .

