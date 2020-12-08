---
unique-page-id: 14745730
description: Salesforce Diagnostics - Documentos do Marketing - Documentação do produto
title: Salesforce Diagnostics
translation-type: tm+mt
source-git-commit: 44ed91b485b52173922c709de63a4353e16c5072
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 0%

---


# Salesforce Diagnostics {#salesforce-diagnostics}

Parte de nossa integração com o Salesforce inclui uma página de diagnóstico do Salesforce no aplicativo da Web. Esta página captura erros de registro de dados com falha para o Salesforce. Os erros podem ser úteis, mas nem sempre são legíveis. Assim, montamos uma folha de trapos que ajuda a explicar as mensagens de erro.

**Erro:** API_CURRENTLY_DISABLED\
**Categoria:** Acesso/validação\
**Mensagem:** A API está desabilitada para este usuário\
**O que está acontecendo:** O usuário não tem acesso à API\
**Etapas de solução de problemas:** O administrador do Salesforce precisa conceder acesso à API do usuário.

<br> 

**Erro:** AUTHENTICATION_FAILURE\
**Categoria:** Autenticação\
**Mensagem:** invalid_Grant: falha de autenticação\
**O que está acontecendo:** Falha na autenticação\
**Etapas de solução de problemas:** Desconecte-se do Salesforce e reconecte-se.

<br> 

**Erro:** CANNOT_INSERT_UPDATE_ATIVATE_ENTITY\
**Categoria:** Acesso/validação\
**Mensagem:** {&quot;errorCode&quot;:&quot;INVALID_SESSION_ID&quot;,&quot;message&quot;:&quot;Sessão expirada ou inválida&quot;}\
**O que está acontecendo:**

1 - O código do acionador está causando falha na atualização.\
2 - O usuário não tem permissões de gravação no nível do objeto no objeto em questão.

**Etapas de solução de problemas:**

1 - Revise o acionador que está falhando.\
2 - conceda acesso de gravação ao usuário para o objeto OU desative o recurso que está tentando gravar no objeto.

<br> 

**Erro:** CANNOT_UPDATE_CONVERTED_LEAD\
**Categoria:** Outros\
**Mensagem:** não é possível referenciar cliente potencial convertido\
**O que está acontecendo:** Estamos tentando fazer logon em um cliente potencial convertido durante o Registro de Atividade mais recente para Contatos e Clientes potenciais. Também vi alguns desses para pontos.\
**Etapas de solução de problemas:** Por favor, comunique quaisquer exemplos disso à nossa equipe [de](http://nation.marketo.com/community/support_solutions)suporte.

<br> 

**Erro:** ENTITY_IS_LOCKED\
**Categoria:** Acesso/validação\
**Mensagem:** a entidade está bloqueada para edição\
**O que está acontecendo:** O registro está em um processo de aprovação no qual está bloqueado de quaisquer edições adicionais até que seja aprovado ou negado por uma pessoa proprietária da aprovação.\
**Etapas de solução de problemas:** Consulte acima.

<br> 

**Erro:** EXPIRED_ACCESS **Categoria:** Mensagem de autenticação **:** invalid_Grant: token **de acesso/atualização expiradoO que está acontecendo:** O token de acesso ou atualização expirou. Tokens expiram com base nas configurações de [sessão no Salesforce](http://salesforce.stackexchange.com/questions/10759/invalid-grant-expired-access-refresh-token-error-when-authenticating-access-via).
**Etapas de solução de problemas:** Você precisará autenticar novamente. Desconecte a conexão do Salesforce e reconecte-se.

<br> 

**Erro:** FAILED_WRITE\
**Categoria:** Intermitente\
**Mensagem:** fim do arquivo atingido\
**O que está acontecendo:** Problema de desempenho com o Salesforce, provavelmente devido a acionadores inadequados do lado do cliente.\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, entre em contato com o administrador do Salesforce para solucionar problemas em um acionador problemático.

<br> 

**Erro:** FIELD_CUSTOM_VALIDATION_EXCEPTION **Categoria:** Acesso/**Mensagem de validação:** Varia de cliente para cliente.
**O que está acontecendo:** Falha em uma regra de validação personalizada para o objeto.
**Etapas de solução de problemas:** Verifique a regra de validação personalizada que está causando esse erro. Dado que se trata de uma regra personalizada, o erro deve ser tratado numa base pontual.

<br> 

**Erro:** FIELD_FILTER_VALIDATION_EXCEPTION\
**Categoria:** Acesso/validação\
**Mensagem:** O valor não existe ou não corresponde aos critérios do filtro\
**O que está acontecendo:** Dados incorretos existentes no Salesforce são aplicados na atualização.\
**Etapas de solução de problemas:** Consulte acima.

<br> 

**Erro:** FIELD_INTEGRITY_EXCEPTION\
**Categoria:** Acesso/validação\
**Mensagem:** O país/território existente não reconhece o valor do estado para o campo: Código do Estado/Província\
**O que está acontecendo:** Dados incorretos existentes no Salesforce são aplicados na atualização.\
**Etapas de solução de problemas:** Consulte acima.

<br> 

**Erro:** INATIVE_ORGANIZATION\
**Categoria:** Autenticação\
**Mensagem:** invalid_Grant: organização inativa\
**O que está acontecendo:** Sua organização do Salesforce não está mais ativa.\
**Etapas de solução de problemas:** Desconecte e reconecte-se do Salesforce.

**Erro:** CATEGORIA INATIVE_USER **:** Mensagem de autenticação **:** invalid_Grant: usuário **inativo O que está acontecendo:** O usuário do Salesforce não está mais ativo **nas Etapas de solução de problemas:** Desconecte e reconecte-se do Salesforce.

**Erro:** INSERT_UPDATE_DELETE_NOT_ALLOWED_DURING_MAINTENANCE\
**Categoria:** Intermitente\
**Mensagem:** (nenhuma mensagem adicional)\
**O que está acontecendo:** A instância do Salesforce está no modo de manutenção.\
**Etapas de solução de problemas:** Aguarde até que a manutenção do sistema seja concluída e tente registrar novamente.

**Erro:** INSUFICIENT_ACCESS_ON_CROSS_REFERENCE_ENTITY **Categoria:** Acesso/**Mensagem de validação:** direitos de acesso insuficientes na ID **do objetoO que está acontecendo:** Nenhum acesso ao registro pai para uma tarefa.
**Etapas de solução de problemas:** Consulte acima.

<br> 

**Erro:** INSUFICIENT_ACCESS_OR_READONLY\
**Categoria:** Acesso/Validação** ****Mensagem:** direitos de acesso insuficientes na id do objeto******O que está acontecendo:** O registro de Atividades mais recente não pode editar o registro específico porque o usuário não tem acesso de gravação a.\
**Etapas de solução de problemas:** Conceda ao usuário acesso no Salesforce OU desative o registro de Atividade mais recente para esse objeto do usuário.

**Erro:** INVALID_FIELD\
**Categoria:** Intermitente\
**Mensagem:** Net::ReadTimeout\
**O que está acontecendo:** A solicitação está expirando. Isso é provavelmente resultado de muitas transações lentas.\
**Etapas de solução de problemas:** Analise as personalizações existentes para possíveis culpados de problemas de latência e/ou desative o registro de Atividade mais recente para um ou todos os objetos para reduzir a carga.

**Erro:** INVALID_FIELD_FOR_INSERT_UPDATE\
**Categoria:** Acesso/validação\
**Mensagem:** Não é possível criar/atualizar campos: ToutApp__Tout_Last_Replied__c. Verifique as configurações de segurança deste campo.\
**O que está acontecendo:** Os usuários não têm acesso de gravação aos campos personalizados Tout necessários para executar a transação de registro de Atividade mais recente. O grupo pode ter instalado o pacote, mas não habilitou os campos corretos para os usuários.\
**Etapas de solução de problemas:** O administrador do Salesforce precisa conceder acesso aos campos personalizados OU desativar o registro de Atividades mais recentes.

**Erro:** INVALID_GRANT\
**Categoria:** Autenticação\
**Mensagem:** invalid_Grant: ip restrito\
**O que está acontecendo:** Estamos tentando acessar seu Salesforce, mas você tem Restrições de IP em vigor que estão nos impedindo de fazê-lo.\
**Etapas de solução de problemas:** Seu administrador do Salesforce precisará lista de permissões nossos IPs. Os usuários devem entrar em contato com o Suporte para obter os endereços IP.

**Erro:** INVALID_TYPE\
**Categoria:** Acesso/validação\
**Mensagem:** CreatedDate, (SELECT Id FROM Tarefa) FROM Lead WHERE Email=&#39;emailid&#39;^ERROR at Row:1:Column:53sO tipo de objeto &#39;Lead&#39; não é suportado. Se você estiver tentando usar um objeto personalizado, certifique-se de anexar &#39;__c&#39; após o nome da entidade. Consulte seu WSDL ou a chamada de descrição para obter os nomes apropriados\
**O que está acontecendo:** Estamos tentando query de um tipo de objeto do Salesforce ao qual o usuário não tem acesso. Provavelmente, isso está relacionado ao usuário que não tem o acesso correto ao Objeto principal.\
**Etapas de solução de problemas:** Conceda acesso de Leitura e Atualização ao objeto Lead no Salesforce ou desativa o registro de e-mail e o registro de Atividades Mais Recentes para registros de clientes potenciais.

**Erro:** QUERY_TIMEOUT\
**Categoria:** Intermitente\
**Mensagem:** Sua solicitação de query estava sendo executada por muito tempo\
**O que está acontecendo:** Consulte acima.\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, entre em contato com o administrador do Salesforce para solucionar problemas em um acionador problemático.

**Erro:** REQUEST_LIMIT_EXCEEDED\
**Categoria:** Intermitente\
**Mensagem:**
1 - Limite de ConcurrentPerOrgLongTxn excedido\
2 - Limite TotalRequests excedido\
3 - ConcurrentRequest\
**O que está acontecendo:**
1 - Limite de solicitações simultâneas excedido, provavelmente devido ao código de disparo ineficiente.\
2 - Muitas integrações colocam a organização além da janela acumulada de 24 horas.\
**Etapas de solução de problemas:**
1 - Revise acionadores existentes nos objetos afetados. Possivelmente desative o registro de roll-up para um ou mais objetos.\
2 - Compre mais chamadas de API do Salesforce. Possivelmente desative o registro de roll-up para um ou mais objetos.

**Erro:** REQUIRED_FIELD_MISSING\
**Categoria:** Acesso/validação\
**Mensagem:** Os campos obrigatórios estão ausentes: [Amount_Commited_Private_Capital__c]\
**O que está acontecendo:** Isso geralmente acontece para o registro de Atividades mais recentes. Campos personalizados foram configurados para serem obrigatórios, mas têm valores vazios neles. Isso pode acontecer se o registro tiver sido criado com um valor vazio do campo personalizado e, em seguida, for feito como obrigatório. A exigência é imposta quando estamos tentando atualizar o registro, mesmo que não estejamos tocando no campo personalizado.\
**Etapas de solução de problemas:** Atualize manualmente os valores dos campos ausentes. Em seguida, você pode repetir a mensagem do ToutApp.

**Erro:** SERVER_UNAVAILABLE\
**Categoria:** Intermitente\
**Mensagem:** servidor muito ocupado\
**O que está acontecendo:** Problema de desempenho com o Salesforce, provavelmente devido a acionadores sub-ótimos pelo cliente\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, trabalhe com seu administrador do Salesforce para solucionar problemas em um acionador problemático.

**Erro:** TXN_SECURITY_NO_ACCESS\
**Categoria:** Acesso/validação\
**Mensagem:** A operação solicitada não é permitida devido a uma política de segurança em sua organização. Entre em contato com o administrador.\
**O que está acontecendo:** Foi configurado algum tipo de restrição de segurança - consulte `https://developer.salesforce.com/forums/?id="record` ID&quot;\
**Etapas de solução de problemas:** Fale com seu administrador do Salesforce e veja qual restrição específica pode ser.

**Erro:** UNABLE_TO_LOCK_ROW\
**Categoria:** Intermitente\
**Mensagem:** Impossível obter acesso exclusivo a este registro ou a 1 registros: &quot;record ID&quot;\
**O que está acontecendo:** Provavelmente, há um acionador que está fazendo várias tentativas de acessar o mesmo registro, possivelmente no caso de um email de grupo.\
**Etapas de solução de problemas:** A lógica de repetição deve lidar com isso. Se ainda não estiver funcionando, entre em contato com o administrador do Salesforce para solucionar problemas em um acionador problemático.

**Erro:** UNKNOWN_EXCEPTION\
**Categoria:** Outros\
**Mensagem:** Ocorreu uma Exceção Desconhecida\
**O que está acontecendo:** Exceção não tratada no Salesforce.\
**Etapas de solução de problemas:** Registre um caso com o Salesforce e copie os valores numéricos na mensagem de erro. Este é o código do Salesforce que não está manipulando um erro corretamente.
