---
description: Diagnósticos do Salesforce - Documentação do Marketo - Documentação do produto
title: Diagnósticos do Salesforce
exl-id: c449f938-9615-47cb-b232-613ec29068a3
feature: Sales Insight Actions
source-git-commit: 9384d72b335a4b975b190816ea999ad067fddeda
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 1%

---

# Diagnósticos do Salesforce {#salesforce-diagnostics}

Parte de nossa integração com o Salesforce inclui uma página de Diagnóstico do Salesforce no aplicativo da Web. Esta página captura erros do registro de dados com falha no Salesforce. Os erros podem ser úteis, mas nem sempre são legíveis. Dessa forma, criamos uma folha de características que ajuda a explicar as mensagens de erro.

## Diagnóstico de acesso {#access-diagnostics}

1. Clique no ícone de engrenagem e escolha **Configurações**.

   ![](assets/salesforce-diagnostics-1.png)

1. Em Integrações, clique em **Diagnóstico**.

   ![](assets/salesforce-diagnostics-2.png)

## Folha de características de erro {#error-cheat-sheet}

**Erro:** API_CURRENTLY_DISABLED\
**Categoria:** Acesso/Validação\
**Mensagem:** API desabilitada para este usuário\
**O que está acontecendo:** o usuário não tem Acesso à API\
**Etapas de solução de problemas:** O administrador do Salesforce precisa conceder acesso à API do usuário.

**Erro:** AUTHENTICATION_FAILURE\
**Categoria:** Autenticação\
**Mensagem:** invalid_grant: falha de autenticação\
**O que está acontecendo:** Falha na autenticação\
**Etapas de Solução de Problemas:** Desconecte-se do Salesforce e reconecte.

**Erro:** CANNOT_INSERT_UPDATE_ATIVATE_ENTITY\
**Categoria:** Acesso/Validação\
**Mensagem:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;mensagem&quot;:&quot;Sessão expirada ou inválida&quot;}\
**O que está acontecendo:**

1 - O código do acionador está causando a falha da atualização.\
2 - O usuário não tem permissões de gravação no nível do objeto no objeto fornecido.

**Etapas de Solução de Problemas:**

1 - Revise o acionador que está falhando.\
2 - Conceda acesso de gravação ao usuário para o objeto OU desative o recurso que está tentando gravar no objeto.

**Erro:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoria:** Outro\
**Mensagem:** não pode fazer referência ao lead convertido\
**O que está acontecendo:** estamos tentando fazer logon em um cliente potencial convertido durante o Registro de Atividades Mais Recentes para Contatos e Clientes Potenciais. Também vi alguns desses para lançamentos.\
**Etapas de solução de problemas:** relate qualquer instância disso à nossa [equipe de suporte](https://nation.marketo.com/t5/Support/ct-p/Support).

**Erro:** ENTITY_IS_LOCKED\
**Categoria:** Acesso/Validação\
**Mensagem:** a entidade está bloqueada para edição\
**O que está acontecendo:** o registro está em um processo de aprovação em que está bloqueado contra qualquer edição adicional até ser aprovado ou negado por uma pessoa que possui a aprovação.\
**Etapas de Solução de Problemas:** Veja acima.

**Erro:** EXPIRED_ACCESS
**Categoria:** Autenticação
**Mensagem:** invalid_grant: token de acesso/atualização expirado
**O que está acontecendo:** O token de acesso ou atualização expirou. Os tokens expiram com base nas [configurações de sessão no Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Etapas de Solução de Problemas:** Será necessário autenticar novamente. Desconecte a conexão do Salesforce e reconecte.

**Erro:** FAILED_WRITE\
**Categoria:** Intermitente\
**Mensagem:** fim de arquivo atingido\
**O que está acontecendo:** problema de desempenho com o Salesforce, provavelmente devido a disparadores inadequados no lado do cliente.\
**Etapas de Solução de Problemas:** A lógica de repetição deve tratar disso. Se ainda não estiver funcionando, trabalhe com o administrador do Salesforce para solucionar um acionador problemático.

**Erro:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Categoria:** Acesso/Validação
**Mensagem:** varia de cliente para cliente.
**O que está acontecendo:** Falha em uma regra de validação personalizada para o objeto.
**Etapas de Solução de Problemas:** Verifique a regra de validação personalizada que está causando esse erro. Como esta é uma regra personalizada, o erro deve ser tratado de forma pontual.

**Erro:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoria:** Acesso/Validação\
**Mensagem:** o valor não existe ou não corresponde aos critérios de filtro\
**O que está acontecendo:** Dados inválidos existentes no Salesforce que são aplicados na atualização.\
**Etapas de Solução de Problemas:** Veja acima.

**Erro:** FIELD_INTEGRITY_EXCEPTION\
**Categoria:** Acesso/Validação\
**Mensagem:** o país/território existente não reconhece o valor de estado para o campo: Código de Estado/Província\
**O que está acontecendo:** Dados inválidos existentes no Salesforce que são aplicados na atualização.\
**Etapas de Solução de Problemas:** Veja acima.

**Erro:** INATIVE_ORGANIZATION\
**Categoria:** Autenticação\
**Mensagem:** invalid_grant: organização inativa\
**O que está acontecendo:** sua organização do Salesforce não está mais ativa.
**Etapas de Solução de Problemas:** Desconecte e reconecte novamente do Salesforce.

**Erro:** INATIVE_USER
**Categoria:** Autenticação
**Mensagem:** invalid_grant: usuário inativo
**O que está acontecendo:** o usuário do Salesforce não está mais ativo
**Etapas de Solução de Problemas:** Desconecte e reconecte novamente do Salesforce.

**Erro:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Categoria:** Intermitente\
**Mensagem:** (nenhuma mensagem adicional)\
**O que está acontecendo:** a instância do Salesforce está no modo de manutenção.\
**Etapas de Solução de Problemas:** Aguarde até que a manutenção do sistema seja concluída e tente fazer o log novamente.

**Erro:** INSUFFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Categoria:** Acesso/Validação
**Mensagem:** direitos de acesso insuficientes na ID do objeto
**O que está acontecendo:** nenhum acesso ao registro pai de uma tarefa.
**Etapas de Solução de Problemas:** Veja acima.

**Erro:** INSUFFICIENT_ACCESS_OR_READONLY\
**Categoria:** Acesso/Validação
**Mensagem:** direitos de acesso insuficientes na ID do objeto
**O que está acontecendo:** O log de Atividade mais recente não pode editar o registro específico porque o usuário não tem acesso de gravação.\
**Etapas de Solução de Problemas:** Conceda ao usuário acesso no Salesforce OU desabilite o log de Atividades Mais Recentes para esse objeto para esse usuário.

**Erro:** INVALID_FIELD\
**Categoria:** Intermitente\
**Mensagem:** Net::ReadTimeout\
**O que está acontecendo:** a solicitação está expirando. Isso provavelmente é o resultado de muitas transações lentas.\
**Etapas de Solução de Problemas:** Revise as personalizações existentes para possíveis culpados pelos problemas de latência e/ou desabilite o log de Atividades Mais Recentes para um ou todos os objetos para reduzir a carga.

**Erro:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoria:** Acesso/Validação\
**Mensagem:** Não é possível criar/atualizar campos: MSE_Replied__c. Verifique as configurações de segurança deste campo.
**O que está acontecendo:** os usuários não têm acesso de gravação aos campos personalizados de Ações de Insight de Vendas necessários para executar a transação de log da Atividade Mais Recente. A equipe pode ter instalado o pacote, mas não habilitou os campos corretos para os usuários.\
**Etapas de solução de problemas:** O administrador do Salesforce precisa conceder acesso aos campos personalizados OU desativar o log de Atividades Mais Recentes.

**Erro:** INVALID_GRANT\
**Categoria:** Autenticação\
**Mensagem:** invalid_grant: ip restrito\
**O que está acontecendo:** Estamos tentando acessar sua Salesforce, mas você tem Restrições de IP em vigor que nos impedem de fazer isso.\
incluir na lista de permissões **Etapas de solução de problemas:** O administrador do Salesforce precisará verificar nossos IPs. Os usuários devem entrar em contato com o Suporte para obter os endereços IP.

**Erro:** INVALID_TYPE\
**Categoria:** Acesso/Validação\
**Mensagem:** CreatedDate, (SELECT Id FROM Tasks) FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at `Row:1:Column:53sObject` type &#39;Lead&#39; não tem suporte. Caso queira usar um objeto personalizado, não deixe de anexar o &quot;__c&quot; após o nome da entidade. Consulte seu WSDL ou descreva a chamada para obter os nomes apropriados
**O que está acontecendo:** estamos tentando consultar um tipo de objeto do Salesforce ao qual o usuário não tem acesso. Provavelmente, isso está relacionado ao fato de o usuário não ter o acesso correto ao Objeto principal.\
**Etapas de Solução de Problemas:** conceda acesso de Leitura e Atualização ao objeto de Cliente Potencial no Salesforce ou desative o log de emails e o log de Atividades Mais Recentes para os registros de cliente potencial.

**Erro:** QUERY_TIMEOUT\
**Categoria:** Intermitente\
**Mensagem:** sua solicitação de consulta foi executada por muito tempo\
**O que está acontecendo:** Veja acima.\
**Etapas de Solução de Problemas:** A lógica de repetição deve tratar disso. Se ainda não estiver funcionando, trabalhe com seu administrador do Salesforce para solucionar um acionador problemático.

**Erro:** REQUEST_LIMIT_EXCEEDED\
**Categoria:** Intermitente\
**Mensagem:**
1 - Limite de ConcurrentPerOrgLongTxn excedido\
2 - Limite TotalRequests excedido\
3 - ConcurrentRequest\
**O que está acontecendo:**
1 - Limite de solicitação simultânea excedido, provavelmente devido ao código de acionador ineficiente.\
2 - Muitas integrações colocam a organização além da janela contínua de 24 horas.\
**Etapas de Solução de Problemas:**
1 - Revise os acionadores existentes nos objetos afetados. Possivelmente desative o registro de roll-up para um ou mais objetos.\
2 - Compre mais chamadas de API do Salesforce. Possivelmente desative o registro de roll-up para um ou mais objetos.

**Erro:** REQUIRED_FIELD_MISSING\
**Categoria:** Acesso/Validação\
**Mensagem:** Campos obrigatórios ausentes: `[Amount_Committed_Private_Capital__c]`
**O que está acontecendo:** Isso geralmente acontece no log de Atividades Mais Recentes. Campos personalizados foram configurados para serem obrigatórios, mas contêm valores vazios. Isso pode acontecer se o registro tiver sido criado com um valor vazio do campo personalizado e tiver sido transformado em obrigatório. A exigência é imposta quando estamos tentando atualizar o registro, mesmo que não estejamos tocando no campo personalizado.\
**Etapas de Solução de Problemas:** atualize manualmente os valores dos campos ausentes. Em seguida, você pode tentar novamente a mensagem a partir das Ações do Sales Insight.

**Erro:** SERVER_UNAVAILABLE\
**Categoria:** Intermitente\
**Mensagem:** servidor muito ocupado\
**O que está acontecendo:** problema de desempenho com o Salesforce, provavelmente devido a disparadores insuficientes do cliente\
**Etapas de Solução de Problemas:** A lógica de repetição deve tratar disso. Se ainda não estiver funcionando, fale com o administrador do Salesforce para solucionar problemas com um acionador problemático.

**Erro:** TXN_SECURITY_NO_ACCESS\
**Categoria:** Acesso/Validação\
**Mensagem:** a operação solicitada não é permitida devido a uma política de segurança em sua organização. Entre em contato com o administrador.
**O que está acontecendo:** Algum tipo de restrição de segurança foi configurada - consulte https://developer.salesforce.com/forums/?id=&quot;ID do registro&quot;\
**Etapas de solução de problemas:** converse com o administrador do Salesforce e veja qual pode ser a restrição específica.

**Erro:** UNABLE_TO_LOCK_ROW\
**Categoria:** Intermitente\
**Mensagem:** não é possível obter acesso exclusivo a este registro ou 1 registro: &quot;ID do registro&quot;\
**O que está acontecendo:** Provavelmente há um disparador que está causando várias tentativas de acessar o mesmo registro, possivelmente no caso de um email de grupo.\
**Etapas de Solução de Problemas:** A lógica de repetição deve tratar disso. Se ainda não estiver funcionando, trabalhe com seu administrador do Salesforce para solucionar um acionador problemático.

**Erro:** UNKNOWN_EXCEPTION
**Categoria:** Outro\
**Mensagem:** Exceção desconhecida ocorreu\
**O que está acontecendo:** Exceção sem tratamento no Salesforce.\
**Etapas de solução de problemas:** arquive um caso com o Salesforce e copie os valores numéricos na mensagem de erro. Esse é o código do Salesforce que não trata um erro corretamente.
