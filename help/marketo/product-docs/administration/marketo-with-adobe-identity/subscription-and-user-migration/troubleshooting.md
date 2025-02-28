---
description: Guia de solução de problemas do Adobe IMS - Documentação do Marketo - Documentação do produto
title: Guia de solução de problemas do Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: 2a01045abbc23bce9531c64e3494fb12a9adf1bd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Guia de solução de problemas do Adobe IMS {#adobe-ims-troubleshooting-guide}

Durante o processo de migração de usuário do IMS, um usuário do Adobe é criado para cada usuário do Marketo Engage que está sendo migrado. Às vezes, ele não é criado (por vários motivos, relacionados ao registro do usuário no Ative Diretory ou a problemas com o endereço de email). Quando isso acontecer, o administrador do Marketo Engage verá o motivo no campo status de migração do usuário no console de automigração.

## Mensagens de erro {#error-messages}

Use a seção &quot;Nesta página&quot; à direita para ir diretamente para um erro específico e saber como resolvê-lo.

### Não está no diretório {#not-in-directory}

_Causa raiz_: o usuário não existe no Ative Diretory (AD). Para qualquer organização com SSO que tenha a sincronização do AD ativada, a criação de usuários é permitida somente por meio do Provedor de identidade (IdP). Dessa forma, o usuário não pôde ser adicionado por meio do Admin Console durante a migração.

_Resoluções_:

Pré-migração - O administrador do Marketo Enage deve ignorar o usuário no Console de migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

Pós-migração - O usuário deve ser adicionado ao Ative Diretory com as permissões adequadas. Administrador do Marketo Engage para executar novamente a migração de usuário para este usuário no Console de migração.

### Caractere inválido do Gmail {#gmail-invalid-character}

_Causa raiz_: de acordo com a política de segurança da Adobe, os caracteres `.` e `+` não são permitidos em um endereço de email do Gmail. Ambos os caracteres são permitidos em endereços de email não Gmail.

_Resoluções_:

Pré-migração - O administrador do Marketo Enage deve ignorar o usuário no Console de migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

Pós-migração - O endereço de email deve ser atualizado no Marketo Engage para estar em conformidade com a política de segurança da Adobe. Admin do Marketo para executar novamente a migração de usuário para este usuário no Console de migração.

### Usuário inativo {#inactive-user}

_Causa raiz_: a Sincronização com o AD está habilitada, e a conta federada do usuário existe, mas com status inativo/desabilitado.

_Resoluções_:

Pré-migração - O administrador do Marketo Enage deve ignorar o usuário no Console de migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

Pós-migração - O status do usuário e as permissões apropriadas devem ser restaurados. Administrador do Marketo Engage para executar novamente a migração de usuário para este usuário no Console de migração.

### Não está no Domínio {#not-in-domain}

_Causa raiz_: a imposição de domínio está habilitada na Admin Console, mas o domínio do endereço de email do usuário não é um dos domínios permitidos.

_Resoluções_:

Pré-migração - O administrador do Marketo Enage deve ignorar o usuário no Console de migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

Pós-migração - O endereço de email deve ser atualizado no Marketo Engage para estar em conformidade com a política de Imposição de domínio (DE). Como alternativa, o Administrador do Sistema pode [mover o domínio](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} para outro diretório desabilitado de Imposição de Domínio (DE) ou [criar um novo diretório](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"} que não esteja na política DE. Administrador do Marketo Engage para executar novamente a migração de usuário para este usuário no Console de migração.

### Criar falha {#create-failure}

_Causa raiz_: este erro pode ser causado por vários motivos no back-end.

_Resoluções_:

Pré-migração - Envie um caso de suporte para os [ainda não migrados](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Pós-migração - Envie um caso de suporte para os [já migrados](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.

### Falha do usuário do Type2e {#type2e-user-failure}

_Causa raiz_: este erro pode ser causado por vários motivos no back-end.

_Resoluções_:

Pré-migração - Envie um caso de suporte para os [ainda não migrados](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Pós-migração - Envie um caso de suporte para os [já migrados](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.
