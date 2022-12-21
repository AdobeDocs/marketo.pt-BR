---
description: Salesforce Diagnostics - Documentos do Marketo - Documentação do produto
title: Salesforce Diagnostics
hide: true
hidefromtoc: true
exl-id: c449f938-9615-47cb-b232-613ec29068a3
source-git-commit: d960f0ad0d944bd2e74543f3ab15b59a8040b768
workflow-type: tm+mt
source-wordcount: '1445'
ht-degree: 1%

---

# Salesforce Diagnostics {#salesforce-diagnostics}

Parte de nossa integração com o Salesforce inclui uma página de diagnóstico do Salesforce no aplicativo Web. Esta página captura erros do registro de dados com falha para o Salesforce. Os erros podem ser úteis, mas nem sempre podem ser lidos. Assim, montamos um gabarito que ajuda a explicar as mensagens de erro.

## Diagnóstico de acesso {#access-diagnostics}

1. Clique no ícone de engrenagem e escolha **Configurações**.

   ![](assets/salesforce-diagnostics-1.png)

1. Em Integrações, clique em **Diagnóstico**.

   ![](assets/salesforce-diagnostics-2.png)

## Folha de Cálculo de Erro {#error-cheat-sheet}

**Erro:** API_CURRENTLY_DISABLED\
**Categoria:** Acesso/validação\
**Mensagem:** A API está desativada para este usuário\
**O que está acontecendo:** O usuário não tem acesso à API\
**Etapas de solução de problemas:** O administrador do Salesforce precisa conceder o acesso à API do usuário.

**Erro:** AUTENTICATION_FAILURE\
**Categoria:** Autenticação\
**Mensagem:** invalid_grant: falha de autenticação\
**O que está acontecendo:** Falha na autenticação\
**Etapas de solução de problemas:** Desconecte-se do Salesforce e reconecte-se.

**Erro:** CANNOT_INSERT_UPDATE_ACTIVATE_ENTITY\
**Categoria:** Acesso/validação\
**Mensagem:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Sessão expirada ou inválida&quot;}\
**O que está acontecendo:**

1 - O código do acionador está causando falha na atualização.\
2 - O usuário não tem permissões de gravação no nível do objeto em um determinado objeto.

**Etapas de solução de problemas:**

1 - Revise o acionador que está falhando.\
2 - Conceda acesso de gravação ao usuário para o objeto OU desative o recurso que está tentando gravar no objeto.

**Erro:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoria:** Outras\
**Mensagem:** não é possível referenciar lead convertido\
**O que está acontecendo:** Estamos tentando fazer logon em um lead convertido durante o Registro de atividade mais recente para contatos e leads. Também vi alguns desses para pontos.\
**Etapas de solução de problemas:** Relate quaisquer instâncias disso à nossa [equipe de suporte](https://nation.marketo.com/t5/Support/ct-p/Support).

**Erro:** ENTITY_IS_LOCKED\
**Categoria:** Acesso/validação\
**Mensagem:** a entidade está bloqueada para edição\
**O que está acontecendo:** O registro está em um processo de aprovação em que é bloqueado de qualquer edição adicional até ser aprovado ou negado por uma pessoa que possui a aprovação.\
**Etapas de solução de problemas:** Veja acima.

**Erro:** EXPIRED_ACCESS
**Categoria:** Autenticação
**Mensagem:** invalid_grant: token de acesso/atualização expirado
**O que está acontecendo:** O token de acesso ou atualização expirou. Os tokens expiram com base em [configurações de sessão no Salesforce](https://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Etapas de solução de problemas:** Você precisará autenticar novamente. Desconecte a conexão do Salesforce e reconecte.

**Erro:** FAILED_WRITE\
**Categoria:** Intermitente\
**Mensagem:** fim do arquivo atingido\
**O que está acontecendo:** Problema de desempenho com o Salesforce, provavelmente devido a acionadores com erros ideais no lado do cliente.\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, trabalhe com o administrador do Salesforce para solucionar problemas em um acionador.

**Erro:** FIELD_CUSTOM_VALIDATION_EXCEPTION
**Categoria:** Acesso/validação
**Mensagem:** Varia de cliente para cliente.
**O que está acontecendo:** Falha em uma regra de validação personalizada para o objeto.
**Etapas de solução de problemas:** Verifique a regra de validação personalizada que está causando esse erro. Uma vez que se trata de uma regra personalizada, o erro deve ser tratado numa base pontual.

**Erro:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoria:** Acesso/validação\
**Mensagem:** O valor não existe ou não corresponde aos critérios de filtro\
**O que está acontecendo:** Dados incorretos existentes no Salesforce são aplicados após a atualização.\
**Etapas de solução de problemas:** Veja acima.

**Erro:** FIELD_INTEGRITY_EXCEPTION\
**Categoria:** Acesso/validação\
**Mensagem:** O país/território existente não reconhece o valor do estado para o campo: Código de Estado/Província\
**O que está acontecendo:** Dados incorretos existentes no Salesforce são aplicados após a atualização.\
**Etapas de solução de problemas:** Veja acima.

**Erro:** INATIVE_ORGANIZATION\
**Categoria:** Autenticação\
**Mensagem:** invalid_grant: organização inativa\
**O que está acontecendo:** Sua organização do Salesforce não está mais ativa.
**Etapas de solução de problemas:** Desconecte e reconecte do Salesforce.

**Erro:** INATIVE_USER
**Categoria:** Autenticação
**Mensagem:** invalid_grant: usuário inativo
**O que está acontecendo:** O usuário do Salesforce não está mais ativo
**Etapas de solução de problemas:** Desconecte e reconecte do Salesforce.

**Erro:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Categoria:** Intermitente\
**Mensagem:** (sem mensagem adicional)\
**O que está acontecendo:** A instância do Salesforce está em modo de manutenção.\
**Etapas de solução de problemas:** Aguarde até que a manutenção do sistema seja concluída e tente novamente o registro.

**Erro:** INSUFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY
**Categoria:** Acesso/validação
**Mensagem:** direitos de acesso insuficientes na id do objeto
**O que está acontecendo:** Sem acesso ao registro pai de uma tarefa.
**Etapas de solução de problemas:** Veja acima.

**Erro:** INSUFICIENT_ACCESS_OR_READONLY\
**Categoria:** Acesso/validação
**Mensagem:** direitos de acesso insuficientes na id do objeto
**O que está acontecendo:** O registro de atividades mais recentes não pode editar o registro específico porque o usuário não tem acesso de gravação para gravação.\
**Etapas de solução de problemas:** Conceda ao usuário acesso no Salesforce OU desative o registro de atividades mais recentes para esse objeto para esse usuário.

**Erro:** INVALID_FIELD\
**Categoria:** Intermitente\
**Mensagem:** Net::ReadTimeout\
**O que está acontecendo:** A solicitação está expirando. Isso provavelmente é resultado de muitas transações lentas.\
**Etapas de solução de problemas:** Revise as personalizações existentes para possíveis culpados dos problemas de latência e/ou desative o registro de Atividades Mais Recentes para um ou todos os objetos para reduzir a carga.

**Erro:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoria:** Acesso/validação\
**Mensagem:** Não é possível criar/atualizar campos: MSE_Replied__c. Verifique as configurações de segurança deste campo.
**O que está acontecendo:** Os usuários não têm acesso de gravação aos campos personalizados Ações de insight de vendas necessários para executar a transação de registro de atividade mais recente. O grupo pode ter instalado o pacote, mas não ativou os campos corretos para os usuários.\
**Etapas de solução de problemas:** O administrador do Salesforce precisa conceder acesso aos campos personalizados OU desativar o registro de atividades mais recentes.

**Erro:** INVALID_GRANT\
**Categoria:** Autenticação\
**Mensagem:** invalid_grant: ip restrito\
**O que está acontecendo:** Estamos tentando acessar seu Salesforce, mas você tem Restrições de IP em vigor que estão nos impedindo de fazê-lo.\
**Etapas de solução de problemas:** Seu administrador do Salesforce precisará lista de permissões seus IPs. Os usuários devem entrar em contato com o Suporte para obter os endereços IP.

**Erro:** INVALID_TYPE\
**Categoria:** Acesso/validação\
**Mensagem:** CreatedDate, (SELECIONAR Id DE Tarefas) DO Lead ONDE Email=&#39;emailid&#39;^ERROR na Linha:1:Coluna:Tipo de objeto &#39;Lead&#39; 53s não é suportado. Caso queira usar um objeto personalizado, não deixe de anexar o &quot;__c&quot; após o nome da entidade. Consulte seu WSDL ou a chamada de descrição para os nomes apropriados
**O que está acontecendo:** Estamos tentando consultar um tipo de objeto do Salesforce ao qual o usuário não tem acesso. Isso provavelmente está relacionado ao usuário que não tem o acesso correto ao Objeto de lead.\
**Etapas de solução de problemas:** Conceda acesso de Leitura e Atualização ao objeto Lead no Salesforce ou desative o registro de e-mail e o registro de Atividade Mais Recente para registros de leads.

**Erro:** QUERY_TIMEOUT\
**Categoria:** Intermitente\
**Mensagem:** Sua solicitação de consulta estava sendo executada por muito tempo\
**O que está acontecendo:** Veja acima.\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, trabalhe com o administrador do Salesforce para solucionar problemas em um acionador.

**Erro:** REQUEST_LIMIT_EXCEEDED\
**Categoria:** Intermitente\
**Mensagem:**
1 - Limite ConcurrentPerOrgLongTxn excedido\
2 - Limite de TotalRequests excedido\
3 - ConcurrentRequest\
**O que está acontecendo:**
1 - O limite de solicitação concorrente foi excedido, provavelmente devido ao código de acionador ineficiente.\
2 - Muitas integrações colocam a organização além da janela do acumulado de 24 horas.\
**Etapas de solução de problemas:**
1 - Revise os acionadores existentes nos objetos afetados. Possivelmente, desative o registro de roll-up de um ou mais objetos.\
2 - Compre mais chamadas de API do Salesforce. Possivelmente, desative o registro de roll-up de um ou mais objetos.

**Erro:** Required_FIELD_MISSING\
**Categoria:** Acesso/validação\
**Mensagem:** Campos obrigatórios estão ausentes: `[Amount_Committed_Private_Capital__c]`
**O que está acontecendo:** Isso geralmente acontece no registro de atividades mais recentes. Campos personalizados foram configurados para serem obrigatórios, mas têm valores vazios. Isso pode acontecer se o registro tiver sido criado com um valor vazio do campo personalizado e tiver sido feito para ser obrigatório. O requisito é aplicado quando estamos tentando atualizar o registro, mesmo que não estejamos tocando no campo personalizado.\
**Etapas de solução de problemas:** Atualize manualmente os valores dos campos ausentes. Você pode repetir a mensagem em Ações de insight de vendas.

**Erro:** SERVER_UNAVAILABLE\
**Categoria:** Intermitente\
**Mensagem:** servidor muito ocupado\
**O que está acontecendo:** Problema de desempenho com o Salesforce, provavelmente devido a acionadores sub-ideais pelo cliente\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, trabalhe com o administrador do Salesforce para solucionar problemas em um acionador problemático.

**Erro:** TXN_SECURITY_NO_ACCESS\
**Categoria:** Acesso/validação\
**Mensagem:** A operação solicitada não é permitida devido a uma política de segurança na organização. Procure o administrador.
**O que está acontecendo:** Algum tipo de restrição de segurança foi configurada - consulte https://developer.salesforce.com/forums/?id=&quot;ID de registro&quot;\
**Etapas de solução de problemas:** Fale com o administrador do Salesforce e veja qual pode ser a restrição específica.

**Erro:** UNABLE_TO_LOCK_ROW\
**Categoria:** Intermitente\
**Mensagem:** Impossível obter acesso exclusivo a este registro ou a 1 registros: &quot;record ID&quot;\
**O que está acontecendo:** Provavelmente, há um acionador que está causando várias tentativas de acessar o mesmo registro, possivelmente no caso de um email de grupo.\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, trabalhe com o administrador do Salesforce para solucionar problemas em um acionador.

**Erro:** UNKNOWN_EXCEPTION
**Categoria:** Outras\
**Mensagem:** Ocorreu uma Exceção Desconhecida\
**O que está acontecendo:** Exceção não tratada no Salesforce.\
**Etapas de solução de problemas:** Registre um caso com o Salesforce e copie os valores numéricos na mensagem de erro. Este é o código Salesforce que não está manipulando um erro corretamente.
