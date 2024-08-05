---
unique-page-id: 2950578
description: Gerenciar dados do perfil social - Documentação do Marketo - Documentação do produto
title: Gerenciar dados do perfil social
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 5%

---

# Gerenciar dados do perfil social {#manage-social-profile-data}

Quando alguém interage com um [aplicativo social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) do Marketo ou autoriza sua rede social a preencher previamente um formulário do Marketo com o [preenchimento de formulário social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), o Marketo captura todos os dados disponíveis em seu perfil social. Você pode exibir essas informações na [página Detalhes da Pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) ou adicioná-las como uma coluna em uma [exibição personalizada de uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

>[!IMPORTANT]
>
>Em 31 de julho de 2024, iniciamos o processo de desativação desse recurso. Você não poderá criar novos ativos. Os ativos existentes continuarão a funcionar até 31 de janeiro de 2025. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

O preenchimento de formulário social e os aplicativos sociais capturam conjuntos de campos ligeiramente diferentes; consulte a seção para cada um abaixo.

>[!AVAILABILITY]
>
>Nem todos os usuários do Marketo Engage compraram essa funcionalidade. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter mais detalhes.

## Capturado pelo aplicativo social {#captured-via-social-app}

Dependendo das configurações de privacidade da rede e do usuário, um ou mais destes campos serão recuperados:

>[!NOTE]
>
>As informações adicionais das redes sociais são exibidas na página Detalhes da pessoa cerca de cinco minutos após a pessoa autorizar.

## Do Twitter: {#from-twitter}

* Nome (analisado a partir do Nome de exibição)
* Sobrenome (analisado a partir do Nome de exibição)
* URL da foto do perfil
* URL da página de perfil
* Alcance social (número de seguidores)

>[!NOTE]
>
>Aplicativos sociais não buscam o endereço de email da pessoa.

## No Facebook: {#from-facebook}

* Nome
* Sobrenome
* URL do perfil
* URL da foto do perfil
* Sexo
* Alcance social (número de amigos)

### Registrado via Preenchimento de formulário social {#captured-via-social-form-fill}

Dependendo das configurações de privacidade da rede e do usuário, um ou mais destes campos serão recuperados:

>[!CAUTION]
>
>Os dados capturados pelo preenchimento de formulário social substituem campos correspondentes, a menos que você [bloqueie atualizações nesses campos no nível de formulário](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Do Twitter: {#from-twitter-1}

* Nome (analisado a partir do Nome de exibição)
* Sobrenome (analisado a partir do Nome de exibição)
* Email

## No Facebook: {#from-facebook-1}

* Nome
* Sobrenome
* Email
* Data de nascimento
* Nome do cargo
* Empresa

>[!NOTE]
>
>O preenchimento de formulário social captura o endereço de email _somente_ se a pessoa o inserir no formulário. Se precisar do endereço de email, você deve [torná-lo um campo obrigatório em seu formulário](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Para capturar essas informações de formulários, habilite o [preenchimento de formulário social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
