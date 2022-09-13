---
description: Notas de versão atuais - Documentação do Marketo - Documentação do produto
title: Notas de versão atuais
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: d26428137e9b99d04fef67a3b21b74d150f693e7
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Notas de versão: Outubro de 2022 {#release-notes-oct-22}

Abaixo você encontrará todos os recursos incluídos na versão de 22 de outubro. Verifique sua edição do Adobe Marketo Engage para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

Os seguintes recursos começarão a ser lançados em **14 de outubro de 2022**, com uma distribuição em fases dos recursos restantes durante as semanas subsequentes (salvo indicação em contrário). Os recursos da versão e as datas exatas estão sujeitos a alterações.

## Orquestração entre canais {#cross-channel-orchestration}

* **Organizar automaticamente fluxos de diálogo para bate-papo dinâmico**: Melhore sua tela de diálogo lotada organizando tudo na tela em um formato limpo e fácil de ler com a impressão de um botão por meio da Auto Arrange.

* **Suporte a tipos de dados adicionais para o Dynamic Chat**: Três novos tipos de dados (booleano, inteiro, flutuante) permitem aproveitar mais campos de Marketo Engage existentes no Dynamic Chat para coisas como direcionamento com base em pontuações ou fazer perguntas de sim/não aos visitantes.

* **Links de reunião para bate-papo dinâmico**: Opção para incluir automaticamente um link de Equipes ou Encontrar para Google e Outlook em cada convite de calendário enviado para visitantes.

* **Notificações de reunião agendadas para bate-papo dinâmico**: Representantes de vendas recebem notificações por email automatizadas sobre reuniões programadas, bem como quaisquer informações relevantes sobre a interação do chatbot do visitante.

* **Funções e permissões para o bate-papo dinâmico**: Os administradores podem usar permissões granulares para controlar a visibilidade e o uso do aplicativo e criar funções de usuário personalizadas.

   * Acesso completo - os usuários podem aproveitar ao máximo o recurso (por exemplo, caixas de diálogo de publicação, alteração do esquema de cores etc.)
   * Acesso somente leitura - os usuários podem ver informações, mas não podem fazer alterações (por exemplo, consulte Critérios de público-alvo ou Designer de fluxo, mas não alterar)
   * Acesso restrito - os usuários não podem ver ou acessar as seções Configuração ou Integrações

## Experiência da próxima geração {#next-generation-experience}

* **Telas atualizadas na experiência de próxima geração**: Estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração que oferecem melhorias atualizadas de design e usabilidade acessíveis por meio do switch de alternância:

   * Detalhes do modelo da página de aterrissagem
   * Lista de modelos de email

* **Aprimorado usado por guia em Detalhes do modelo de email**: Na nova experiência, você verá informações adicionais relacionadas aos ativos usando o modelo de email, incluindo Status do ativo, Última modificação e Última modificação por. Também é possível pesquisar, classificar e filtrar a lista de ativos usados por ativos.

* **Modos de Filtro de Ativo de Relatório**: Novo design para modais de configuração de relatório que exibem uma nova árvore de ativos no menu de configuração e um filtro para Data de criação e modificação.

## Ambiente de dados de marketing {#marketing-data-environment}

* **Integração do Adobe Privacy Service**: Faça a harmonização com o Privacy Service para automatizar a conformidade com as regulamentações de privacidade de dados em produtos de Experience Cloud. No momento, esse serviço está disponível somente para clientes do Marketo Engage que se conectaram ao [Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md)Sistema {target=&quot;_blank&quot;}.

* **Sincronização de Campos Personalizados do Membro do Programa**: Capacidade de sincronizar bidirecionalmente campos extensíveis capturados para um membro do programa (por exemplo, preferências do participante durante o registro do evento, como comida, sessões, faixas etc.)

## Melhorias da API {#api-enhancements}

* **Importação de leads em massa: Associação de Vendedores**: Paridade com a API REST de lead para poder associar leads com vendedores durante o processo de importação de lead em massa, reduzindo a complexidade e o número de chamadas de API necessárias.

## Anúncios {#announcements}

* **Forms 1.0**: A desativação do Forms 1.0 será concluída com a versão de outubro. Os ativos do Forms 1.0 não poderão mais enviar dados para o Marketo Engage e retornarão erros se tentarem.

* **Forms sem script**: O Forms não funcionará mais quando o Javascript estiver desativado no navegador. O envio de formulário exigirá a ativação do Javascript.
