---
description: Explore o conjunto de agentes do Marketo AI projetados para automatizar tarefas de marketing como controle de qualidade do programa, importação de clientes potenciais, normalização de dados e muito mais.
title: Folha de informações de dados da IA do Marketo
badge: beta
hide: true
source-git-commit: 39fef7edc7c475efd901a75235ccf7b25f789793
workflow-type: tm+mt
source-wordcount: '1478'
ht-degree: 0%

---

# Folha de informações de dados da IA do Marketo {#data-information}

A IA do Marketo é um recurso nativo e prático da Adobe Marketo Engage que permite que as equipes de operações de marketing automatizem fluxos de trabalho selecionados por meio da interação em linguagem natural, incluindo importação de clientes potenciais, validação de programas, normalização de dados, criação de programas, investigação de clientes potenciais, análise e orientação de produtos. A IA do Marketo opera no ambiente Marketo Engage existente de um usuário e usa a infraestrutura gerenciada pela Adobe para raciocínio e orquestração de IA.

**Ambiente de usuário:** a IA do Marketo opera em um ambiente Marketo Engage existente e não apresenta um novo caminho de compartilhamento de usuário para usuário.

**Escopo dos dados:** o serviço processa dados de marketing B2B padrão já presentes no ambiente do usuário, incluindo registros de cliente potencial, dados de programa e atividade de campanha inteligente.

**Serviços de IA:** a IA do Marketo aproveita um recurso de IA criado pela Adobe e usa o Azure OpenAI GPT-4.1 e o Claude no AWS Bedrock para raciocínio de IA, com ferramentas MCP do Marketo que oferecem suporte à execução de ações de produtos.

**Governança:** as saídas geradas por IA permanecem no ambiente do usuário e estão sujeitas aos controles existentes de governança, residência e retenção.

**Transparência:** as saídas geradas por IA podem ser revisadas por meio de histórico de conversa e auditoria para oferecer suporte à supervisão do usuário.

## Controles de acesso e implantação

### Importar clientes em potencial

**Função:** processa dados de cliente potencial fornecidos pelo usuário para mapeamento, normalização, desduplicação e importação para o Marketo Engage.

### Controle de qualidade do programa

**Função:** avalia os programas do Marketo em relação às regras organizacionais definidas pelos usuários em um arquivo de Markdown de Habilidade, como padrões de nomenclatura, status de aprovação, conformidade de email e lógica de fluxo.

### Criar programa a partir do resumo

**Função:** usa prompts em linguagem natural para gerar estruturas de programa do Marketo, incluindo campanhas inteligentes, etapas de fluxo e espaços reservados para conteúdo, diretamente no ambiente do usuário.

### Agentes chamáveis

**Função:** executa ações de IA acionadas por ação de fluxo nas etapas de fluxo do Smart Campaign para casos de uso como validação, normalização e detecção de bot.

### Investigação de lead

**Função:** fornece uma análise conversacional do motivo pelo qual uma pessoa avançou ou não para uma etapa examinando a execução da etapa de fluxo e a associação à lista inteligente.

### Measurement and analytics

**Função:** mostra a análise de desempenho da campanha e do programa, incluindo recomendações e insights de causa raiz.

### Conhecimento do produto

**Função:** fornece orientação prática recomendada e como da Marketo por meio de uma camada de conhecimento compartilhada usada na experiência do agente.

## Casos de uso

Além dos listados, considere usar a IA do Marketo para diagnosticar e solucionar problemas operacionais complexos (falhas de sincronização de CRM, erros de webhook, análise de causa principal de delivery de email, incompatibilidades de campo), realizar auditorias em sua conta (capacidade de delivery de email, conformidade do centro de subscrição, revisões de campanhas inteligentes, avaliações de modelos de pontuação) e acelerar a criação de programas a partir de resumos e modelos (programas de eventos, campanhas de email em vários idiomas, configurações de webinário). O recurso adicional foi projetado para ajudar na classificação de clientes potenciais assistidos por IA e no enriquecimento de dados em escala, na análise de desempenho com recomendações de correção e na depuração guiada de configurações técnicas, como scripts Velocity e modelos de ciclo de vida.

## Status de disponibilidade e implantação

**Qualificação:** a habilitação inicial de usuário está limitada aos usuários qualificados do Marketo Engage que aceitaram o Adobe Gen AI Rider.

**Provisionamento:** o acesso é gerenciado por meio de controles de habilitação de produtos existentes e do provisionamento de sinalizador de recursos na experiência do Marketo Engage.

**Modelo de implantação:** a implantação avança por meio da Alpha e da Private Beta antes de uma expansão mais ampla da Beta Pública.

**Escopo geográfico:** a versão inicial destina-se a usuários globais do Marketo Engage, excluindo a China continental.

**Escopo do setor:** a implantação atual não inclui recursos verticais específicos para setores altamente regulamentados, como saúde, serviços financeiros, governo ou defesa.

## Documentação e suporte

**Documentação:** a documentação do Experience League está sendo expandida como parte da disponibilidade geral.

**Modelo de suporte:** A abordagem de suporte atual inclui entrada de comentários do usuário, horário comercial e uma comunidade Experience League da Marketo AI.

**Monitoramento de serviço:** o Adobe identifica a observabilidade, os painéis de comentários e os mecanismos de avaliação de qualidade como componentes importantes da maturidade da inicialização e do aprimoramento contínuo.

## Dados e exclusões fora do escopo

**Nenhum dado de categoria especial:** a IA do Marketo não introduz um novo processamento para dados de saúde, financeiros, de localização precisa, biométricos ou outros dados de categoria especial.

**Nenhum novo caminho de compartilhamento:** O serviço não cria um novo mecanismo de compartilhamento de conteúdo de usuário para usuário.

**Saídas contidas pelo usuário:** as saídas geradas por IA permanecem no ambiente Marketo Engage existente do usuário sob os controles de governança existentes.

**Exclusões atuais:** a implantação inicial exclui a China continental e não fornece recursos verticais específicos para setores altamente regulamentados.

## Uso do Azure OpenAI e do Claude no AWS Bedrock

Esta seção explica como o Azure OpenAI oferece suporte aos fluxos de trabalho do Marketo AI. Quaisquer diagramas ou descrições de fluxo relacionados devem ser lidos juntamente com os controles descritos aqui, incluindo limitações no escopo dos dados, supervisão do usuário e treinamento do modelo.

**Propósito:** o Azure OpenAI GPT-4.1 é usado para raciocínio conversacional e orquestração de fluxos de trabalho orientados por agente.

**Escopo dos dados:** As entradas estão limitadas aos dados de marketing B2B padrão já presentes no ambiente Marketo Engage do usuário e necessários para preencher o fluxo de trabalho solicitado.

**Saída de IA:** as saídas de IA são determinadas por prompts e configuração do usuário, e os recursos de IA do Marketo não tomam decisões de forma autônoma sem a configuração do usuário.

**Treinamento:** a Adobe não usa dados do usuário para treinar ou ajustar modelos do Azure OpenAI para este serviço.

**Supervisão do usuário:** as saídas geradas por IA permanecem revisáveis no Marketo Engage por meio de recursos de histórico de conversa e auditoria.

## Retenção e armazenamento de dados

**Saídas contidas pelo usuário:** saídas geradas por IA, como listas de clientes potenciais limpas, relatórios de controle de qualidade, estruturas de programa geradas e dados normalizados, permanecem no ambiente Marketo Engage do usuário.

**Alinhamento de governança:** Os dados de saída permanecem sujeitos aos controles de governança, residência e retenção de dados existentes no Marketo Engage.

**Nenhum novo repositório entre usuários:** O serviço não apresenta um caminho de compartilhamento de dados separado de usuário para usuário.

## Locais de processamento e armazenamento de dados

Esta seção resume os ambientes nos quais a IA do Marketo opera e onde ocorre o processamento. Se o documento incluir diagramas regionais ou visuais de infraestrutura, esses materiais devem ser entendidos como representações de alto nível do local de serviço e do fluxo de processamento, em vez de esquemas de rede exaustivos.

**Ambiente de aplicativo:** a IA do Marketo opera dentro do ambiente Adobe Marketo Engage existente do usuário.

**Processamento de IA:** o Marketo AI usa o Azure OpenAI GPT-4.1 e o Claude no AWS Bedrock para raciocínio conversacional e orquestração de tarefas.

**Local dos dados do usuário:** os dados do usuário e as saídas geradas por IA permanecem no ambiente Marketo Engage do usuário e estão sujeitos aos controles existentes de residência, governança e retenção do usuário.

**Nenhum repositório entre usuários separado:** O serviço não introduz uma camada de armazenamento ou compartilhamento de dados separada entre usuários.

## Considerações sobre PII e privacidade de dados

### Escopo de dados por tipo de fluxo de trabalho

Os dados processados pela IA do Marketo são determinados pelo padrão de uso do usuário e pelo fluxo de trabalho específico chamado. Nem todos os fluxos de trabalho exigem dados de nível de lead de processamento.

### Fluxos de trabalho que processam somente metadados da campanha (sem PII do cliente potencial)

* Criação de programa a partir de resumo — gera estruturas de programa, campanhas inteligentes, etapas de fluxo e espaços reservados para conteúdo a partir de instruções em linguagem natural
* Clonagem e tradução de e-mails — duplica e traduz conteúdo do HTML por e-mail, linhas de assunto e cópia de marketing em variantes de idioma
* Auditoria de campanha — analisa configurações inteligentes de campanha, definições de acionador/filtro, lógica de fluxo e convenções de nomenclatura
* Validação de controle de qualidade do programa — avalia os programas em relação às regras definidas pelo usuário para conformidade, status de aprovação e integridade estrutural
* Revisões do centro de assinaturas e da arquitetura do programa — analisa a lógica da campanha e a estrutura do programa
* Conhecimento do produto e orientação de práticas recomendadas — fornece respostas práticas da Marketo a partir de uma camada de conhecimento compartilhada

### Fluxos de trabalho que processam registros de nível de lead (campos de contato B2B padrão)

* Investigação e solução de problemas de clientes potenciais: examina valores de campo de clientes potenciais individuais, histórico de atividades e progressão do ciclo de vida para diagnosticar por que um cliente potencial atingiu ou não o MQL ou se qualificou para uma campanha de marketing
* Importação e normalização de clientes potenciais — processa dados de clientes potenciais fornecidos pelo usuário, inclusive nomes, endereços de email, números de telefone e campos da empresa para mapeamento, limpeza e desduplicação
* Classificação e enriquecimento de clientes potenciais: avalia os registros de clientes potenciais em relação à pontuação ou lógica de classificação definida pelo usuário (por exemplo, clientes potenciais válidos vs. spam para integridade do banco de dados, personalidades para fins de personalização, clientes potenciais de negócios com clientes potenciais de email corporativo versus clientes potenciais de consumidor)
* Auditorias de qualidade e capacidade de entrega de dados — analisa dados de contrato de nível de lead, padrões de rejeição e registros duplicados para identificar problemas de integridade do banco de dados
* Análise de desempenho do Campaign — padrões de envolvimento de clientes potenciais de superfícies, dados de conversão e composição de público para oferecer suporte à análise de desempenho

### Minimização de dados por design

* Em todos os casos, os dados enviados para o modelo de IA são limitados ao necessário para atender à solicitação específica do usuário nesse fluxo de trabalho
* A IA herda as permissões existentes do Marketo Engage do usuário solicitante — não é possível acessar registros, campos ou programas de clientes potenciais além do que o usuário já pode visualizar por meio da interface do usuário do produto
* Os workflows investigativos e de operações de dados exigem necessariamente dados de nível de lead, pois o usuário está pedindo explicitamente à IA que analise, classifique ou aja nesses registros
* os usuários que desejam limitar o processamento de dados de clientes potenciais podem restringir o acesso às ferramentas fluxos de trabalho de investigação por meio dos controles de permissões e funções existentes do Marketo Engage, mantendo o acesso total aos recursos de IA estruturais e administrativos

### Sem exposição de dados incremental

A IA funciona como um acelerador nas permissões do usuário existentes, não como um caminho de escalonamento. Um usuário que não consegue visualizar determinados campos, programas ou partições principais na interface do usuário do Marketo Engage também não pode exibir esses dados por meio da IA do Marketo. O serviço não ignora regras de partição, permissões em nível de campo ou restrições de espaço de trabalho.
