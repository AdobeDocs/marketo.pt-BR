---
description: Guia de solução de problemas de migração de usuário do Adobe IMS - Documentação do Marketo - Documentação do produto
title: Guia de solução de problemas de migração de usuário do Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e96bc8676a73694ec60f46bb045f2a6ea5d8069c
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Guia de solução de problemas de migração de usuário do Adobe IMS {#adobe-ims-user-migration-troubleshooting-guide}

Durante o processo de migração de usuário do IMS, um usuário do Adobe é criado para cada usuário do Marketo Engage que está sendo migrado (a menos que já exista com o mesmo endereço de email). Às vezes, ele não é criado, o que pode ser atribuído ao registro do usuário no Ative Diretory ou a problemas com o endereço de email. Quando isso acontecer, o administrador do Marketo Engage verá o motivo no campo status de migração do usuário no console de automigração.

## Mensagens de erro {#error-messages}

Primeiro, determine se o usuário precisa ser migrado ou não, pois isso afetará quais etapas de resolução seguir.

Use a seção &quot;Nesta página&quot; à direita para ir diretamente para um erro específico.

### Não está no diretório {#not-in-directory}

**Causa raiz**: o usuário não existe no Ative Diretory (AD). Para qualquer organização com SSO que tenha a sincronização do AD ativada, a criação de usuários é permitida somente por meio do Provedor de identidade (IdP). Dessa forma, o usuário não pôde ser adicionado por meio do Admin Console durante a migração.

**Resoluções**:

_Se o usuário não precisar ser migrado_ - O administrador do Marketo Engage pode ignorá-lo no Console de Migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

_Se o usuário precisar ser migrado_ - O usuário deve ser adicionado ao Ative Diretory com as devidas permissões por um administrador do sistema. Administrador do Marketo Engage para executar novamente a migração de usuário para este usuário no Console de migração.

### Caractere inválido do Gmail {#gmail-invalid-character}

**Causa raiz**: de acordo com a política de segurança da Adobe, os caracteres `.` e `+` não são permitidos em um endereço de email do Gmail. Ambos os caracteres são permitidos em endereços de email não Gmail.

**Resoluções**:

_Se o usuário não precisar ser migrado_ - O administrador do Marketo Engage pode ignorá-lo no Console de Migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

_Se o usuário precisar ser migrado_ - O endereço de email deve ser atualizado no Marketo Engage para estar em conformidade com a política de segurança da Adobe e verificado novamente. Administrador do Marketo para executar novamente a migração de usuário para este usuário no Console de migração.

### Usuário inativo {#inactive-user}

**Causa raiz**: a Sincronização com o AD está habilitada, e a conta federada do usuário existe, mas com status inativo/desabilitado.

**Resoluções**:

_Se o usuário não precisar ser migrado_ - O administrador do Marketo Engage pode ignorá-lo no Console de Migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

_Se for necessário migrar o usuário_, o status do usuário e as permissões adequadas deverão ser restaurados. Administrador do Marketo Engage para executar novamente a migração de usuário para este usuário no Console de migração.

### Não está no Domínio {#not-in-domain}

**Causa raiz**: a imposição de domínio está habilitada na Admin Console, mas o domínio do endereço de email do usuário não é um dos domínios permitidos.

**Resoluções**:

_Se o usuário não precisar ser migrado_ - O administrador do Marketo Engage pode ignorá-lo no Console de Migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

_Se o usuário precisar ser migrado_ - O endereço de email deve ser atualizado no Marketo Engage para estar em conformidade com a política de Imposição de Domínio (DE). Como alternativa, o Administrador do Sistema pode [mover o domínio](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} para outro diretório desabilitado de Imposição de Domínio (DE) ou [criar um novo diretório](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"} que não esteja na política DE. Administrador do Marketo Engage para executar novamente a migração de usuário para este usuário no Console de migração.

### Criar falha {#create-failure}

**Causa raiz**: este erro pode ser causado por vários motivos no back-end.

**Resoluções**:

Envie um caso de suporte com detalhes relevantes para o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

### Falha do usuário do Type2e {#type2e-user-failure}

**Causa raiz**: este erro pode ser causado por vários motivos no back-end.

**Resoluções**:

Envie um caso de suporte com detalhes relevantes para o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
