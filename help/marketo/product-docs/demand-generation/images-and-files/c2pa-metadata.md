---
description: Saiba como os metadados do C2PA são anexados automaticamente a imagens geradas por IA no Marketo Engage, preservados por meio de edições e usados para a origem do conteúdo.
title: Metadados C2PA no Marketo Engage
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 77c4c0b6438f8a5070fd33412b7037b79f7fded1
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 2%

---

# Metadados C2PA no Marketo Engage

Novas leis estão surgindo em torno da transparência generativa da IA, e a Adobe está trabalhando para atender aos requisitos aplicáveis em todas as jurisdições. Os metadados C2PA são a ferramenta de origem que o Adobe usa para atender aos requisitos dessas leis.

Os metadados C2PA são metadados duráveis e invisíveis que registram como um conteúdo foi criado ou editado. Ao gerar ou editar uma imagem com ferramentas de IA gerativas no Marketo Engage, os metadados do C2PA são anexados automaticamente a essa imagem (nenhuma ação é necessária de sua parte). São informações criptografadas e invioláveis que podem ajudar os visualizadores a entender a linhagem do conteúdo e garantir a integridade dos ativos da marca. Essas informações incluem:

* **Emissor ou Assinante**: informações sobre a entidade ou empresa que emitiu a assinatura digital para certificar ou assinar o ativo.
* **Data de Emissão**: a data em que os metadados C2PA foram aplicados ao ativo.
* **Crédito e Uso**: Informações sobre o produtor do ativo, incluindo nome, identificadores de mídia social ou outras informações relacionadas à identidade.
* **Processo**: registros de edições ou modificações feitas no ativo.
* **Detalhes do dispositivo**: informações sobre o aplicativo ou dispositivo usado para criar ou editar o ativo.
* **Ferramenta de IA usada**: se uma IA gerativa tiver sido usada para criar o ativo, o nome do modelo usado poderá ser incluído.
* **Outras Informações Pertinentes**: dados adicionais também estão incluídos para ajudar a oferecer mais contexto sobre o histórico de um ativo.

## Ações que anexam metadados C2PA

A tabela a seguir resume quando os metadados C2PA são anexados, com base na ação de imagem executada na geração da imagem no Marketo Engage.

| Ação | Descrição | Metadados C2PA anexados? | Exemplo de caso de uso |
|---|---|---|---|
| **Usar a ferramenta &#39;Gerar imagem&#39;** | Crie uma nova imagem a partir de um prompt de texto, de uma imagem de referência ou gere uma imagem semelhante. | Sempre. A imagem é gerada por IA gerativa, de modo que sempre transporta metadados C2PA novos. | Uma imagem de banner para uma campanha de email é gerada a partir de um prompt de texto que descreve o visual desejado. |
| **Cortar uma imagem** | Ajuste uma imagem para as dimensões solicitadas. | Somente se a imagem de origem já tiver metadados C2PA. O corte recria os pixels da imagem, o que normalmente apagaria esses metadados do C2PA. Portanto, o Marketo Engage os lê da imagem de origem antes de cortar e, em seguida, os recria e anexa novamente ao resultado cortado. O corte em si não adiciona uma nova ação de IA gerativa; ele preserva a existente. | Uma imagem de banner gerada é cortada para caber em uma página da Web: os metadados C2PA são preservados por meio do corte. Uma foto do stock carregada usada como um plano de fundo de notificação por push é cortada para caber na tela: como a foto do stock não carrega nenhuma ação de IA gerativa, nenhum metadado C2PA é criado. |
| **Adicionar uma sobreposição de texto** | Renderiza o texto gerado sobre uma imagem de plano de fundo. | Somente se a imagem de fundo já tiver metadados C2PA. A renderização da sobreposição produz uma nova imagem do plano de fundo mais o texto, o que normalmente apagaria esses metadados do C2PA. Portanto, o Marketo Engage os lê da imagem do plano de fundo com antecedência, depois os reconstrói e os reanexa ao resultado. A etapa de sobreposição não adiciona uma nova ação de IA gerativa. | Um título promocional é renderizado como uma sobreposição de texto em uma imagem de fundo gerada para uma landing page: os metadados C2PA da imagem de fundo são preservados. |

## Tipos de conteúdo e seu escopo

**Imagens**: Cobertas. Os metadados C2PA são anexados quando as imagens são geradas com IA gerativa e preservados por meio de operações de recorte e sobreposição de texto executadas pela geração de imagens no Marketo Engage.

**Texto**: não aplicável. As saídas somente texto da geração de imagem no Marketo Engage, como geração de cópia, tradução e sugestões de alinhamento de marca, não exigem metadados C2PA.

## O que acontece quando o conteúdo se move

O Marketo Engage preserva os metadados C2PA associados aos ativos de imagem compatíveis. Se uma imagem contiver metadados C2PA quando importados para o Marketo Engage, os metadados serão retidos quando o ativo for usado no conteúdo da campanha gerado e em experiências de email de saída.

## Recursos adicionais

* [Diretrizes do usuário da IA gerada da Adobe Experience Cloud](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* [Medidas de proteção e limitações](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer/using/content-management/generate-content/gs-generative#generative-guardrails)
