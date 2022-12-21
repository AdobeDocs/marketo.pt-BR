---
unique-page-id: 2359646
description: Configurar a criação de perfis progressivos do formulário - Documentos do Marketo - Documentação do produto
title: Configurar a criação de perfis progressivos do formulário
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 1%

---

# Configurar a criação de perfis progressivos do formulário {#configure-form-progressive-profiling}

As formas curtas são boas! Quando alguém volta a um formulário, é possível apresentar novos campos e preencher progressivamente o perfil do visitante. Veja como.

>[!NOTE]
>
>Para que esse recurso funcione corretamente, verifique se o Preenchimento prévio do formulário está ativado para campos visíveis e [desativado](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) para campos ocultos.

1. Ir para **Atividades de marketing**.

   ![](assets/ma-1.png)

1. Selecione o formulário e clique em **Editar formulário**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Em **Configurações do formulário**, clique em **Configurações**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Definir **Criação de perfis progressiva** para **Ativado**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Ok, agora vamos configurá-lo. Ir para **Detalhes do campo**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Arraste e solte todos os campos que fazem parte do conjunto de perfis progressivos.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Quando terminar de mover todos os campos, ele deverá ter esta aparência:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Os campos fora do **Criação de perfis progressiva** sempre serão mostradas no formulário, mesmo que estejam preenchidas.

1. Selecione o **Criação de perfis progressiva** caixa.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Tenha cuidado ao usar campos obrigatórios na criação de perfis progressivos. Esses campos ainda podem ser deixados em branco se o visitante digitar um novo endereço de email (o que criaria uma nova pessoa) depois de enviar dados anteriormente para os outros campos, como seriam suprimidos no formulário mais recente.

1. Agora escolha quantos campos em branco você deseja que as pessoas vejam da **Criação de perfis progressiva** em qualquer momento.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Se você escolher **Número** **de** **Em branco** **Campos** como 1, o visitante verá o seguinte na primeira vez que visualizar este formulário:
   >
   >* First Name (empty)
   >* Sobrenome (vazio)
   >* Endereço de email (vazio)
   >* Número de telefone (vazio)

   >
   >Supondo que eles preencham cada campo, na segunda vez que visitarem, eles verão:
   >
   >* Nome (pré-preenchido)
   >* Sobrenome (pré-preenchido)
   >* Endereço de email (pré-preenchido)
   >* Número de telefone celular (vazio)

   >
   >Supondo que eles preencham o Número do telefone celular, na terceira vez que visitarem o site, eles verão:
   >
   >* Nome (pré-preenchido)
   >* Sobrenome (pré-preenchido)
   >* Endereço de email (pré-preenchido)
   >* País (vazio)


1. Clique em **Concluir**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Clique em **Aprovar e fechar**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Excelente! O trabalho que você acabou de fazer vai pagar.

Experimente este recurso e certifique-se de testar. É avançado, mas você pode tornar seus formulários muito dinâmicos dessa forma.
