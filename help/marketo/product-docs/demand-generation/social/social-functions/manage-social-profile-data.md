---
unique-page-id: 2950578
description: Gerenciar dados de perfil social - Documentos do Marketo - Documentação do produto
title: Gerenciar dados de perfil social
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 8%

---

# Gerenciar dados de perfil social {#manage-social-profile-data}

Quando alguém interage com uma Marketo [aplicativo social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)ou autoriza sua rede social a preencher previamente um formulário Marketo com [preenchimento do formulário social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), o Marketo captura todos os dados disponíveis do perfil social. Você pode exibir essas informações na [Página Detalhes da pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)ou adicione-a como uma coluna em uma [exibição personalizada de uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

O preenchimento de formulários sociais e os aplicativos sociais capturam conjuntos de campos ligeiramente diferentes; consulte a seção para cada um abaixo.

>[!AVAILABILITY]
>
>Nem todos os clientes compraram essa funcionalidade. Confira os detalhes com seu representante de vendas.

## Capturado via aplicativo social {#captured-via-social-app}

Dependendo das configurações de privacidade da rede e do usuário, um ou mais desses campos são recuperados:

>[!NOTE]
>
>As informações adicionais das redes sociais aparecem na página Detalhes da pessoa cerca de cinco minutos depois que a pessoa autoriza.

## No Twitter: {#from-twitter}

* Nome (analisado a partir do Nome de exibição)
* Sobrenome (analisado a partir do Nome de exibição)
* URL de foto do perfil
* URL da página de perfil
* Alcance social (número de seguidores)

>[!NOTE]
>
>Os aplicativos sociais não buscam o endereço de email da pessoa.

## No Facebook: {#from-facebook}

* Nome
* Sobrenome
* URL do perfil
* URL de foto do perfil
* Sexo
* Alcance social (número de amigos)

### Capturado por meio do preenchimento do formulário social {#captured-via-social-form-fill}

Dependendo das configurações de privacidade da rede e do usuário, um ou mais desses campos são recuperados:

>[!CAUTION]
>
>Os dados capturados pelo preenchimento do formulário social substituem os campos correspondentes, a menos que você [bloquear atualizações para esses campos no nível do formulário](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## No Twitter: {#from-twitter-1}

* Nome (analisado a partir do Nome de exibição)
* Sobrenome (analisado a partir do Nome de exibição)
* E-mail

## De Facebook: {#from-facebook-1}

* Nome
* Sobrenome
* E-mail
* Data de nascimento
* Cargo
* Empresa

>[!NOTE]
>
>O preenchimento do formulário social captura o endereço de email _only_ se a pessoa inseri-la no formulário. Se você precisar do endereço de email, [tornar um campo obrigatório no formulário](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Para capturar essas informações de formulários, ative [preenchimento do formulário social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
