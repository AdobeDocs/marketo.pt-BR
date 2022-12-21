---
unique-page-id: 8783322
description: Validar o Microsoft Dynamics Sync - Documentos do Marketo - Documentação do produto
title: Validar a sincronização do Microsoft Dynamics
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# Validar a sincronização do Microsoft Dynamics {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Se a Autenticação de vários fatores (MFA) estiver ativada para a Sincronização dinâmica, é necessário desativá-la para que o Dynamics sincronize corretamente com a Marketo. Para obter mais informações, entre em contato com o [Suporte Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

## Executar Validar Sincronização no Marketo {#run-validate-sync-in-marketo}

É muito importante executar a ferramenta Validar sincronização para garantir que a sincronização do Microsoft Dynamics com o Marketo esteja configurada corretamente antes de fazer a conexão final entre elas. O processo gera uma lista de verificação de sete etapas de configuração que identificam onde existem problemas. Verificar se eles foram feitos corretamente pode economizar muito tempo depois.

1. Clique no botão **Administrador** e depois a guia **Microsoft Dynamics** na área Integração.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Selecionar **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Clique no botão **Validar Configuração de Sincronização** guia .

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Insira seu nome de usuário, senha e URL (ID do cliente e Segredo do cliente são opcionais). Clique em **Próximo** quando concluído.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Se você já sincronizou antes, **CRM** na árvore da esquerda será lido **Microsoft Dynamics** e os dados no formulário acima podem ser pré-preenchidos.

1. Se tudo estiver bem, a Validar sincronização gera uma lista de verificação cheia de marcas de seleção verdes ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Se você vir uma ![—](assets/delete.png), então essa etapa tem um problema. Consulte [Corrigir problemas de sincronização de validação do Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) para identificar e corrigir o problema. Em seguida, execute novamente as etapas de validação de sincronização até que o resultado se pareça com a imagem acima.

   >[!CAUTION]
   >
   >No momento, não oferecemos suporte à atualização da caixa de proteção para a Sincronização do Marketo Dynamics. Se você precisar atualizar a caixa de proteção do Dynamics CRM, será necessária uma nova caixa de proteção do Marketo. Entre em contato com o Gerente de sucesso do cliente para obter mais detalhes.

>[!MORELIKETHIS]
>
>[Corrigir problemas de sincronização de validação do Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
