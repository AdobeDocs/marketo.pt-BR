---
unique-page-id: 2360297
description: Restringir logons do Marketo com base em IP - Documentação do Marketo - Documentação do produto
title: Restringir logons do Marketo com base no IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: b6680c404075f13b1713ce28299e60a4d26f4a06
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 7%

---

# Restringir logons do Marketo com base no IP {#restrict-marketo-logins-based-on-ip}

Você pode restringir ou permitir que os usuários acessem o Marketo com base em seus endereços IP. Veja como.

>[!NOTE]
>
>**Permissões de administrador são necessárias**

>[!IMPORTANT]
>
>O Adobe Admin Console (AAC) dá suporte a [controle de acesso baseado em IP](https://helpx.adobe.com/br/enterprise/using/ip-based-access.html){target="_blank"}. Para garantir uma transição suave, as restrições de IP da Marketo Engage existentes estarão ativas, incluindo usuários da Adobe ID, até o primeiro trimestre de 2027, nas assinaturas em que esse recurso estiver habilitado.
>
>* Você pode configurar o acesso baseado em IP da AAC a qualquer momento.
>* As restrições da AAC e do Marketo Engage podem ser executadas simultaneamente. Use a mesma lista de permissões de IP para obter compatibilidade.
>
>Após o primeiro trimestre de 2027, as restrições de IP da Marketo Engage serão desativadas. O acesso baseado em IP será gerenciado exclusivamente por meio da AAC e deve ser configurado para aplicar restrições de logon. Uma data final de transição será anunciada posteriormente.

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
