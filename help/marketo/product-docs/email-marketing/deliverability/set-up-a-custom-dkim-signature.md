---
unique-page-id: 2360219
description: Configurar uma assinatura DKIM personalizada - Documentos do Marketing - Documentação do produto
title: Configurar uma assinatura DKIM personalizada
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Configurar uma assinatura DKIM personalizada {#set-up-a-custom-dkim-signature}

Para garantir o melhor fornecimento, assinamos automaticamente todos os emails de saída com uma assinatura DKIM do Marketing Cloud compartilhada.

>[!NOTE]
>
>Você pode precisar da ajuda de sua equipe de TI para concluir algumas das etapas deste artigo.

Você pode personalizar a assinatura DKIM para refletir os domínios de sua escolha. Veja como.

1. Vá para a seção **Admin**.

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >
   >Se você configurar uma assinatura DKIM personalizada da maneira antiga, ela continuará funcionando e deverá aparecer aqui.

1. Clique em **Email**, na guia **DKIM** e, por fim, **Adicionar domínio**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. Digite o domínio que você usará nos e-mails do Marketo como Endereço de origem e clique em **Adicionar**.

   >[!TIP]
   >
   >
   >Se você usar um domínio diferente em seu Endereço de origem, usaremos a assinatura DKIM compartilhada do Marketo.

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. Envie **Registro do host** e **Valor TXT** para a sua TI. Solicite que eles criem o registro para você e verifique se ele se propaga para todos os servidores de nomes associados ao domínio from. A verificação DKIM do Marketo requer que a chave DKIM seja propagada para todos os servidores de nomes associados ao domínio que está sendo assinado pelo DKIM.

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. Depois que eles confirmarem que criaram o registro, retorne ao Marketo, selecione seu domínio e clique em **Verificar DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >**Lembrete**
   >
   >Se a confirmação falhar e sua TI tiver criado o registro corretamente, isso pode ser uma questão de propagação DNS. Tente novamente mais tarde.

   >[!CAUTION]
   >
   >
   >Modificar/remover o registro DNS correspondente resultará em danos na entrega. Certifique-se de excluir a entrada no Marketo antes de fazer alterações de DNS.

   Isso ajudará com a entrega por email. Você deve obter a validação de que o registro está lá e correto.

