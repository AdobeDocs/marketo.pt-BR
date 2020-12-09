---
unique-page-id: 8783322
description: Validar Microsoft Dynamics Sync - Documentos do Marketing - Documentação do produto
title: Validar Microsoft Dynamics Sync
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Validar Microsoft Dynamics Sync {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Se a Autenticação Multifator (MFA) estiver ativada para sua Sincronização Dinâmica, você deverá desativá-la para que a Dinâmica seja sincronizada corretamente com o Marketo. Para obter informações adicionais, entre em contato com o suporte [do](http://nation.marketo.com/community/support_solutions)Marketing.

## Executar Validar sincronização no Marketo {#run-validate-sync-in-marketo}

É muito importante executar a ferramenta Validar sincronização para garantir que a sincronização do Microsoft Dynamics com o Marketo esteja configurada corretamente antes de estabelecer a conexão final entre eles. O processo gera uma lista de verificação de sete etapas de configuração que indicam onde existem problemas. Verificar se eles foram feitos corretamente pode economizar muito tempo depois.

1. Clique na guia **Admin** e, em seguida, no link **Microsoft Dynamics** na área Integração.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Selecione **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Clique na guia **Validar configuração** de sincronização.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Digite seu nome de usuário, senha e URL (a ID do cliente e o segredo do cliente são opcionais). Clique em **Avançar** quando terminar.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Se você já tiver sincronizado antes, o **CRM** na árvore esquerda lerá o **Microsoft Dynamics** e os dados no formulário acima poderão ser pré-preenchidos.

1. Se tudo estiver bem, a opção Validar sincronização gerará uma lista de verificação cheia de marcas de seleção verdes ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Se você vir um ![—](assets/delete.png), então essa etapa tem um problema. Consulte [Corrigir problemas](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) de sincronização de validação dinâmica para identificar e corrigir o problema. Em seguida, execute novamente as etapas de validação de sincronização até que o resultado se pareça com a imagem acima.

   >[!CAUTION]
   >
   >No momento, não oferecemos suporte à atualização da caixa de proteção para a Sincronização Dinâmica do Marketing. Se precisar atualizar sua caixa de proteção do Dynamics CRM, uma nova caixa de proteção do Marketo será necessária. Entre em contato com o Gerente de sucesso do cliente para obter mais detalhes.

>[!MORELIKETHIS]
>
>[Corrigir problemas de sincronização de validação do Dynamics](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)

