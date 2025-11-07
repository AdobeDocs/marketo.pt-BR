---
title: Converter imagens em modelos do HTML
description: Use essa ferramenta sem código para transformar uma imagem em um modelo de email editável.
solution: Marketo Engage
product: marketo
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 74c8b1597bed7e2ac827bea444200dacfe4b29a5
workflow-type: tm+mt
source-wordcount: '1287'
ht-degree: 1%

---

# Converter imagens em modelos do HTML {#image-to-html}

## Visão geral {#overview}

O conversor de imagem para HTML acelera significativamente a criação de emails convertendo imagens estáticas em modelos de conteúdo de email do HTML totalmente personalizáveis e modulares. Essa ferramenta sem código permite transformar designs visuais de designers gráficos ou ferramentas de design em modelos de email responsivos e editáveis que podem ser reutilizados várias vezes.

Aproveitando a tecnologia de IA gerativa, o conversor de imagem para HTML analisa o layout, a tipografia, as cores e os elementos visuais da imagem e gera um código HTML limpo e modular que mantém a fidelidade do design e, ao mesmo tempo, garante total capacidade de edição e compatibilidade com o Designer de email.

>[!PREREQUISITES]
>
>* Primeiro, você deve concordar com os [termos principais da Gen-AI e os termos complementares](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} para usar a funcionalidade da Gen-AI no Designer de email. Entre em contato com a Equipe de conta da Adobe (seu gerente de conta) para obter detalhes.
>* Você deve ter permissões _Acessar Modelo de Email_ e _Editar/Gerar Modelo de Email_ habilitadas [em sua função da Marketo](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#edit-a-role).

## Converter uma imagem {#convert-an-image}

Para converter uma imagem em um modelo de email do HTML totalmente personalizável, siga as etapas abaixo.

>[!NOTE]
>
>Para obter melhores resultados, use imagens de alta qualidade com elementos visuais claros e texto legível. Idealmente, as imagens devem ter entre 600 e 800 pixels de largura para corresponder às dimensões de email padrão.

1. No _Design Studio_, clique em **Modelos de Email** e depois em **Modelos de Email (Novos)**.

   ![](assets/image-to-html-1.png)

1. Clique em **[!UICONTROL Converter imagem em modelo]**.

   ![](assets/image-to-html-2.png)

1. Insira um _Nome do modelo_ e uma descrição opcional. Além disso, opcionalmente, você pode escolher o estilo da marca. Carregue ou arraste e solte a imagem desejada.

   ![](assets/image-to-html-3.png)

1. Role para baixo e marque a caixa de seleção _O arquivo de carregamento não contém..._. Clique em **Converter**.

   ![](assets/image-to-html-4.png)

   >[!NOTE]
   >
   >O processo de geração pode levar até cinco minutos, dependendo da complexidade e do tamanho do design de imagem. O processamento da IA ocorre em segundo plano, para que você possa sair dessa tela e trabalhar em outras tarefas enquanto a conversão estiver em andamento. Talvez seja necessário atualizar a tela de biblioteca _Modelo de email_ para ver a alteração de status.

1. Após a conclusão da conversão, o modelo será salvo automaticamente como rascunho. Clique no nome para exibir/editar.

   ![](assets/image-to-html-5.png)

1. O modelo convertido é aberto no Designer de email com recursos de edição completos. Agora você pode:

   * Editar conteúdo de texto e aplicar personalização
   * Modificar imagens e adicionar links
   * Ajustar cores, fontes e estilo
   * Adicionar, remover ou reorganizar componentes de conteúdo
   * Aproveite todos os recursos do Email Designer como com qualquer outro modelo

   ![](assets/image-to-html-6.png){width="800" zoomable="yes"}

1. É possível fazer os ajustes desejados para refinar o modelo e corresponder às diretrizes da marca.

1. Depois de satisfeito com seu modelo, clique em **[!UICONTROL Salvar e fechar]** e em **Publicar**.

Seu modelo agora está disponível na biblioteca _Modelos de email_ e pode ser usado ao criar emails.

## Casos de uso comuns {#use-cases}

O conversor de imagem para HTML é ideal para:

* **Migração de plataforma**: migrando de outra plataforma de marketing por email? Converter seus designs de email existentes em modelos do HTML prontos para Marketo Engage sem reconstruir do zero
* **Conversão do modelo de design**: transforme modelos de design de ferramentas como Photoshop, Figma ou outro software de design em modelos de email funcionais
* **Criação rápida de modelo**: gere modelos de email rapidamente para campanhas com limite de tempo sem esperar pelos recursos do desenvolvedor
* **Criando bibliotecas de modelos**: crie uma biblioteca abrangente de modelos consistentes com a marca que os membros da equipe não técnica possam personalizar e implantar

## Práticas recomendadas {#best-practices}

**Antes de começar**

* **Salvar conteúdo existente**: a conversão de uma imagem em HTML substituirá todo o conteúdo existente no seu email. Sempre salve o trabalho atual antes de usar este recurso.
* **Planeje seu fluxo de trabalho**: use o conversor de imagem para HTML no início do processo de criação de email ou verifique se você está pronto para substituir todo o conteúdo atual.

**Preparação da imagem**

* **Solução**: use imagens de alta resolução para obter um melhor reconhecimento de texto e detecção de elementos.
* **Clareza**: verifique se o texto é claramente legível e se os elementos visuais estão bem definidos.
* **Largura**: crie imagens nas larguras de email padrão (600-800px) para corresponder aos requisitos típicos do cliente de email.
* **Formato de arquivo**: use o formato JPEG ou PNG; evite imagens compactadas ou de baixa qualidade.
* **Design completo**: incluir o design de email completo em uma única imagem, do cabeçalho ao rodapé.

**Considerações sobre o design**

* **Layouts simples**: layouts simples e bem estruturados são convertidos com mais precisão do que designs altamente complexos.
* **Elementos padrão**: use padrões comuns de design de email (cabeçalho, seções de corpo, CTAs, rodapé).
* **Legibilidade do texto**: garanta contraste suficiente entre o texto e os planos de fundo.
* **Fontes seguras para a Web**: os designs que usam fontes comuns seguras para a Web terão melhor fidelidade.
* **Evitar elementos sobrepostos**: mantenha os elementos de design claramente separados para obter um melhor reconhecimento de estrutura.

**Após a conversão**

* **Analisar rascunho**: depois que a conversão for concluída, o modelo será salvo automaticamente como rascunho. Reserve tempo para analisar cuidadosamente a precisão do HTML gerado.
* **Testar completamente**: teste o email em diferentes clientes e dispositivos de email. Para obter resultados mais rápidos, aproveite a [integração do Litmus](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).
* **Refinar manualmente**: faça os ajustes necessários usando os recursos de edição completos do Designer de email.
* **Alinhamento da marca**: verifique se as cores, as fontes e o estilo correspondem às diretrizes da sua marca.
* **Personalization**: adicione conteúdo dinâmico e tokens de personalização conforme desejado.
* **Acessibilidade**: revise e aprimore os recursos de acessibilidade, se necessário.

## Limitações e considerações {#limitations}

Esteja ciente das seguintes limitações ao usar o conversor de imagem para HTML.

* **Interpretação de IA**: a IA gera o HTML com base em uma interpretação visual da sua imagem. Designs complexos ou incomuns podem exigir ajustes manuais após a conversão.

* **Precisão do texto**: enquanto a IA tenta reconhecer e reproduzir o texto com precisão, sempre verifique o conteúdo do texto e faça as correções necessárias.

* **Conteúdo dinâmico**: o processo de conversão cria um HTML estático com base na sua imagem. Você precisará adicionar personalização, conteúdo dinâmico e rastreamento manualmente após a conversão.

* **Layouts complexos**: projetos altamente complexos com camadas complexas, formas incomuns ou elementos não padrão podem não ser perfeitamente convertidos. Designs mais simples geralmente produzem melhores resultados.

* **Tempo de processamento**: o processo de conversão pode levar até cinco minutos, dependendo da complexidade e do tamanho da sua imagem. O processamento da IA acontece em segundo plano, permitindo que você trabalhe em outras tarefas sem manter a tela aberta. O modelo é salvo automaticamente como um rascunho após a conclusão da conversão.

>[!NOTE]
>
>O conversor de imagem para HTML foi projetado para fornecer um forte ponto de partida para a criação de emails. O HTML gerado deve ser revisado e refinado usando o Designer de email para garantir que atenda aos seus requisitos.

## Perguntas frequentes {#faq}

+++O que acontece com meu conteúdo de email existente quando uso o conversor de imagem para HTML?

Todo o conteúdo existente no seu email será excluído e substituído pelo modelo recém-gerado ao fazer upload de uma imagem para conversão. Salve qualquer conteúdo importante antes de usar este recurso. É melhor usar o conversor de imagem para HTML no início do processo de criação de email.

+++

+++Quais formatos de arquivo são compatíveis?

O conversor de imagem para HTML é compatível com os formatos de imagem JPEG (.jpg, .jpeg) e PNG (.png).

+++

+++Quanto tempo leva o processo de conversão?

A conversão pode levar até cinco minutos, dependendo da complexidade e do tamanho do design de imagem. O processamento da IA acontece em segundo plano, para que você possa sair e trabalhar em outras tarefas; não é necessário manter a tela aberta. Após a conclusão da conversão, o arquivo será salvo automaticamente como rascunho para que você o revise e edite.

+++

+++Posso editar o modelo gerado?

Sim! O modelo de HTML gerado é aberto no Designer de email com recursos de edição completos. É possível modificar todos os aspectos do modelo, incluindo texto, imagens, estilo, layout e estrutura.

+++

+++O que acontece se a conversão não corresponder exatamente ao meu design?

A IA faz o melhor para interpretar com precisão o design, mas pode ser necessário refinar manualmente. Use o Designer de email para ajustar todos os elementos que precisam de ajuste.

+++

+++Posso usar esse recurso para páginas de aterrissagem ou outros tipos de conteúdo?

Atualmente, o conversor de imagem para HTML é projetado especificamente para modelos de email. Para outros tipos de conteúdo, use as opções padrão de design e importação disponíveis no Designer de email.

+++

+++É possível reutilizar modelos convertidos em várias campanhas de email?

Sim! Os modelos criados com o conversor de imagem para HTML são salvos automaticamente na biblioteca _Modelos de email_. Você pode acessá-las e reutilizá-las em qualquer email a partir de agora.

+++
