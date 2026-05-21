---
unique-page-id: 2360219
description: Saiba como configurar uma assinatura personalizada do DKIM para seu domínio no Marketo. Adicione um domínio no Administrador e trabalhe com TI para publicar o registro DNS.
title: Configurar uma assinatura personalizada do DKIM
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
TQID: https://experienceleague.adobe.com/ln23WoloRVzBoC8CXFsm90LqYV5FDJzbII8UItp3xDc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 39b6fecdc7aa16ab1205582d3bf372a8538a2d35
workflow-type: tm+mt
source-wordcount: 434
ht-degree: 4%

---

# Configurar uma assinatura personalizada do DKIM {#set-up-a-custom-dkim-signature}

Para garantir a capacidade de entrega ideal, o Marketo assina automaticamente todos os emails de saída com uma assinatura compartilhada do DKIM.

>[!NOTE]
>
>Você pode precisar da ajuda de sua equipe de TI para concluir algumas etapas deste artigo.

É possível personalizar a assinatura do DKIM para refletir os domínios de sua escolha.

1. Vá para a seção **[!UICONTROL Admin]**.

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >Se você configurar uma assinatura personalizada do DKIM usando o método herdado, ela continuará a funcionar e deverá ser exibida aqui.

1. Clique em **Email**.

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. Clique na guia **SPF/DKIM** e depois em **Adicionar Domínio**.

   ![](assets/set-up-a-custom-dkim-signature-3.png)

1. Insira o domínio que você usará nos emails do Marketo como o Endereço do remetente. Escolha um Seletor e um Tamanho de chave. Clique em **Adicionar** quando terminar.

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   <table>
   <tr>
   <td width="20%"><b>Seletor</b></td>
   <td>Uma string/identificador exclusivo usado para localizar a parte da chave pública do registro do DKIM. Pode ser uma string arbitrária ou um identificador exclusivo para separar e identificar a finalidade dessa chave/registro do DKIM.</td>
   </tr>
   <tr>
   <td width="20%"><b>Tamanho da chave</b></td>
   <td>O nível de segurança com o qual você deseja que sua assinatura DKIM seja criptografada.</td>
   </tr>
   </tbody>
   </table>

   <p>

   >[!TIP]
   >
   >* Recomenda-se um Tamanho de chave de 2048.
   >* Se você usar um domínio diferente no endereço do remetente, o Marketo usará a assinatura compartilhada do DKIM.

   >[!IMPORTANT]
   >
   >Se precisar atualizar o Seletor de DKIM ou o Tamanho da criptografia do DKIM para o domínio, exclua o registro existente e republique o registro recém-gerado com os novos valores.
   >
   >Ao fazer isso, o DKIM não será assinado para o seu domínio até que o novo registro seja publicado e validado pelo nosso sistema. Planeje a alteração de acordo, pois pode levar de 24 a 48 horas até que o novo registro do DKIM seja totalmente propagado pela Internet.

1. Envie o **[!UICONTROL Registro do Host]** e o **[!UICONTROL Valor TXT]** para sua TI. Peça a eles para criar o registro para você e garantir que ele se propague para todos os servidores de nomes associados ao domínio do. A verificação do DKIM da Marketo exige que a chave do DKIM seja propagada para todos os servidores de nomes associados ao domínio que está sendo assinado pela DKIM.

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. Depois que eles confirmarem que criaram o registro, volte para a Marketo, selecione seu domínio e clique em **[!UICONTROL Verificar DNS]**.

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >Se a confirmação falhar e o departamento de TI tiver criado o registro corretamente, talvez seja uma questão de propagação de DNS. Tente novamente mais tarde.

   >[!CAUTION]
   >
   >Modificar/remover o registro DNS correspondente resultará em uma capacidade de entrega danificada. Exclua a entrada no Marketo antes de fazer alterações de DNS.

   Isso melhorará a capacidade de entrega de emails. Você deve obter a validação de que o registro está lá e correto.
