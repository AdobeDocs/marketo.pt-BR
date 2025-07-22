---
unique-page-id: 2359646
description: Configurar Criação Progressiva De Perfil Do Formulário - Documentação Do Marketo - Documentação Do Produto
title: Configurar o formulário de criação de perfil progressiva
exl-id: 72afe3dc-0688-45ec-ab70-4dc9accf4fc8
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 1%

---

# Configurar o formulário de criação de perfil progressiva {#configure-form-progressive-profiling}

Formas curtas são boas! Quando alguém retorna a um formulário, é possível apresentar novos campos e preencher progressivamente o perfil do visitante. Veja como.

>[!NOTE]
>
>Para que esse recurso funcione corretamente, verifique se o Preenchimento prévio de formulário está habilitado para campos visíveis e [desabilitado](/help/marketo/product-docs/demand-generation/forms/form-fields/disable-pre-fill-for-a-form-field.md) para campos ocultos.

1. Vá para **[!UICONTROL Atividades de marketing]**.

   ![](assets/ma-1.png)

1. Selecione seu formulário e clique em **[!UICONTROL Editar Formulário]**.

   ![](assets/image2014-9-15-12-3a31-3a20.png)

1. Em **[!UICONTROL Configurações de formulário]**, clique em **[!UICONTROL Configurações]**.

   ![](assets/image2014-9-15-12-3a31-3a29.png)

1. Definir **[!UICONTROL Criação de Perfil Progressiva]** para **[!UICONTROL Habilitado]**.

   ![](assets/image2014-9-15-12-3a31-3a47.png)

1. Ok, agora vamos configurá-lo. Vá para **[!UICONTROL Detalhes do campo]**.

   ![](assets/image2014-9-15-12-3a31-3a55.png)

1. Arraste e solte todos os campos que fazem parte do conjunto de perfis progressivos.

   ![](assets/image2014-9-15-12-3a32-3a3.png)

1. Quando terminar de mover todos os campos, deverá ser semelhante a:

   ![](assets/image2014-9-15-12-3a32-3a12.png)

   >[!NOTE]
   >
   >Os campos fora da caixa **[!UICONTROL Criação de perfil progressiva]** sempre serão exibidos no formulário, mesmo se estiverem preenchidos.

1. Selecione a caixa **[!UICONTROL Progressive Profiling]**.

   ![](assets/image2014-9-15-12-3a32-3a19.png)

   >[!CAUTION]
   >
   >Tenha cuidado ao usar campos obrigatórios em [!UICONTROL Criação de Perfil Progressiva]. Esses campos ainda podem ser deixados em branco se o visitante inserir um novo endereço de email (que criaria uma nova pessoa) após enviar dados anteriormente para os outros campos, pois seriam suprimidos no formulário mais recente.

1. Agora escolha quantos campos em branco você deseja que as pessoas vejam na caixa **Criação de perfil progressiva** em um determinado momento.

   ![](assets/image2014-9-15-12-3a32-3a26.png)

   >[!NOTE]
   >
   >Se você escolher **[!UICONTROL Número de campos em branco]** como 1, o visitante verá o seguinte na primeira vez que vir este formulário:
   >
   >* Nome (vazio)
   >* Sobrenome (vazio)
   >* Endereço de email (vazio)
   >* Número de telefone (vazio)
   >
   >Supondo que eles preencham cada campo, na segunda vez que visitarem, verão:
   >
   >* Nome (pré-preenchido)
   >* Sobrenome (pré-preenchido)
   >* Endereço de email (pré-preenchido)
   >* Número de telefone celular (vazio)
   >
   >Supondo que eles preencham o Número de Telefone Celular, a terceira vez que visitarem eles verão:
   >
   >* Nome (pré-preenchido)
   >* Sobrenome (pré-preenchido)
   >* Endereço de email (pré-preenchido)
   >* País (vazio)

1. Clique em **[!UICONTROL Concluir]**.

   ![](assets/image2014-9-15-12-3a33-3a35.png)

1. Clique em **[!UICONTROL Aprovar e Fechar]**.

   ![](assets/image2014-9-15-12-3a33-3a45.png)

Excelente! O trabalho que você acabou de fazer compensará.

Experimente esse recurso e certifique-se de testar. É avançado, mas você pode tornar seus formulários muito dinâmicos dessa maneira.
