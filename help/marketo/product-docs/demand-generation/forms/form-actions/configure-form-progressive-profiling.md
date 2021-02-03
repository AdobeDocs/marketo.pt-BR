---
unique-page-id: 2359646
description: Configurar o perfil progressivo do formulário - Documentos de marketing - Documentação do produto
title: Configurar o perfil progressivo do formulário
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---


# Configurar o perfil progressivo do formulário {#configure-form-progressive-profiling}

As formas curtas são boas! Quando alguém volta a um formulário, é possível apresentar novos campos e preencher progressivamente o perfil do visitante. Veja como.

>[!NOTE]
>
>Para que esse recurso funcione corretamente, verifique se o Preenchimento prévio do formulário está ativado para campos visíveis e [disabled](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) para campos ocultos.

1. Vá para **Atividades de marketing**.

   ![](assets/ma-1.png)

1. Selecione o formulário e clique em **Editar formulário**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Em **Configurações do formulário**, clique em **Configurações**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Defina **Perfil Progressivo** como **Ativado**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Ok, agora vamos configurá-lo. Vá para **Detalhes do campo**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Arraste e solte todos os campos que fazem parte do conjunto de perfis progressivos.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Quando terminar de mover todos os campos, ele deve se parecer com isto:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Os campos fora da caixa **Definição de perfil progressiva** sempre serão exibidos no formulário, mesmo que estejam preenchidos.

1. Selecione a caixa **Definição de perfil progressiva**.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Tenha cuidado ao usar os campos obrigatórios na criação de perfil progressiva. Esses campos ainda podem ser deixados em branco se o visitante digitar um novo endereço de email (o que criaria uma nova pessoa) depois de enviar dados anteriormente para os outros campos, como seriam suprimidos no formulário mais recente.

1. Agora, escolha quantos campos em branco você deseja que as pessoas vejam na caixa **Definição de perfil progressiva** a qualquer momento.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Se você escolher **Number** **de** **Em branco** **Fields** como 1, o visitante verá o seguinte na primeira vez que vir este formulário:
   >
   >* Nome (vazio)
   >* Sobrenome (vazio)
   >* Endereço de email (vazio)
   >* Número de telefone (vazio)

   >
   >Supondo que eles preencham cada campo, na segunda vez que visitam, eles verão:
   >
   >* Nome (pré-preenchido)
   >* Sobrenome (pré-preenchido)
   >* Endereço de email (pré-preenchido)
   >* Número de telefone celular (vazio)

   >
   >Supondo que eles preencham o número de telefone celular, na terceira vez que visitarem eles verão:
   >
   >* Nome (pré-preenchido)
   >* Sobrenome (pré-preenchido)
   >* Endereço de email (pré-preenchido)
   >* País (vazio)


1. Clique em **Concluir**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Clique em **Aprovar e Fechar**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Bom trabalho! O trabalho que você acabou de fazer vai pagar.

Experimente este recurso e certifique-se de testar. É avançado, mas você pode tornar seus formulários muito dinâmicos dessa forma.
