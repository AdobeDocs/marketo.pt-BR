---
solution: Marketo Engage
product: marketo
title: Testar renderização de email com Litmus
description: Os usuários do Marketo Engage podem integrar sua conta Litmus para testar aparentemente a renderização do conteúdo em vários clientes de email.
level: Beginner, Intermediate
feature: Email Designer
exl-id: ccef36af-362a-4ac0-9030-492e9d7f10b5
source-git-commit: 3a71e0f0da0f6201ccda73a0c8bd5b94864308c0
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Testar renderização de email com Litmus {#test-email-rendering-with-litmus}

Aproveite sua conta do [Litmus](https://www.litmus.com/email-testing) no Marketo Engage para ver instantaneamente como seu email é renderizado em clientes de email populares.

>[!AVAILABILITY]
>
>Esse recurso está disponível para todos os usuários do Marketo Engage que têm uma conta Litmus ativa.

## Usuários do Litmus Enterprise {#litmus-enterprise}

As etapas a seguir são para usuários no [Plano Corporativo Litmus](https://www.litmus.com/pricing/enterprise){target="_blank"}.

1. Na tela _Editar conteúdo do email_, clique no botão **Simular Conteúdo**.

   ![](assets/test-email-rendering-with-litmus-1.png)

1. Selecione o destinatário do teste e clique no botão **Renderizar email**.

   ![](assets/test-email-rendering-with-litmus-2.png){width="800" zoomable="yes"}

1. Caso ainda não o tenha feito, **conecte sua conta Litmus**. Se você já tiver feito isso, pule para a Etapa 6.

   ![](assets/test-email-rendering-with-litmus-3.png){width="800" zoomable="yes"}

1. Insira suas credenciais do Litmus e clique em **Entrar**.

   >[!IMPORTANT]
   >
   >Ao conectar sua conta do Litmus ao Marketo Engage, você concorda que os emails de teste são enviados para o Litmus. Após o envio, esses emails de teste não são mais gerenciados pelo Adobe. Dessa forma, a política de retenção de dados por email Litmus se aplica a esses emails, incluindo dados de personalização que podem ser incluídos neles.

1. Clique em **Conectar** para concluir a integração.

   ![](assets/test-email-rendering-with-litmus-4.png)

1. Clique no botão **Executar teste** para gerar visualizações de email.

1. Veja como o conteúdo é exibido em clientes de email populares de desktop, móveis e baseados na Web. Clique em quantas miniaturas desejar visualizar.

   ![](assets/test-email-rendering-with-litmus-5.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Saiba como [personalizar sua lista padrão de clientes de email](https://help.litmus.com/article/227-change-your-default-email-clients-list).

1. Quando terminar o teste, clique na seta para trás no canto superior esquerdo para retornar à tela _Simular conteúdo_.

   ![](assets/test-email-rendering-with-litmus-6.png)

**ETAPA OPCIONAL**: se você decidir fazer alterações no seu email depois de clicar em **Renderizar email** para exibi-los, clique também no botão **Retestar** no canto superior direito da tela _Visualizações de Email_ do Litmus.

![](assets/test-email-rendering-with-litmus-7.png)

## Usuários principais Litmus {#litmus-core}

As etapas a seguir são para usuários no [Plano Principal Litmus](https://www.litmus.com/pricing/){target="_blank"}.

1. Na sua conta Litmus, recupere o endereço de email de teste clicando no botão **Copiar endereço de teste** na tela _Testar_.

   ![](assets/test-email-rendering-with-litmus-8.png){width="800" zoomable="yes"}

1. No Marketo Engage, navegue até a tela _Editar conteúdo de email_ do email desejado e clique no botão **Simular conteúdo**.

   ![](assets/test-email-rendering-with-litmus-9.png){width="600" zoomable="yes"}

1. Selecione os destinatários do teste e clique no botão **Enviar prova**.

   ![](assets/test-email-rendering-with-litmus-10.png){width="800" zoomable="yes"}

1. Insira o endereço de email Litmus que você copiou na Etapa 1 e clique novamente em **Enviar prova**.

   ![](assets/test-email-rendering-with-litmus-11.png)

1. Revise o email dentro da conta Litmus (na pasta correspondente ao endereço de email copiado do Litmus).

   ![](assets/test-email-rendering-with-litmus-12.png){width="800" zoomable="yes"}
