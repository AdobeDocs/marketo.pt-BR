---
unique-page-id: 2360219
description: Configurar uma assinatura personalizada do DKIM - Documentação do Marketo - Documentação do produto
title: Configurar uma assinatura personalizada do DKIM
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 4%

---

# Configurar uma assinatura personalizada do DKIM {#set-up-a-custom-dkim-signature}

Para garantir uma capacidade de entrega de alto nível, assinamos automaticamente todos os emails de saída com uma assinatura compartilhada do Marketo DKIM.

>[!NOTE]
>
>Você pode precisar da ajuda de sua equipe de TI para concluir algumas etapas deste artigo.

É possível personalizar a assinatura do DKIM para refletir os domínios de sua escolha. Veja como.

1. Vá para a seção **[!UICONTROL Admin]**.

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >Se você configurar uma assinatura personalizada de DKIM da maneira antiga, ela continuará a funcionar e deverá ser exibida aqui.

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
   >* Recomendamos um Tamanho de chave de 2048.
   >* Se você usar um domínio diferente no seu Endereço de origem, usaremos a assinatura compartilhada do DKIM no Marketo.

   >[!IMPORTANT]
   >
   >Se precisar atualizar o Seletor de DKIM ou o Tamanho da criptografia do DKIM para o domínio, exclua o registro existente e republique o registro recém-gerado com os novos valores.
   >
   >Observe que, ao fazer isso, o DKIM não será assinado para o seu domínio até que o novo registro seja publicado e validado pelo nosso sistema. Planeje a alteração de acordo, pois pode levar de 24 a 48 horas até que o novo registro do DKIM seja totalmente propagado pela Internet.

1. Envie o **[!UICONTROL Registro do Host]** e o **[!UICONTROL Valor TXT]** para sua TI. Peça a eles que criem o registro para você e verifique se ele se propaga para todos os servidores de nomes associados ao domínio do. A verificação do DKIM da Marketo exige que a chave do DKIM seja propagada para todos os servidores de nomes associados ao domínio que está sendo assinado pela DKIM.

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. Depois que ele confirmar que criou o registro, volte para a Marketo, selecione seu domínio e clique em **[!UICONTROL Verificar DNS]**.

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >Se a confirmação falhar e o departamento de TI tiver criado o registro corretamente, talvez seja uma questão de propagação de DNS. Tente novamente mais tarde.

   >[!CAUTION]
   >
   >Modificar/remover o registro DNS correspondente resultará em uma capacidade de entrega danificada. Exclua a entrada no Marketo antes de fazer alterações no DNS.

   Isso ajudará com sua capacidade de entrega de email. Você deve obter a validação de que o registro está lá e correto.
