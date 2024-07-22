---
description: Expiração de ativo local - Documentação do Marketo - Documentação do produto
title: Expiração do ativo local
exl-id: 603e3eee-0531-4139-a8f5-279831ad011f
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Expiração do ativo local {#local-asset-expiration}

Defina uma data/hora de expiração para desfazer a publicação de páginas de aterrissagem, desativar campanhas de acionador ou parar campanhas de lote recorrentes.

## Conceder permissão de expiração de ativo de agendamento {#grant-schedule-asset-expiration-permission}

Antes de agendar a expiração de um ativo, a função Marketo deve ter a permissão adequada ativada.

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. Na área [!UICONTROL Administrador], clique em **[!UICONTROL Usuários e funções]**.

   ![](assets/local-asset-expiration-1.png)

1. Clique na guia **[!UICONTROL Funções]**, selecione o usuário ao qual deseja conceder acesso e clique em **[!UICONTROL Editar Função]**.

   ![](assets/local-asset-expiration-2.png)

1. Em [!UICONTROL Acessar atividades de marketing], selecione **[!UICONTROL Agendar expiração de ativo local]** e clique em **[!UICONTROL Salvar]**.

   ![](assets/local-asset-expiration-3.png)

## Definir uma data de expiração {#set-an-expiration-date}

1. Clique com o botão direito do mouse no programa desejado e selecione **[!UICONTROL Definir Expiração de Ativo Local]**.

   ![](assets/local-asset-expiration-4.png)

1. Verifique o(s) ativo(s) para o(s) qual(is) você deseja definir uma data de expiração e clique em **[!UICONTROL Definir expiração]**.

   ![](assets/local-asset-expiration-5.png)

1. Escolha uma data de expiração.

   ![](assets/local-asset-expiration-6.png)

1. Defina um horário. Você deve agendar um horário para pelo menos 15 minutos no futuro (não se esqueça de inserir AM/PM). Clique em **[!UICONTROL Confirmar]** quando terminar.

   ![](assets/local-asset-expiration-7.png)

>[!NOTE]
>
>* Para editar uma data de expiração existente, basta verificar o(s) ativo(s) e clicar em **[!UICONTROL Definir expiração]**.
>* Depois que um ativo expirar, ele não será mais exibido na grade Expiration. A grade exibirá somente landing pages publicadas, campanhas de acionador ativas e campanhas de lote recorrentes.
>* As expirações programadas serão removidas se o ativo for movido para outro programa.

## Remover uma data de expiração {#remove-an-expiration-date}

1. Para remover uma data de expiração, verifique o(s) ativo(s) e clique em **[!UICONTROL Remover expiração]**.

   ![](assets/local-asset-expiration-8.png)

1. Revise os ativos afetados e clique em **[!UICONTROL Confirmar]**.

   ![](assets/local-asset-expiration-9.png)

>[!NOTE]
>
>Datas de expiração com menos de 15 minutos não podem ser removidas. Para &quot;remover&quot; a expiração, você precisará aguardar a expiração do ativo e, em seguida, reaprová-lo ou reativá-lo.
