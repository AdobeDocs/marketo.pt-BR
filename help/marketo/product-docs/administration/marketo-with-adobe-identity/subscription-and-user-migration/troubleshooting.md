---
description: Guia de solução de problemas de migração de usuário do Adobe IMS - Documentação do Marketo - Documentação do produto
title: Guia de solução de problemas de migração de usuário do Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: c5b05cf7d1131c9d98d89c12a4a8bd04d215886d
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 1%

---

# Guia de solução de problemas de migração de usuário do Adobe IMS {#adobe-ims-user-migration-troubleshooting-guide}

Durante o processo de migração de usuário do IMS, um usuário do Adobe é criado para cada usuário do Marketo Engage que está sendo migrado (a menos que já exista com o mesmo endereço de email). Às vezes, ele não é criado, o que pode ser atribuído ao registro do usuário no Ative Diretory ou a problemas com o endereço de email.

Este artigo, para usuários que executam migrações automáticas, lista cada mensagem de erro que pode ser exibida no campo status do console de migração automática.

>[!NOTE]
>
>Os erros relacionados ao diretório/domínio podem ser acionados por outra organização/Admin Console em que uma relação de confiança de diretório está configurada ou o domínio foi reivindicado.

## Mensagens de erro {#error-messages}

Primeiro, determine se o usuário precisa ser migrado ou não, pois isso afetará quais etapas de resolução seguir.

Use a seção &quot;Nesta página&quot; à direita para ir diretamente para um erro específico.

### Caractere inválido do Gmail {#gmail-invalid-character}

**Causa raiz**: de acordo com a política de segurança da Adobe, os caracteres `.` e `+` não são permitidos em um endereço de email do Gmail. Ambos os caracteres são permitidos em endereços de email não Gmail.

**Resoluções**:

_Se for necessário migrar o usuário_ - O endereço de email deve ser atualizado no Marketo Engage para estar em conformidade com a política de segurança da Adobe e verificado novamente. Administrador do Marketo para executar novamente a migração de usuário para este usuário no Console de migração.

_Se o usuário **não**precisar ser migrado_ - o administrador do Marketo Engage precisará ignorá-lo no Console de Migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

### Usuário não está no diretório {#user-not-in-directory}

**Causa raiz**: o usuário não existe no Ative Diretory (AD). Para qualquer organização com SSO que tenha a sincronização do AD ativada, a criação de usuários é permitida somente por meio do Provedor de identidade (IdP). Dessa forma, o usuário não pôde ser adicionado por meio do Admin Console durante a migração.

**Resoluções**:

_Se o usuário precisar ser migrado_ - O usuário deve ser adicionado ao Ative Diretory com as permissões adequadas por um administrador do sistema. Administrador do Marketo Engage para executar novamente a migração de usuário para este usuário no Console de migração.

_Se o usuário **não**precisar ser migrado_ - o administrador do Marketo Engage precisará ignorá-lo no Console de Migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

### Usuário inativo {#inactive-user}

**Causa raiz**: a Sincronização com o AD está habilitada, e a conta federada do usuário existe, mas com status inativo/desabilitado.

**Resoluções**:

_Se for necessário migrar o usuário_ - O status do usuário e as permissões adequadas devem ser restaurados por um administrador do sistema. Administrador do Marketo Engage para executar novamente a migração de usuário para este usuário no Console de migração.

_Se o usuário **não**precisar ser migrado_ - o administrador do Marketo Engage precisará ignorá-lo no Console de Migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

### Domínio inválido {#invalid-domain}

**Causa raiz**: a imposição de domínio está habilitada na Admin Console. No entanto, o domínio do endereço de email do usuário não é um dos domínios permitidos ou o domínio foi reivindicado em outra organização/Admin Console.

**Resoluções**:

_Se for necessário migrar o usuário_ (e a imposição de domínio estiver habilitada na organização de migração) - O endereço de email deve ser atualizado no Marketo Engage para estar em conformidade com a política de Imposição de Domínio (DE). Como alternativa, o Administrador do Sistema pode [mover o domínio](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} para outro diretório desabilitado de Imposição de Domínio (DE) ou [criar um novo diretório](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"} que não esteja na política DE. Administrador do Marketo Engage para executar novamente a migração de usuário para este usuário no Console de migração.

_Se for necessário migrar o usuário_ (e a imposição de domínio estiver habilitada em outra organização), um administrador do sistema da organização em que o domínio foi reivindicado precisa adicionar o endereço de email do usuário à lista de exceções. Administrador do Marketo Engage para executar novamente a migração de usuário para este usuário no Console de migração.

_Se o usuário **não**precisar ser migrado_ - o administrador do Marketo Engage precisará ignorá-lo no Console de Migração. O botão &quot;Migração concluída&quot; aparece quando todos os usuários são considerados ao migrar ou ignorar o. Clique no botão para concluir o processo de migração do usuário.

**As mensagens de erro a seguir têm a mesma causa raiz/resolução...**

### Falha na criação do usuário {#user-creation-failed}

[Veja abaixo](#failed)

### Falha de Type2E {#type2e-failure}

[Veja abaixo](#failed)

### Falha das prerrogativas do Marketo  {#marketo-entitlement-failed}

[Veja abaixo](#failed)

### Falha na migração do Pendo {#pendo-migration-failed}

[Veja abaixo](#failed)

### Falha na migração de dados do usuário {#user-data-migration-failed}

[Veja abaixo](#failed)

### Falha na sincronização dos dados do produto {#product-data-sync-failed}

[Veja abaixo](#failed)

### Falha na qualificação para o Adobe {#adobe-entitlement-failed}

[Veja abaixo](#failed)

### Falha ao sair do usuário {#user-sign-out-failed}

[Veja abaixo](#failed)

### Falha na criação do Adobe ID {#adobe-id-creation-failed}

[Veja abaixo](#failed)

### Falha {#failed}

**Causa raiz**: esses erros podem ser causados por vários motivos no back-end.

**Resoluções**:

Envie um caso de suporte com detalhes relevantes para o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
