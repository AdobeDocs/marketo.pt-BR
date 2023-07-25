---
unique-page-id: 2360219
description: Configurar uma assinatura DKIM personalizada - Documentação do Marketo - Documentação do produto
title: Configurar uma assinatura DKIM personalizada
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# Configurar uma assinatura DKIM personalizada {#set-up-a-custom-dkim-signature}

Para garantir um delivery de alto nível, assinamos automaticamente todos os emails de saída com uma assinatura DKIM compartilhada do Marketo.

>[!NOTE]
>
>Você pode precisar da ajuda de sua equipe de TI para concluir algumas etapas deste artigo.

Você pode personalizar a assinatura DKIM para refletir os domínios de sua escolha. Veja como.

1. Vá para a **Admin** seção.

   ![](assets/adminhand.png)

   >[!NOTE]
   >
   >Se você configurar uma assinatura DKIM personalizada da maneira antiga, ela continuará a funcionar e deverá aparecer aqui.

1. Clique em **E-mail**, depois o **DKIM** e, finalmente, **Adicionar domínio**.

   ![](assets/image2014-9-18-15-3a39-3a30.png)

1. Insira o domínio que você usará nos emails do Marketo como o Endereço do remetente e clique em **Adicionar**.

   >[!TIP]
   >
   >Se você usar um domínio diferente no seu Endereço do remetente, usaremos a assinatura DKIM compartilhada do Marketo.

   ![](assets/image2014-9-18-15-3a40-3a28.png)

1. Envie o **Registro de host** e **Valor TXT** para a sua TI. Peça a eles que criem o registro para você e verifique se ele se propaga para todos os servidores de nomes associados ao domínio do. A verificação DKIM do Marketo exige que a chave DKIM seja propagada para todos os servidores de nomes associados ao domínio que está sendo assinado pelo DKIM.

   ![](assets/image2014-9-18-15-3a40-3a44.png)

1. Depois de confirmar que criou o registro, volte para a Marketo, selecione seu domínio e clique em **Verificar DNS**.

   ![](assets/check.png)

   >[!NOTE]
   >
   >Se a confirmação falhar e o departamento de TI tiver criado o registro corretamente, talvez seja uma questão de propagação de DNS. Tente novamente mais tarde.

   >[!CAUTION]
   >
   >Modificar/remover o registro DNS correspondente resultará em uma capacidade de entrega danificada. Exclua a entrada no Marketo antes de fazer alterações no DNS.

   Isso ajudará com sua capacidade de entrega de email. Você deve obter a validação de que o registro está lá e correto.
