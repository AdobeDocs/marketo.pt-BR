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
**Categoria:** Acesso/validação\
**Mensagem:** A API está desabilitada para este usuário\
**O que está acontecendo:** O usuário não tem acesso à API\
**Etapas de solução de problemas:** O administrador do Salesforce precisa conceder acesso à API do usuário.

**Erro:** AUTHENTICATION_FAILURE\
**Categoria:** Autenticação\
**Mensagem:** invalid_grant: falha de autenticação\
**O que está acontecendo:** Falha na autenticação\
**Etapas de solução de problemas:** Desconecte-se do Salesforce e reconecte.

**Erro:** CANNOT_INSERT_UPDATE_ATIVATE_ENTITY\
**Categoria:** Acesso/validação\
**Mensagem:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Session expired or invalid&quot;}\
**O que está acontecendo:**

1 - O código do acionador está causando a falha da atualização.\
2 - O usuário não tem permissões de gravação no nível do objeto no objeto fornecido.

**Etapas de solução de problemas:**

1 - Revise o acionador que está falhando.\
2 - Conceda acesso de gravação ao usuário para o objeto OU desative o recurso que está tentando gravar no objeto.

**Erro:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoria:** Outro\
**Mensagem:** não é possível fazer referência ao lead convertido\
**O que está acontecendo:** Estamos tentando registrar em um cliente potencial convertido durante o Registro de Atividades Mais Recentes para Contatos e Clientes Potenciais. Também vi alguns desses para lançamentos.\
**Etapas de solução de problemas:** Relate quaisquer instâncias disso para nossa [equipe de suporte](https://nation.marketo.com/t5/Support/ct-p/Support).

**Erro:** ENTITY_IS_LOCKED\
**Categoria:** Acesso/validação\
**Mensagem:** a entidade está bloqueada para edição\
**O que está acontecendo:** O registro está em um processo de aprovação em que está bloqueado contra qualquer edição adicional até ser aprovado ou negado por uma pessoa que possui a aprovação.\
**Etapas de solução de problemas:** Veja acima.

**Erro:** EXPIRED_ACCESS
**Categoria:** Autenticação
**Mensagem:** invalid_grant: token de acesso/atualização expirado
**O que está acontecendo:** O token de acesso ou atualização expirou. Os tokens expiram com base em [configurações de sessão no Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Etapas de solução de problemas:** Você precisará autenticar novamente. Desconecte a conexão do Salesforce e reconecte.

**Erro:** FAILED_WRITE\
**Categoria:** Intermitente\
**Mensagem:** fim de arquivo atingido\
**O que está acontecendo:** Problema de desempenho com o Salesforce, provavelmente devido a acionadores abaixo do ideal no lado do cliente.\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, trabalhe com o administrador do Salesforce para solucionar um acionador problemático.

**Erro:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Categoria:** Acesso/validação
**Mensagem:** Varia de cliente para cliente.
**O que está acontecendo:** Falha em uma regra de validação personalizada para o objeto.
**Etapas de solução de problemas:** Verifique a regra de validação personalizada que está causando esse erro. Como esta é uma regra personalizada, o erro deve ser tratado de forma pontual.

**Erro:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoria:** Acesso/validação\
**Mensagem:** O valor não existe ou não corresponde aos critérios de filtro\
**O que está acontecendo:** Dados inválidos existentes no Salesforce são aplicados na atualização.\
**Etapas de solução de problemas:** Veja acima.

**Erro:** FIELD_INTEGRITY_EXCEPTION\
**Categoria:** Acesso/validação\
**Mensagem:** O país/território existente não reconhece o valor de estado para o campo: Código de Estado/Província\
**O que está acontecendo:** Dados inválidos existentes no Salesforce são aplicados na atualização.\
**Etapas de solução de problemas:** Veja acima.

**Erro:** INATIVE_ORGANIZATION\
**Categoria:** Autenticação\
**Mensagem:** invalid_grant: organização inativa\
**O que está acontecendo:** Sua organização do Salesforce não está mais ativa.
**Etapas de solução de problemas:** Desconecte e reconecte-se do Salesforce.

**Erro:** INATIVE_USER
**Categoria:** Autenticação
**Mensagem:** invalid_grant: usuário inativo
**O que está acontecendo:** O usuário do Salesforce não está mais ativo
**Etapas de solução de problemas:** Desconecte e reconecte-se do Salesforce.

**Erro:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Categoria:** Intermitente\
**Mensagem:** (nenhuma mensagem adicional)\
**O que está acontecendo:** A instância do Salesforce está no modo de manutenção.\
**Etapas de solução de problemas:** Aguarde até que a manutenção do sistema seja concluída e, em seguida, tente fazer o logon novamente.

**Erro:** INSUFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Categoria:** Acesso/validação
**Mensagem:** direitos de acesso insuficientes na id do objeto
**O que está acontecendo:** Sem acesso ao registro pai de uma tarefa.
**Etapas de solução de problemas:** Veja acima.

**Erro:** INSUFFICIENT_ACCESS_OR_READONLY\
**Categoria:** Acesso/validação
**Mensagem:** direitos de acesso insuficientes na id do objeto
**O que está acontecendo:** O log de Atividades Mais Recentes não pode editar o registro específico porque o usuário não tem acesso de gravação.\
**Etapas de solução de problemas:** Conceda acesso ao usuário no Salesforce OU desative o log de Atividades mais recentes para esse objeto para esse usuário.

**Erro:** INVALID_FIELD\
**Categoria:** Intermitente\
**Mensagem:** Net::ReadTimeout\
**O que está acontecendo:** A solicitação está expirando. Isso provavelmente é o resultado de muitas transações lentas.\
**Etapas de solução de problemas:** Revise as personalizações existentes para possíveis culpados pelos problemas de latência e/ou desative o log de Atividade mais recente para um ou todos os objetos para reduzir a carga.

**Erro:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoria:** Acesso/validação\
**Mensagem:** Não é possível criar/atualizar campos: MSE_Replied_c. Verifique as configurações de segurança deste campo.
**O que está acontecendo:** Os usuários não têm acesso de gravação aos campos personalizados Ações do Sales Insight necessários para executar a transação de log de Atividade mais recente. A equipe pode ter instalado o pacote, mas não habilitou os campos corretos para os usuários.\
**Etapas de solução de problemas:** O administrador do Salesforce precisa conceder acesso aos campos personalizados OU desativar o log de atividades mais recentes.

**Erro:** INVALID_GRANT\
**Categoria:** Autenticação\
**Mensagem:** invalid_grant: ip restrict\
**O que está acontecendo:** Estamos tentando acessar seu Salesforce, mas você tem Restrições de IP em vigor que estão nos impedindo de fazer isso.\
**Etapas de solução de problemas:** Seu administrador do Salesforce precisará incluir na lista de permissões nossos IPs. Os usuários devem entrar em contato com o Suporte para obter os endereços IP.

**Erro:** INVALID_TYPE\
**Categoria:** Acesso/validação\
**Mensagem:** CreatedDate, (SELECIONE a ID das tarefas) DO lead ONDE Email=&#39;emailid&#39;^ERRO em `Row:1:Column:53sObject` O tipo &#39;Lead&#39; não é suportado. Caso queira usar um objeto personalizado, não deixe de anexar o &quot;__c&quot; após o nome da entidade. Consulte seu WSDL ou descreva a chamada para obter os nomes apropriados
**O que está acontecendo:** Estamos tentando consultar um tipo de objeto do Salesforce ao qual o usuário não tem acesso. Provavelmente, isso está relacionado ao fato de o usuário não ter o acesso correto ao Objeto principal.\
**Etapas de solução de problemas:** Conceda acesso de Leitura e Atualização ao objeto de cliente potencial no Salesforce ou desative o registro em log de emails e o registro em log de Atividades Mais Recentes para os registros de cliente potencial.

**Erro:** QUERY_TIMEOUT\
**Categoria:** Intermitente\
**Mensagem:** Sua solicitação de consulta estava em execução por muito tempo\
**O que está acontecendo:** Veja acima.\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, trabalhe com seu administrador do Salesforce para solucionar um acionador problemático.

**Erro:** REQUEST_LIMIT_EXCEEDED\
**Categoria:** Intermitente\
**Mensagem:**
1 - Limite de ConcurrentPerOrgLongTxn excedido\
2 - Limite TotalRequests excedido\
3 - ConcurrentRequest\
**O que está acontecendo:**
1 - Limite de solicitação simultânea excedido, provavelmente devido ao código de acionador ineficiente.\
2 - Muitas integrações colocam a organização além da janela contínua de 24 horas.\
**Etapas de solução de problemas:**
1 - Revise os acionadores existentes nos objetos afetados. Possivelmente desative o registro de roll-up para um ou mais objetos.\
2 - Compre mais chamadas de API do Salesforce. Possivelmente desative o registro de roll-up para um ou mais objetos.

**Erro:** CAMPO_OBRIGATÓRIO_AUSENTE\
**Categoria:** Acesso/validação\
**Mensagem:** Campos obrigatórios ausentes: `[Amount_Committed_Private_Capital__c]`
**O que está acontecendo:** Isso geralmente acontece para o registro de atividade mais recente. Campos personalizados foram configurados para serem obrigatórios, mas contêm valores vazios. Isso pode acontecer se o registro tiver sido criado com um valor vazio do campo personalizado e tiver sido transformado em obrigatório. A exigência é imposta quando estamos tentando atualizar o registro, mesmo que não estejamos tocando no campo personalizado.\
**Etapas de solução de problemas:** Atualize manualmente os valores dos campos ausentes. Em seguida, você pode tentar novamente a mensagem a partir das Ações do Sales Insight.

**Erro:** SERVIDOR_INDISPONÍVEL\
**Categoria:** Intermitente\
**Mensagem:** servidor muito ocupado\
**O que está acontecendo:** Problema de desempenho com o Salesforce, provavelmente devido a acionadores abaixo do ideal pelo cliente\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, fale com o administrador do Salesforce para solucionar problemas com um acionador problemático.

**Erro:** TXN_SECURITY_NO_ACCESS\
**Categoria:** Acesso/validação\
**Mensagem:** A operação solicitada não é permitida devido a uma política de segurança em sua organização. Entre em contato com o administrador.
**O que está acontecendo:** Algum tipo de restrição de segurança foi configurada - consulte https://developer.salesforce.com/forums/?id=&quot;record ID&quot;\
**Etapas de solução de problemas:** Converse com o administrador do Salesforce e veja qual pode ser a restrição específica.

**Erro:** UNABLE_TO_LOCK_ROW\
**Categoria:** Intermitente\
**Mensagem:** não é possível obter acesso exclusivo a este registro ou 1 registro: &quot;ID do registro&quot;\
**O que está acontecendo:** Provavelmente, há um acionador que está causando várias tentativas de acesso ao mesmo registro, possivelmente no caso de um email de grupo.\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, trabalhe com seu administrador do Salesforce para solucionar um acionador problemático.

**Erro:** EXCEÇÃO_DESCONHECIDA
**Categoria:** Outro\
**Mensagem:** Ocorreu uma exceção desconhecida\
**O que está acontecendo:** Exceção sem tratamento no Salesforce.\
**Etapas de solução de problemas:** Registre um caso com o Salesforce e copie os valores numéricos na mensagem de erro. Esse é o código do Salesforce que não trata um erro corretamente.
