---
description: Conectar o bate-papo dinâmico ao Marketo - Documentos do Marketo - Documentação do produto
title: Conectar o bate-papo dinâmico ao Marketo
exl-id: bad6c2dc-d4e7-4f98-bf6d-743043f96e4e
source-git-commit: 9b49c9f0ee03ab72672f46618fb24eed174bf835
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Conectar o bate-papo dinâmico ao Marketo {#connect-dynamic-chat-to-marketo}

Depois de concluir o [configuração inicial](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md), é hora de executar a sincronização única conectando o Dynamic Chat à sua assinatura do Marketo.

1. Em Minha Marketo, clique no botão **Bate-papo dinâmico** mosaico.

   ![](assets/connect-dynamic-chat-to-marketo-1.png)

   >[!NOTE]
   >
   >Caso não veja o bloco, entre em contato com o administrador do Marketo.

1. Se você acessou anteriormente um aplicativo com uma Adobe ID, você será direcionado diretamente para o Bate-papo dinâmico. Caso contrário, [configurar sua Adobe ID](https://helpx.adobe.com/manage-account/using/create-update-adobe-id.html).

1. Para conectar a instância do Marketo, selecione **Integrações**.

   ![](assets/connect-dynamic-chat-to-marketo-2.png)

1. No cartão Marketo , clique em **Iniciar Sincronização**.

   ![](assets/connect-dynamic-chat-to-marketo-3.png)

1. Selecione até 50 campos padrão ou personalizados da instância do Marketo para sincronizar com o Bate-papo dinâmico para usar na definição de metas do público-alvo, mapeamento de dados e personalização. Clique em **Próximo** quando concluído.

   ![](assets/connect-dynamic-chat-to-marketo-4.png)

   >[!CAUTION]
   >
   >No momento, seleções de atributo **cannot** ser alterado após a sincronização inicial. Quando a sincronização estiver concluída, você só poderá voltar e adicionar mais (se tiver escolhido menos de 50).

1. Revise suas seleções (lembrete: não é possível remover atributos pós-sincronização, portanto, clique em **Editar seleções** se precisar alterar alguma nesta etapa). Clique em **Confirmar** quando concluído para iniciar a sincronização.

   ![](assets/connect-dynamic-chat-to-marketo-5.png)

>[!NOTE]
>
>Pode levar de 2 a 24 horas para a sincronização ser concluída, dependendo do tamanho do banco de dados.

## Vincule sua organização do Adobe e do Marketo {#link-your-adobe-org-and-marketo}

Em seguida, é hora de vincular o Adobe e o Marketo.

1. Faça logon em [experience.adobe.com](https://experience.adobe.com).

1. Clique na tela em qualquer lugar no Experience Cloud e pressione ctrl+i. No **Orgs Atribuídas** , realce e copie a ID da organização (_minus_ o &quot;@AdobeOrg&quot;). Press **Fechar** quando concluído.

   ![](assets/connect-dynamic-chat-to-marketo-6.png)

1. No Marketo, acesse **Administrador** e selecione **Mapeamento da organização do Adobe**.

   ![](assets/connect-dynamic-chat-to-marketo-7.png)

1. Clique em **Editar**.

   ![](assets/connect-dynamic-chat-to-marketo-8.png)

1. Cole a ID da organização copiada na Etapa 2 e clique em **OK**.

   ![](assets/connect-dynamic-chat-to-marketo-9.png)

>[!MORELIKETHIS]
>
>[Configuração inicial](/help/marketo/product-docs/demand-generation/dynamic-chat/initial-setup.md)
