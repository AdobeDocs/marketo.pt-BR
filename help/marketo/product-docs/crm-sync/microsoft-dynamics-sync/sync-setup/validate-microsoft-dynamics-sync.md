---
unique-page-id: 8783322
description: Validar a sincronização do Microsoft Dynamics - Documentação do Marketo - Documentação do produto
title: Validar a sincronização do Microsoft Dynamics
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Validar a sincronização do Microsoft Dynamics {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Se a Autenticação Multifator (MFA) estiver habilitada para o Dynamics Sync, desabilite-a para que o Dynamics seja sincronizado corretamente com o Marketo. Para obter informações adicionais, contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

## Executar Validar sincronização no Marketo {#run-validate-sync-in-marketo}

É muito importante executar a ferramenta Validar sincronização para garantir que a sincronização do Microsoft Dynamics com o Marketo esteja configurada corretamente antes de fazer a conexão final entre elas. O processo gera uma lista de verificação de sete etapas de configuração que indicam onde existem problemas. A verificação de que eles foram feitos corretamente pode economizar muito tempo depois.

1. Clique na guia **[!UICONTROL Admin]** e depois no link **[!DNL Microsoft Dynamics]** na área de Integração.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Selecione **[!DNL Microsoft]**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Clique na guia **[!UICONTROL Validar configuração de sincronização]**.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Insira seu nome de usuário, senha e URL (ID do cliente e segredo do cliente são opcionais). Clique em **[!UICONTROL Avançar]** quando terminar.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Se você tiver sincronizado anteriormente, o **[!UICONTROL CRM]** na árvore esquerda lerá **[!DNL Microsoft Dynamics]** e os dados no formulário acima poderão ser pré-preenchidos.

1. Se tudo estiver bem, a Sincronização de Validação gera uma lista de verificação cheia de marcas de seleção verdes ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Se você vir um ![—](assets/delete.png), essa etapa tem um problema. Consulte [Corrigir problemas de sincronização de validação do Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"} para identificar e corrigir o problema. Em seguida, execute novamente as etapas de validação de sincronização até que o resultado se pareça com a imagem acima.

   >[!CAUTION]
   >
   >No momento, não oferecemos suporte à atualização de sandbox para o Marketo Dynamics Sync. Se você precisar atualizar sua sandbox do Dynamics CRM, uma nova sandbox do Marketo será necessária. Entre em contato com a equipe de conta do Adobe (seu gerente de conta) para obter mais detalhes.

>[!MORELIKETHIS]
>
>[Corrigir Problemas De Sincronização De Validação Do Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md){target="_blank"}
