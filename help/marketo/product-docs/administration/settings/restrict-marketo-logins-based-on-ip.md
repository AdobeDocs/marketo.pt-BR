---
unique-page-id: 2360297
description: Restringir logons do Marketo com base em IP - Documentos do Marketo - Documentação do produto
title: Restringir logons do Marketo com base em IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 1%

---

# Restringir logons do Marketo com base em IP {#restrict-marketo-logins-based-on-ip}

Você pode restringir ou permitir que os usuários acessem o Marketo com base em seus endereços IP. Veja como.

>[!NOTE]
>
>**Permissões de administrador necessárias**

>[!NOTE]
>
>As informações neste artigo se aplicam apenas aos logons diretos em login.marketo.com. Não é possível impor restrições de IP em logons de logon único (SSO) no momento.

1. Em **Administrador**, clique em **Configurações de logon**.

   ![](assets/image2014-9-16-12-3a57-3a56.png)

1. Clique em **Editar restrições de IP**.

   ![](assets/image2014-9-16-12-3a58-3a13.png)

1. Escolha se deseja **Permitir** ou **Bloco** endereços específicos, insira o(s) endereço(s) e clique em **Salvar**.

   >[!NOTE]
   >
   >**Definição**
   >
   >* **Endereços IP permitidos**: Adicionar endereços IP permitidos é inclusivo. Ele incluirá todos os endereços IP especificados e excluirá todos os outros.
   >* **Bloquear endereços IP**: Impede que IPs específicos acessem o Marketo.
   >* **Desativar restrições de IP**: Ao verificar isso, as regras de restrição de todas/todas não funcionarão. Use para fins de teste.


   >[!NOTE]
   >
   >Você pode adicionar várias restrições, mas elas só podem ser TODAS permitidas ou TODAS bloqueadas. Não é possível misturar e combinar permitido e bloqueado.

   ![](assets/image2014-9-16-13-3a9-3a40.png)

   Muito bem feito, seus dados de marketing agora são mais seguros do que nunca!
