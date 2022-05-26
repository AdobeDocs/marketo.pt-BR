---
description: Notas de versão atuais - Documentação do Marketo - Documentação do produto
title: Notas de versão atuais
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: f7bb22572ed1a79fe8afe4a1066a2cc172a43f23
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# Notas de versão: Junho de 2022 {#release-notes-june-22}

Abaixo você encontrará todos os recursos incluídos na versão de 22 de junho. Verifique sua edição do Adobe Marketo Engage para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

Os seguintes recursos começarão a ser lançados em **24 de junho de 2022**, com uma distribuição em fases dos recursos restantes durante as semanas subsequentes (salvo indicação em contrário).

## Ambiente de dados de marketing {#marketing-data-environment}

* **Expor os campos CreatedAt/UpdatedAt para objetos personalizados**: Oferece a capacidade de inspecionar esses campos na tela Detalhes da pessoa para obter informações adicionais.

## Orquestração entre canais {#cross-channel-orchestration}

* **Usabilidade do Stream Designer aprimorada para o Dynamic Chat**: Adicione cartões diretamente da tela do Stream Designer sem a necessidade de arrastar e soltar. A interface do Dynamic Chat também foi aprimorada para oferecer melhor visibilidade do conteúdo em cartões individuais.

* **Regras avançadas de roteamento de compromisso para bate-papo dinâmico**: O Dynamic Chat oferece mais opções para roteamento de compromissos direcionado. Especifique quais compromissos de agente devem ser roteados com base em atributos de Marketo Engage, garantindo que os leads sejam roteados para os agentes apropriados.

* **Relatório da caixa de diálogo avançada para bate-papo dinâmico**: Visualize o desempenho de suas campanhas do Dynamic Chat com mais detalhes usando visualizações de dados totalmente novas para métricas de envolvimento e conversão.

* **Atributos de Marketo Engage não sincronizados não utilizados para o bate-papo dinâmico**: Atributos Marketo Engage não sincronizados da sua assinatura do Dynamic Chat que não são utilizados, ajudando você a facilitar a limpeza dos dados e permitindo que atributos alternativos sejam sincronizados conforme necessário.

## Automação de experiência {#experience-automation}

* **Exclusões de regra de validação do campo de formulário global**: Exclua formulários específicos das Regras de validação de formulário global para que os centros de assinatura e outros fluxos de trabalho comerciais críticos possam aceitar todos os valores.

* **Etapas do fluxo de autoatendimento**: Expanda a conectividade entre o Marketo Engage e o resto da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas inteligentes. Os usuários e parceiros do Marketo Engage podem aproveitar essa funcionalidade para permitir o uso de serviços da Web externos em Acionador, Lote e Campanhas Executáveis, em contraste com Webhooks, que só podem ser usados em Campanhas do Acionador.

* **Rastreamento de link agnóstico do protocolo Munchkin**: Estender suporte para rastrear `tel` e `mailto` links com o Munchkin para rastrear um conjunto expandido de comportamentos da Web.

* **Métodos HTTP adicionais para webhooks**: Especifique PUT, PATCH e DELETE como tipos de solicitação para interagir com serviços da Web.

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **Permissão de insight de vendas definida no Salesforce**: Os administradores podem fornecer acesso ao Sales Insight a um conjunto limitado de pessoas em um nível de usuário, em vez de no nível de perfil, por meio do conjunto de permissões do aplicativo Marketo, que faz parte do pacote Sales Insight Salesforce .

* **Minha atualização do mosaico da Marketo - Ações de insight de vendas**: Agora, os administradores do Marketo (e os usuários designados por eles) podem navegar rapidamente para a instância de ações de insight de vendas por meio de um novo bloco de ações de insight de vendas , localizado na página Meu Marketo .

## SalesConnect {#sales-connect}

* **Atualização da API do Salesforce**: Com a versão do Salesforce Verão de 222, as versões herdadas da API 21-30 não serão mais suportadas pelo Salesforce. Com esta versão do Marketo Engage, todas as solicitações de Conexão de Vendas usando versões de API herdadas foram atualizadas para permanecer em uma versão suportada. Para obter detalhes completos sobre os planos de aposentadoria da API do Salesforce, clique em [here](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target=&quot;_blank&quot;}.

## Melhorias da API {#api-enhancements}

* **Novos recursos de filtragem para a API de extração de membro do programa em massa**: Filtre por status de associação ao programa, atualizadoEm, cadência ou conteúdo esgotado para refinar o conjunto de dados extraído.

* **Aprimoramento da API de extração de membro do programa em massa**: Especifique até 10 programas durante a criação de emprego para melhorar a taxa de transferência.

## Anúncios {#announcements}

* **Substituição do Forms - Forms 1.0, ponto de extremidade de Captura/salvamento do lead e versões sem script de formulários**: O suporte para ativos do Forms 1.0 será completamente removido do Marketo Engage. Todos os ativos existentes do Forms 1.0 não funcionarão. Os formulários Marketo Engage exigirão que o JavaScript seja carregado nas páginas de aterrissagem e nos sites.

**_Webinar da versão do produto_**

Junte-se a nós em 24 de agosto de 2022, às 9:00 PT / 12:00 PM ET para um [webinário ao vivo](https://engage.marketo.com/2022_June_August_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} hospedado pela nossa equipe de produtos, onde você pode aprender a usar todas as inovações de produtos mais recentes.
