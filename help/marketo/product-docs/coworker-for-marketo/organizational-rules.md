---
description: Descrição aqui.
title: Regras organizacionais
source-git-commit: 0949e5193333d56943a5c9a52c1715ecbcb274f3
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%
---
# Regras organizacionais {#organizational-rules}

As Regras organizacionais definem seus padrões de operações de marketing e requisitos de governança em um único documento que orienta o Colaborador na criação de programas, no planejamento de campanhas e nos workflows de validação.

## O que são Regras Organizacionais? {#what-are-organizational-rules}

As Regras organizacionais são um documento de configuração baseado em marcação que captura os padrões de campanha de sua organização:

* Convenções de nomenclatura para programas, emails e campanhas inteligentes
* Ativos e estrutura necessários (pastas, tokens, relatórios)
* Requisitos de conformidade (links para cancelar inscrição, parâmetros UTM, filtros de exclusão)
* Práticas recomendadas (design de email, configuração de lista inteligente)

Cada instância do Marketo inclui Regras organizacionais padrão. Você pode personalizá-los para refletir as necessidades de governança específicas de sua organização.

## Onde as Regras Organizacionais são usadas {#where-organizational-rules-are-used}

As regras organizacionais orientam o colaborador em três habilidades:

| Habilidade | Como as regras são aplicadas |
| --- | --- |
| Criar programas | As regras orientam a criação da estrutura do programa, o nome e a configuração inicial. O colaborador sinaliza quaisquer problemas de conformidade em seu resumo antes de criar o programa. |
| Planejar campanhas | As regras informam como o Colaborador estrutura campanhas inteligentes, filtros e etapas de fluxo com base em seus padrões. |
| Validar Programas | As regras definem o que o Colaborador verifica ao validar programas antes da ativação. |

## Como acessar e personalizar regras organizacionais {#how-to-access-and-customize-organizational-rules}

1. Em Meu Marketo, clique no bloco **Colaborador do Marketo Engage**.
1. Clique no ícone de engrenagem.
1. Selecione a guia **Regras Organizacionais**.
1. Revise as regras padrão (elas vêm pré-preenchidas com práticas recomendadas de operações de marketing).
1. Edite as regras de acordo com as de sua organização:

   * Convenções de nomenclatura (programas, emails, campanhas)
   * Estrutura de pasta necessária
   * Tokens e campos obrigatórios
   * Padrões de conformidade e exclusão

1. Atualize o número da versão ao fazer alterações.
1. Salve as alterações. Todas as habilidades de colegas de trabalho usarão suas regras personalizadas imediatamente.

## Estrutura de regras organizacionais {#organizational-rules-structure}

As Regras organizacionais são formatadas no markdown com o YAML frontmatter:

```markdown
---
name: Your Organization Name — Marketo Campaign Governance
version: 1.0
enabled: true
customized: true
---

# Naming Conventions

## Programs
- Pattern: {{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}
- Example: AMER_FY25_Q2_WBR_250315_Product_Launch_Webinar
- Region codes: AMER, EMEA, APAC, GLOBAL

## Emails
- Pattern: {{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}
- Example: Product_Launch_01_Invitation

# Program Structure

## Required Local Folders
- 01 Emails
- 02 Smart Campaigns
- 03 Reports

## Required Tokens
- {{my.eventDate}}
- {{my.replyToEmail}}

# Email Compliance

## ⚠️ REQUIRED Elements
- Unsubscribe link in footer
- Company name and physical address
- All external links include UTM parameters

## Recommended Elements
- Alt text on all images
- Mobile-responsive design (600px max-width)
```

## Práticas recomendadas para Regras organizacionais {#best-practices-for-organizational-rules}

* **Iniciar com padrões**: examine as regras padrão antes de personalizar. Elas refletem as práticas recomendadas do setor para operações de marketing.
* **Manter regras focalizadas**: inclua apenas os requisitos que são importantes para sua organização. Regras desnecessárias criam ruídos e reduzem pontuações de conformidade desnecessariamente.
* **Usar verificações automáticas e manuais**:

  * Verificações automatizadas — convenções de nomenclatura, pastas necessárias, uso de token (o Co-worker pode verificá-las)
  * Verificações manuais — design visual de email, conformidade com a marca, lógica de campanha (o parceiro sinalizará isso como etapas de revisão manual)

* **Restrição de equilíbrio com flexibilidade**: regras muito estritas podem retardar a criação de programas. Regras muito dispersas não detectam problemas importantes de conformidade.
* **Versão de suas regras**: atualize o número da versão ao fazer alterações significativas para que sua equipe saiba que os padrões de governança foram atualizados.
* **Comunicar alterações**: ao atualizar as Regras organizacionais, informe à sua equipe de operações de marketing o que mudou e o porquê.

## O que o Colaborador pode ou não validar {#what-coworker-can-and-cannot-validate}

O colaborador PODE validar (verificações automatizadas):

* As convenções de nomenclatura correspondem aos seus padrões
* A estrutura de pasta necessária existe
* Os tokens necessários estão em vigor
* O email tem links para cancelar a inscrição e elementos de rodapé necessários
* Os links externos incluem parâmetros UTM
* Nomes de campanha inteligentes seguem convenções

O colaborador NÃO PODE validar (revisão manual necessária):

* Lógica de filtro de lista inteligente (limitação de API — é necessário configurar filtros manualmente)
* Lógica de etapa do fluxo de campanha inteligente (limitação de API — é necessário configurar fluxos manualmente)
* Renderização visual de email e capacidade de resposta (requer inspeção visual)
* Conformidade da marca e tom de mensagem (requer julgamento humano)
* Regras de segmentação de conteúdo dinâmico (limitação de API)

Quando o Colaborador encontra algo que não pode validar, ele a sinaliza como uma etapa de revisão manual no fluxo de trabalho.

## Pontuação de conformidade {#compliance-scoring}

Quando você usa Validar Programas, o Colaborador calcula uma pontuação de conformidade com base em:

* **Verificações aprovadas** — O colega verificou a conformidade e não encontrou problemas
* **Verificações com falha** — Colaborador encontrou violações de suas Regras Organizacionais
* **Etapas de revisão manual** — Itens que exigem verificação humana (eles NÃO contam para a sua pontuação)

Um programa pode ter 100% de conformidade e ainda exigir etapas de revisão manual — elas são excluídas do cálculo de pontuação.

## Exemplos de personalização de Regras Organizacionais {#examples-of-organizational-rules-customization}

**Exemplo 1: convenção de nomenclatura estrita**

```markdown
## Programs
Pattern: {{COUNTRY}}-{{BUSINESS_UNIT}}-{{CAMPAIGN_TYPE}}-FY{{YEAR}}-{{QUARTER}}-{{DATE}}
```

Use-a se sua organização exigir governança rigorosa em todas as regiões e unidades de negócios.

**Exemplo 2: nomenclatura flexível com o prefixo obrigatório**

```markdown
## Programs
Pattern: {{PREFIX}}_* (where PREFIX = EMEA, AMER, APAC, GLOBAL)
Example: AMER_Q2_Product_Launch_Webinar_2025
```

Use isso se desejar consistência nos códigos de região, mas flexibilidade no restante.

**Exemplo 3: regras mínimas (foco na conformidade)**

```markdown
# Email Compliance — REQUIRED

- Unsubscribe link present
- CAN-SPAM physical address in footer
- Reply-to email configured
```

Use-a se sua organização priorizar a conformidade em relação à consistência de nomenclatura/estrutura.

## Solução de problemas {#troubleshooting}

**P: atualizei as Regras Organizacionais, mas o Colaborador ainda está usando as regras antigas.**

R: As alterações entram em vigor imediatamente para novos programas e validações. Se estiver trabalhando em um programa existente, atualize o navegador ou inicie um novo fluxo de trabalho de Colaborador para ver as regras atualizadas.

**P: Posso reverter para as regras padrão?**

R: Sim. Vá para **Configurações** > **Regras Organizacionais** e clique em **Redefinir para o Padrão**. Suas regras personalizadas serão substituídas pelas regras padrão.

**P: Minha pontuação de conformidade é baixa, mesmo que o programa pareça bom.**

R: Verifique quais verificações estão falhando. Analise suas Regras organizacionais para ver se são muito rigorosas para seus fluxos de trabalho atuais ou se você precisa ajustar o programa para atender aos seus padrões.
