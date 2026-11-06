---
description: Use agentes com chamada no CX Enterprise Coworker para Marketo Engage a fim de executar etapas de IA em Campanhas inteligentes que limpam, classificam, enriquecem ou filtram dados de leads.
title: Agentes chamáveis
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
source-git-commit: 16b8e470bd4a4460c0179ccdd406ef89af7e9e17
workflow-type: tm+mt
source-wordcount: '2002'
ht-degree: 1%
---
# Agentes chamáveis {#callable-agents}

Os agentes com chamada permitem usar um agente de IA como uma etapa em uma Campanha inteligente do Marketo Engage. Crie um agente no CX Enterprise Coworker para Marketo Engage, escolha os campos de clientes potenciais que lê e atualiza e publique-o para uso em campanhas. Os agentes podem ajudar a limpar dados, classificar clientes potenciais, enriquecer informações ausentes ou filtrar envios de formulários.

>[!PREREQUISITES]
>
>Você deve ter a permissão **Acessar administrador** no Marketo Engage.

## Antes de começar {#before-you-begin}

- Decida quais campos de cliente potencial o agente precisa ler e quais campos ele deve atualizar. Cada entrada e saída deve ser mapeada para um campo de cliente potencial do Marketo Engage.
- Confirme se os campos de saída são atualizáveis. Campos somente leitura e campos de membros do programa não são compatíveis.

## Como usar {#how-to-use}

1. Em Meu Marketo, clique no bloco **[!UICONTROL CX Enterprise Coworker para Marketo Engage]**.

1. Selecione **[!UICONTROL Agentes chamáveis]** na navegação à esquerda. A lista mostra o nome, a data de criação, o criador e o status de cada agente. Pesquisar por nome ou classificar por nome ou data de criação.

1. Selecione **[!UICONTROL Criar agente chamável]**. Escolha um modelo ou deixe o seletor de modelos vazio para começar do zero.

1. Insira um **[!UICONTROL Nome do agente]** e escreva **[!UICONTROL instruções do agente]** descrevendo como processar cada cliente potencial.

1. Em **[!UICONTROL Campos de cliente potencial a serem enviados]**, adicione os campos de cliente potencial de que o agente precisa como entradas. Em **[!UICONTROL Campos de cliente potencial a serem atualizados]**, adicione cada valor que o agente deve retornar e mapeie-o para um campo de cliente potencial atualizável.

1. Selecione **[!UICONTROL Salvar]** para salvar um rascunho ou **[!UICONTROL Salvar e publicar]** para disponibilizar o agente no Marketo Engage.

1. Abra uma Campanha Inteligente e selecione a guia **[!UICONTROL Fluxo]**. Na seção Marketing da lista de etapas de fluxo, localize o **Agente de chamada: _[Nome do agente]_**&#x200B;e arraste-o para o fluxo.

1. Teste a campanha com um pequeno conjunto de clientes em potencial. Revise o log de atividades e confirme se os campos de saída foram atualizados conforme esperado antes de ativar a campanha para todos os clientes potenciais.

## Itens a serem observados {#things-to-note}

- Um agente chamável processa cada lead independentemente. O Marketo Engage envia os valores de lead mapeados para o agente, grava os valores retornados nos campos de lead mapeados e continua para a próxima etapa da campanha.
- Você cria e gerencia agentes chamáveis no CX Enterprise Coworker para Marketo Engage. Nenhuma conexão externa é necessária.
- Os agentes publicados não são editáveis. Para alterar um agente já publicado, crie um novo agente e atualize as Campanhas inteligentes relevantes.

## Criar um agente {#create-an-agent}

### Criar um agente do zero {#create-an-agent-from-scratch}

Deixe o seletor de modelo vazio. O formulário começa com um campo de entrada vazio e um campo de saída vazio. Insira o nome e as instruções e configure os campos de entrada e saída para corresponder à sua regra de negócios.

### Iniciar com base em um modelo {#start-from-a-template}

Escolha um modelo para preencher previamente as instruções, os campos de entrada e os campos de saída. O agente é salvo como sua própria cópia, que pode ser editada ou excluída. Se você excluir um agente criado a partir de um modelo, o modelo ficará disponível no seletor novamente.

| Modelo | Finalidade | Entradas | Saídas |
| --- | --- | --- | --- |
| Normalizador do nome da empresa | Limpa os nomes de empresas removendo sufixos legais, corrigindo erros comuns de digitação e aplicando a capitalização padrão da marca. | Empresa | Empresa normalizada (texto); confiança (número) |
| Formatador E.164 de telefone | Formata números de telefone para o padrão internacional E.164. | Telefone | Telefone normalizado (texto); confiança (número) |
| Padronização do Cargo | Padroniza os cargos e deriva a antiguidade. | Título | Título normalizado (texto); antiguidade (nível C, vice-presidente, diretor, gerente, indivíduo ou desconhecido); confiança |
| Detector de spam e bot | Sinaliza envios de formulário de bot ou spam. | Email, Nome, Sobrenome, Empresa, Telefone | É bot (true/false); confiança; razão; sinalizadores (separados por vírgula) |
| Detector de email descartável | Identifica endereços de email temporários ou descartáveis. | Email | É bot (verdadeiro/falso); confiança; motivo; tipo de email (descartável, pessoal ou comercial) |
| Classificador de lead | Segmentos lideram por tamanho da empresa, setor, persona e intenção. | Empresa, Cargo, Email, Funcionários, Receita | Segmento (Enterprise, Mid-Market, SMB, Startup ou Unknown); setor; persona; nível de intenção (High, Medium ou Low); confiança |
| Enriquecimento de chumbo | Infere detalhes de lead ausentes das informações disponíveis. | Email, Cargo, Empresa | Empresa inferida, departamento, antiguidade, é tomador de decisão (verdadeiro/falso), é B2B (verdadeiro/falso), confiança |
| Pesquisa da empresa | Gera inteligência de vendas a partir de informações da empresa. | Empresa, Site, Descrição | Consulte o modelo para obter a lista completa |

### Escrever instruções eficazes {#write-effective-instructions}

- Coloque regras gerais e exemplos nas instruções do agente. Use as instruções de campo para especificar expectativas para uma saída individual.
- Seja específico. Por exemplo, &quot;Remover sufixos legais como Inc, LLC e Corp&quot; é mais claro do que &quot;limpar nomes de empresas&quot;.
- Inclua exemplos de entradas e saídas esperadas, especialmente para casos de borda.
- Informe o que o agente deve retornar quando não puder decidir, como &quot;Se não tiver certeza, retorne o valor original&quot;.
- Adicione uma saída de confiança para que a lógica da campanha possa direcionar resultados de baixa confiança para revisão.
- Mantenha os prompts concisos. Solicitações mais curtas são executadas mais rapidamente e custam menos.

## Salvar, publicar e gerenciar agentes {#save-publish-and-manage-agents}

### Salvar como rascunho ou publicar {#save-as-a-draft-or-publish}

Selecione **[!UICONTROL Salvar]** para salvar o agente como rascunho. Os rascunhos podem ser editados, mas não estão disponíveis como etapas de fluxo do Smart Campaign. Selecione **[!UICONTROL Salvar e publicar]** quando o agente estiver pronto. O Marketo Engage disponibiliza o agente como uma etapa de fluxo e retorna você à lista de agentes com uma confirmação de publicação. Selecione **[!UICONTROL Cancelar]** para sair sem salvar.

| Status | Significado | Ação disponível |
| --- | --- | --- |
| Rascunho | O agente é salvo, mas não está disponível no Marketo Engage. | Edite-o e selecione **[!UICONTROL Salvar e publicar]** quando estiver pronto. |
| Publicado | O agente está disponível em Campanhas inteligentes. Os agentes publicados estão congelados. | Use o agente publicado ou crie um novo agente para fazer alterações. |
| Falha na publicação | O Marketo Engage rejeitou o agente, por exemplo, porque um nome de campo de saída é reservado. Mas o agente ainda é salvo como um rascunho. | Edite o agente, corrija o campo chamado na mensagem e publique novamente. |

### Editar, verificar uso ou excluir {#edit-check-usage-or-delete}

- Selecione **[!UICONTROL Editar]** em um rascunho para alterá-lo. **[!UICONTROL Salvar]** mantém você na página e mostra uma confirmação de &quot;Agente salvo&quot;. Você também pode selecionar **[!UICONTROL Salvar e publicar]**, **[!UICONTROL Cancelar]** ou **[!UICONTROL Excluir]**.
- Os agentes publicados estão congelados porque as Campanhas inteligentes podem depender deles. Crie um novo agente para fazer alterações.
- Verifique **[!UICONTROL Usado por]** para ver quais Campanhas inteligentes fazem referência a um agente antes de excluir um agente ou alterar sua configuração de campanha.
- Não é possível excluir um agente enquanto uma Campanha inteligente ainda o utilizar. Remova a etapa de fluxo do agente de cada campanha listada e exclua o agente.

## Integração de regras organizacionais {#organizational-rules-integration}

### Nomeação de convenções {#naming-conventions}

- **Nome do agente:** 1-100 caracteres e exclusivo na assinatura. O nome também é usado na etapa de fluxo do Campaign inteligente. Escolha um nome reconhecível, como `Company Name Normalizer`.
- **Nome do campo de saída:** Use letras, dígitos e sublinhados. O nome deve começar com uma letra ou um sublinhado, ser exclusivo e não pode ter mais de 64 caracteres.
- **Nomes reservados:** alguns nomes de saída estão reservados para uso do sistema. Se um nome for rejeitado, escolha outro nome, como `qualificationReason` em vez de `reason`.

### Elementos obrigatórios e campos compatíveis {#required-elements-and-supported-fields}

- Mapeie cada campo de entrada para um campo de cliente potencial do Marketo Engage antes de salvar.
- Configure pelo menos um campo de saída. Mapear cada saída para um campo de cliente potencial atualizável; campos somente leitura não estão disponíveis no seletor de campos.
- Os campos de membro do programa não são compatíveis. O seletor de campos mostra apenas campos de cliente potencial.
- Os tipos de saída suportados são **Texto**, **Número** e **Verdadeiro/Falso**.
- Para retornar uma lista, use um valor de texto separado por vírgulas e descreva o formato esperado nas instruções do campo.
- Cada execução bem-sucedida retorna exatamente os campos de saída configurados.

### Limites {#limits}

| Configuração | Limite |
| --- | --- |
| Nome do agente | 1-100 caracteres; exclusivo na assinatura |
| Instruções do agente | 1-4.000 caracteres |
| Campos de entrada | Até 20; cada um deve ser mapeado para um campo de cliente potencial |
| Campos de saída | 1-20; cada um deve mapear para um campo de lead atualizável |
| Nome do campo de saída | Até 64 caracteres; letras, dígitos e sublinhados; começa com uma letra ou um sublinhado; único |
| Instruções do campo de saída | Até 512 caracteres |
| Clientes potenciais por solicitação | Até 1.000 clientes potenciais do Marketo Engage, processados em paralelo |

## Triagem de conteúdo e manuseio de dados {#content-screening-and-data-handling}

Quando você cria um agente ou edita suas instruções, o Marketo Engage filtra as instruções do agente e as instruções do campo de saída para violações de política, solicitação de injeção e tentativas de exfiltração de dados. Os exemplos incluem solicitações para revelar credenciais ou substituir o comportamento do agente. Se o conteúdo for sinalizado, o salvamento será bloqueado e uma mensagem poderá ser exibida, como &quot;O prompt contém conteúdo restrito&quot; ou &quot;O prompt falhou na moderação de conteúdo&quot;. Revise o texto e salve novamente.

- **O acesso:** o gerenciamento de agentes requer a permissão de **Administrador de acesso**. Os agentes e o histórico de chamadas são isolados por assinatura.
- **Proteção de dados de cliente potencial:** os dados de cliente potencial são transmitidos separadamente das instruções do agente, com proteções que tratam os valores de cliente potencial como dados em vez de comandos.
- **Política de conteúdo:** Se os dados de um cliente potencial violarem a política de conteúdo do provedor de IA, esse cliente potencial receberá uma atividade de erro em vez de um resultado.
- **Retenção:** as cargas de solicitação e resposta, incluindo os valores do campo de cliente potencial enviados ao agente, são mantidas no histórico de chamadas por 30 dias para dar suporte à solução de problemas e, em seguida, são excluídas automaticamente.

## Como os agentes chamáveis são executados em uma campanha {#how-callable-agents-run-in-a-campaign}

1. Quando a campanha é executada, o Marketo Engage envia os valores do campo de lead mapeado para cada lead qualificado para o agente.
1. O agente processa cada lead independentemente e retorna os campos de saída configurados.
1. O Marketo Engage grava os resultados nos campos de clientes potenciais mapeados. Os campos alterados também aparecem como atividades padrão de alteração de valor de dados.
1. A campanha passa para a próxima etapa.

O processamento é assíncrono. A etapa de fluxo aguarda um resultado até a janela de espera da etapa de fluxo no Marketo Engage. Se um lead falhar (por exemplo, devido a um tempo limite), esse lead receberá uma atividade de erro e outros leads continuarão. Cada resultado aparece no registro de atividades do lead para o agente que pode ser chamado.

Use campos de saída na lógica da campanha. Por exemplo, a ramificação em **É bot** para rotear os envios de spam de forma diferente ou ramificação em **confidence** para enviar resultados de baixa confiança para uma etapa de revisão.

## Controle de qualidade da pré-ativação {#pre-activation-qa}

Antes de ativar uma campanha para todos os clientes potenciais:

- Executar a campanha com um pequeno conjunto de testes de clientes potenciais.
- Revise cada log de atividade do lead e confirme se os campos de saída foram atualizados corretamente.
- Casos de borda de teste, incluindo valores ausentes e entradas incomuns.
- Confirme se as ramificações de campanha lidam com valores como baixa confiança ou uma classificação de bot/spam conforme pretendido.

## Casos de uso {#use-cases}

- **Limpeza de dados:** padronize nomes de empresas, formate números de telefone para E.164 e normalize títulos de trabalho quando clientes potenciais forem criados ou importados.
- **Triagem de spam e bot:** verifique se há nomes incorretos, emails suspeitos e números de telefone de dígitos repetidos nos envios; ramifique a campanha com base no resultado.
- **Detecção de email descartável:** Identifique endereços de email temporários e encaminhe-os de forma diferente dos endereços comerciais.
- **Classificação de cliente potencial:** Segmente clientes potenciais por tamanho de empresa, setor, persona e intenção de oferecer suporte a roteamento ou pontuação.
- **Enriquecimento de cliente potencial:** Infira detalhes ausentes, como departamento, antiguidade ou se um cliente potencial é um tomador de decisão.
- **Regras personalizadas:** crie uma verificação ou categorização sim/não que possa ser descrita como uma regra de processamento de cliente potencial, como sinalização de clientes potenciais de uma região ou setor.

## Solução de problemas {#troubleshooting}

| Problema | Resolução |
| --- | --- |
| **Agentes** não aparecem na navegação. | Peça ao administrador do Marketo Engage para conceder a permissão de **Administrador de acesso**. |
| Salvamento bloqueado com uma mensagem de conteúdo. | Revise as instruções do agente ou as instruções do campo para remover o conteúdo sinalizado e salve novamente. |
| O status do agente é **Falha na publicação**. | Edite o agente, corrija o campo nomeado na mensagem e selecione **Salvar e publicar**. |
| Não é possível editar um agente publicado. | Os agentes publicados estão congelados. Crie um novo agente para fazer alterações. |
| Não é possível excluir um agente. | Remova a etapa de fluxo de cada Campanha inteligente listada como usando o agente e, em seguida, exclua-a. |
| Um nome de campo é relatado como reservado. | Escolha um nome de campo de saída diferente, como `qualificationReason`, e salve novamente. |
| Alguns leads recebem uma atividade de erro. | Verifique o log de atividades do lead. Falhas individuais, incluindo tempos limite ou violações de política de conteúdo, não afetam outros leads. |
| Resultados inesperados. | Torne as instruções mais específicas, adicione exemplos, refine as instruções de campo e teste novamente com um pequeno conjunto de leads. |

## Próximas etapas {#next-steps}

- Revise a lista **Usado por** do agente e confirme quais Campanhas inteligentes usarão esse recurso.
- Teste a etapa de fluxo com um pequeno grupo de clientes potenciais e valide os logs de atividade e os campos de saída.
- Use os campos de saída para adicionar ramificações de campanha para classificações ou resultados de baixa confiança.
- Remova a etapa de fluxo do agente de todas as campanhas antes de excluir o agente.
