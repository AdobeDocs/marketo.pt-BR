---
description: O programa Clone duplica um programa Marketo existente em uma nova pasta com um novo nome, preservando sua estrutura e permitindo personalizar a nova campanha.
title: Clonar programa
badge: Beta
hide: true
source-git-commit: 1e70b9383bf3a1cd30715df4379d440c4efb1abd
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Clonar programa {#clone-program}

O agente do programa Clone copia um programa de trabalho, incluindo campanhas inteligentes, etapas de fluxo, ativos de email e configuração, em um novo local no ambiente do Marketo.

>[!PREREQUISITES]
>
>* Para usar esse recurso, primeiro você deve concordar com os [termos principais da Gen-AI e os termos complementares](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Entre em contato com a Equipe de conta da Adobe (seu gerente de conta) para obter detalhes.
>
>* Você deve ter permissão para criar programas na pasta de destino.
>
>* O programa de origem que você deseja clonar já deve existir em seu ambiente do Marketo.

>[!AVAILABILITY]
>
>No momento, esse recurso está na versão beta fechada. Não divulgue esta documentação.

## Como usar {#how-to-use}

1. Em Meu Marketo, clique no bloco **IA do Marketo**.
1. Na janela do prompt, digite as instruções. Por exemplo, &quot;Clone meu programa de webinário do segundo trimestre na pasta Campanhas do terceiro trimestre e chame-o de webinário de demonstração de produto do terceiro trimestre&quot;.
1. A Marketo AI confirma o programa de origem, a pasta de destino e o novo nome. Revise e confirme.
1. O clone é criado. A IA do Marketo confirma quando está concluída e informa onde encontrá-la.
1. Abra o novo programa no Marketo e atualize o que é diferente: conteúdo de email, datas, filtros de público-alvo, tokens etc.
1. Execute o agente [Controle de qualidade do programa](/help/marketo/product-docs/marketo-ai/skills/validate-programs.md) antes de ativar.

## Casos de uso {#use-cases}

**Reutilização da campanha trimestral**: um gerente de campanha executa a mesma série de webinários a cada trimestre. Eles solicitam à Marketo AI que clone o programa de webinário do trimestre passado na pasta do trimestre novo com um nome atualizado. Em seguida, eles atualizam a cópia do email, os tokens de data do webinário e o link de registro, economizando horas de tempo de configuração.

**Criação de um modelo a partir de um programa comprovado**: um especialista em operações de marketing clona um programa de lançamento de produto de alto desempenho em uma pasta &quot;Modelos&quot; para servir como ponto de partida para inicializações futuras. O clone é deixado desativado e usado como uma cópia de referência.

**Teste A/B de uma nova abordagem**: um gerente de campanha deseja testar uma cadência de email diferente sem alterar um programa em execução. Eles clonam o programa ativo, modificam as etapas de espera no clone e ativam ambos, executando-os em diferentes segmentos de público-alvo para comparar resultados.

## Itens a serem observados {#things-to-note}

* Os programas clonados são criados em um estado desativado. Nada é publicado até que você ative as campanhas inteligentes.
* Os ativos de email no clone são cópias, não compartilhadas com o original. As alterações nos emails do clone não afetarão o programa de origem.
* Os tokens usados no programa de origem são copiados para o clone. No entanto, eles ainda devem ser atualizados com novos valores (datas, URLs, nomes de eventos).
* Os filtros de campanha inteligente no clone fazem referência às mesmas listas e campos que os originais. Revise e atualize o direcionamento de público-alvo antes de ativar.
* Os ativos locais que fazem referência a outros programas ou listas compartilhadas são copiados para o clone. Essas referências devem ser revisadas antes da ativação.
