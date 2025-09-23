---
unique-page-id: 2360297
description: Restringir logons do Marketo com base em IP - Documentação do Marketo - Documentação do produto
title: Restringir logons do Marketo com base no IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 7%

---

# Restringir logons do Marketo com base no IP {#restrict-marketo-logins-based-on-ip}

Você pode restringir ou permitir que os usuários acessem o Marketo com base em seus endereços IP. Veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!IMPORTANT]
>
>As informações neste artigo são para usuários que fazem logon diretamente em login.marketo.com e não se aplicam a usuários que se autenticam com o Adobe ID. Não é possível impor restrições de IP em logons de logon único (SSO) neste momento.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Clique em **[!UICONTROL Configurações de logon]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Clique em **[!UICONTROL Editar restrições de IP]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Escolha se deseja **Permitir** ou **Bloquear** endereços específicos, insira o(s) endereço(s) e clique em **[!UICONTROL Salvar]**.

   >[!NOTE]
   >
   >**Definição**
   >
   >* **[!UICONTROL Endereços IP permitidos]**: a adição de endereços IP permitidos é uma inclusão. Ele incluirá todos os endereços IP especificados e excluirá todo o resto.
   >* **[!UICONTROL Bloquear endereços IP]**: impede que IPs específicos acessem o Marketo.
   >* **[!UICONTROL Desabilitar Restrições de IP]**: marcar essa opção impedirá que qualquer/todas as regras de restrição funcionem. Use isso para fins de teste.

   >[!NOTE]
   >
   >Você pode adicionar várias restrições, mas elas só podem ser TODAS permitidas ou TODAS bloqueadas. Não é possível misturar e combinar permitidos e bloqueados.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Feito bem, seus dados de marketing agora estão mais seguros do que nunca!
