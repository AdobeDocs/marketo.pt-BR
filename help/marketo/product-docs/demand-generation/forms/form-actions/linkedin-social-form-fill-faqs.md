---
unique-page-id: 10098238
description: Perguntas frequentes sobre o preenchimento de formulários no LinkedIn Social - Documentação do Marketo - Documentação do produto
title: Perguntas frequentes sobre o preenchimento de formulários sociais do LinkedIn
hide: true
hidefromtoc: true
exl-id: ce87b918-5b45-418f-9b42-8e8275f2e60a
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# [!DNL LinkedIn] Perguntas frequentes sobre preenchimento de formulários sociais {#linkedin-social-form-fill-faqs}

A política de API revisada de [!DNL LinkedIn] exigiu a remoção do Preenchimento de formulário social [!DNL LinkedIn] de nosso produto.

## O que é importante saber {#important-things-to-know}

* Os botões de Preenchimento de formulário social do [!DNL LinkedIn] não eram mais uma opção para adicionar ao Marketo em 28 de abril de 2016

* Removemos o botão Preenchimento de formulário social [!DNL LinkedIn] de todos os formulários que o habilitaram

## Por que essa funcionalidade foi removida da minha assinatura do Marketo? {#why-was-this-functionality-removed-from-my-marketo-subscription}

O LinkedIn fez algumas mudanças significativas em seu programa para desenvolvedores. Como parte dessas alterações, a Marketo não é mais capaz de oferecer suporte a essa funcionalidade para clientes do.

## O que aconteceu se eu não removi os botões de Preenchimento de formulário social [!DNL LinkedIn] dos meus formulários que tinham o Formulário social ativado? {#what-happened-if-i-didnt-remove-the-linkedin-social-form-fill-buttons-from-my-forms-that-had-social-form-enabled}

Em 28 de abril de 2016, removemos o botão Preenchimento de formulário social do [!DNL LinkedIn] dos formulários que ainda tinham o Formulário social habilitado.

## Estou inserindo essa funcionalidade em formulários desde que nos tornamos clientes do Marketo. Como sei quais formulários estavam usando o Preenchimento de formulário social [!DNL LinkedIn]? {#i-have-been-inserting-this-functionality-on-forms-since-we-became-a-marketo-customer-how-do-i-know-which-forms-were-using-linkedin-social-form-fill}

Antes de fazermos essa alteração, enviamos notificações semanais para sua Caixa de Entrada de notificações com uma lista de formulários que usavam o Preenchimento de formulário social do [!DNL LinkedIn]. Esses alertas tinham o objetivo de ajudá-lo a identificar onde você estava usando essa funcionalidade.

## Os botões de Compartilhamento em Redes Sociais do [!DNL LinkedIn] ainda funcionam? {#do-linkedin-social-sharing-buttons-still-work}

Sim. A alteração afeta apenas a funcionalidade de Preenchimento de formulário social [!DNL LinkedIn].

## O Preenchimento de formulário social [!DNL Facebook] e [!DNL Twitter] ainda funciona? {#do-facebook-and-twitter-social-form-fill-still-work}

Sim. [!DNL Facebook] e [!DNL Twitter] Preenchimento de formulário social não foram alterados.

## Algo aconteceu com os dados que já capturamos através do Preenchimento de formulário social [!DNL LinkedIn]? {#did-anything-happen-to-the-data-we-already-captured-via-linkedin-social-form-fill}

Não, esses dados já estavam armazenados no registro de pessoa no Marketo e não foram afetados por essa alteração.

## Onde posso encontrar mais informações sobre a política de API do LinkedIn? {#where-can-i-find-more-information-about-linkedin-s-api-policy}

Siga este link para saber mais sobre as alterações [!DNL LinkedIn] feitas na política de API: [https://developer.linkedin.com/blog/posts/2015/developer-program-changes](https://developer.linkedin.com/blog/posts/2015/developer-program-changes)

## Como posso contatar [!DNL LinkedIn] com perguntas? {#how-can-i-contact-linkedin-with-questions}

Siga este link para contatar [!DNL LinkedIn] sobre suas Soluções de Marketing: [https://business.linkedin.com/marketing-solutions/contact-us](https://business.linkedin.com/marketing-solutions/contact-us)

## Se o Marketo removeu essa funcionalidade de meus formulários em 28 de abril, meus formulários e as páginas de aterrissagem afetadas foram colocados no modo de rascunho? {#if-marketo-removed-this-functionality-from-my-forms-on-april-were-my-forms-and-the-affected-landing-pages-put-into-draft-mode}

Não, os formulários dos quais removemos essa funcionalidade permaneceram publicados.

## Se [!DNL LinkedIn] foi minha única rede selecionada, isso alterará a aparência do meu formulário? {#if-linkedin-was-my-only-selected-network-will-this-change-the-appearance-of-my-form}

Não, removeremos apenas o botão [!DNL LinkedIn] do seu formulário. Sempre que o Preenchimento de formulário social é aplicado a um formulário, há um contêiner criado acima dele que contém os botões Preenchimento de formulário social. Antes de 28 de abril de 2016, se [!DNL LinkedIn] fosse a única opção, a aparência do contêiner seria semelhante a esta imagem:

![—](assets/one.png)

Depois de 28 de abril de 2016, há um contêiner vazio na parte superior de qualquer formulário que tenha removido o Preenchimento de formulário social [!DNL LinkedIn]:

![—](assets/two.png)

>[!NOTE]
>
>As imagens acima são somente para exemplo. Pode não ser exatamente assim que o contêiner do botão Preenchimento de formulário social é renderizado. Qualquer cor, estilo, etc. da fonte você escolheu influenciar a aparência do seu recipiente.

## Se [!DNL LinkedIn] foi minha única rede selecionada, como posso remover o container vazio acima do meu formulário? {#if-linkedin-was-my-only-selected-network-how-can-i-remove-the-empty-container-above-my-form}

Você pode remover o contêiner vazio editando o formulário, selecionando [!DNL Facebook] ou [!DNL Twitter] como uma opção para Preenchimento de formulário social e desmarcando [!DNL Facebook] ou [!DNL Twitter] como uma opção para Preenchimento de formulário social. Isso redefinirá as opções sociais no contêiner de preenchimento do formulário e as removerá do formulário.
