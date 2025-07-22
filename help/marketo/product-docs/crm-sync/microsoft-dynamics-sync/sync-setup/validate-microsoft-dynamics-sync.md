---
unique-page-id: 8783322
description: Validar [!DNL Microsoft Dynamics] Sincronização - Documentação do Marketo - Documentação do produto
title: Validar [!DNL Microsoft Dynamics] Sincronizar
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# Validar a sincronização de [!DNL Microsoft Dynamics] {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Se a Autenticação Multifator (MFA) estiver habilitada para a Sincronização do [!DNL Dynamics], você deverá desabilitá-la para que o [!DNL Dynamics] seja sincronizado corretamente com o Marketo. Para obter informações adicionais, contate o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

## Executar Validar sincronização no Marketo {#run-validate-sync-in-marketo}

É muito importante executar a ferramenta Validar Sincronização para verificar se a Sincronização do [!DNL Microsoft Dynamics] com o Marketo está configurada corretamente antes de fazer a conexão final entre elas. O processo gera uma lista de verificação de sete etapas de configuração que indicam onde existem problemas. A verificação de que eles foram feitos corretamente pode economizar muito tempo depois.

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
   >Se você tiver sincronizado anteriormente, o **CRM** na árvore esquerda lerá **[!DNL Microsoft Dynamics]** e os dados no formulário acima poderão ser pré-preenchidos.

1. Se tudo estiver bem, a Sincronização de Validação gera uma lista de verificação cheia de marcas de seleção verdes ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Se você vir um ![—](assets/delete.png), essa etapa tem um problema. Consulte [Corrigir [!DNL Dynamics] Problemas de Sincronização de Validação](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) para identificar e corrigir o problema. Em seguida, execute novamente as etapas de validação de sincronização até que o resultado se pareça com a imagem acima.

   >[!CAUTION]
   >
   >No momento, não oferecemos suporte à atualização da sandbox para a sincronização [!DNL Marketo Dynamics]. Se precisar atualizar sua sandbox do CRM [!DNL Dynamics], uma nova sandbox da Marketo será necessária. Entre em contato com o Gerente de sucesso do cliente para obter mais detalhes.

>[!MORELIKETHIS]
>
>[Correção [!DNL Dynamics] Problemas de Sincronização de Validação](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
