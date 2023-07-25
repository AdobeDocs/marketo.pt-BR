---
unique-page-id: 2360297
description: Restringir logons do Marketo com base em IP - Documentação do Marketo - Documentação do produto
title: Restringir logons do Marketo com base no IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 1%

---

# Restringir logons do Marketo com base no IP {#restrict-marketo-logins-based-on-ip}

Você pode restringir ou permitir que os usuários acessem o Marketo com base em seus endereços IP. Veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>As informações neste artigo se aplicam apenas aos logons diretos em login.marketo.com. Não é possível impor restrições de IP em logons de logon único (SSO) no momento.

1. Vá para a **[!UICONTROL Admin]** área.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Clique em **[!UICONTROL Configurações de logon]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Clique em **[!UICONTROL Editar restrições de IP]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Escolha se deseja **Permitir** ou **Bloquear** endereços específicos, insira os endereços e clique em **[!UICONTROL Salvar]**.

   >[!NOTE]
   >
   >**Definição**
   >
   >* **[!UICONTROL Endereços IP permitidos]**: a adição de endereços IP permitidos é inclusiva. Ele incluirá todos os endereços IP especificados e excluirá todo o resto.
   >* **[!UICONTROL Bloquear endereços IP]**: impede que IPs específicos acessem o Marketo.
   >* **[!UICONTROL Desativar restrições de IP]**: marcar essa opção impedirá que qualquer/todas as regras de restrição funcionem. Use isso para fins de teste.

   >[!NOTE]
   >
   >Você pode adicionar várias restrições, mas elas só podem ser TODAS permitidas ou TODAS bloqueadas. Não é possível misturar e combinar permitidos e bloqueados.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Feito bem, seus dados de marketing agora estão mais seguros do que nunca!
