---
unique-page-id: 6848747
description: Descrições de permissões de função - Documentos de marketing - Documentação do produto
title: Descrições de permissões de função
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '1154'
ht-degree: 0%

---


# Descrições de permissões de função {#descriptions-of-role-permissions}

Abaixo está uma lista de todas as permissões disponíveis que você pode atribuir às suas funções. As permissões são geralmente associadas a áreas funcionais específicas dentro do Marketo e podem ajudá-lo a controlar as áreas e funcionalidades às quais os diferentes usuários têm acesso.

Algumas informações adicionais sobre permissões:

* A permissão &quot;Acesso&quot; concede uma permissão de função para a visualização e, às vezes, edita essa parte do aplicativo.
* Para que uma função tenha acesso às subpermissões (&quot;Criar&quot;, &quot;Excluir&quot; etc.), essa função deve ter permissão de &quot;Acesso&quot; para essa parte do aplicativo. Por exemplo, se você quiser conceder a alguém permissão para Editar Campanhas, eles deverão ter permissão geral para acessar Atividades de marketing.
* Você pode ver ações ou ativos que não têm permissão para usar. No entanto, se tentar acessá-los, você verá uma mensagem avisando sobre seu acesso limitado.

## Permissões disponíveis {#available-permissions}

Ao [criar ou editar uma função](../../../../product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), você pode selecionar qual das seguintes permissões permite essa função marcando as caixas apropriadas.

![](assets/createnewrole.png)

## Administrador de acesso  {#access-admin}

Visualização e faça alterações nas configurações na seção Minha conta de Administrador.

* Trilha de auditoria de acesso - concede aos usuários acesso à Trilha de auditoria de ativos e à Trilha de auditoria de administração
* Canais de acesso - concede aos usuários acesso somente para modificar a tag do Canal, não outras tags personalizadas
* Limite de comunicação de acesso - concede aos usuários acesso para habilitar um limite de comunicação em Administrador
* Access CRM - concede aos usuários acesso ao CRM, como Salesforce ou Microsoft Dynamics, em Admin
* Access [Data.com](http://Data.com) - concede aos usuários acesso à ação de fluxo Data.com
* Access Email Admin - Concede aos usuários o Administrador de email para alterar as configurações padrão, como cancelar a assinatura e domínios de marca
* Parceiros de Evento de acesso - concede aos usuários acesso ao LaunchPoint em Admin
* Gerenciamento de campo de acesso - concede aos usuários acesso ao Gerenciamento de campo na Administração
* Carregamento de arquivo de acesso - concede aos usuários a capacidade de carregar imagens e arquivos no Design Studio
* Landings page de acesso - concede aos usuários acesso às Landings page em Administração
* Local de acesso - concede aos usuários acesso ao Local na Administração para configurar o idioma padrão, a localidade, o fuso horário e a moeda
* Histórico de logon de acesso - concede aos usuários acesso ao Histórico de logon de usuário no Trilho de auditoria
* Configurações de logon de acesso - concede aos usuários acesso às Configurações de logon em Admin para configurações de segurança, restrições de IP e Relatório de Lista inteligente
* Acesso à Atividade personalizada de marketing - concede aos usuários acesso a Atividades personalizadas de marketing em Admin
* Acessar objeto personalizado de marketing - concede aos usuários acesso a objetos personalizados de marketing em Admin
* Access Munchkin - os usuários do GI acessam Munchkin em Admin, para configurar o código de rastreamento, o rastreamento de pessoas e a configuração da API
* Access Revenue Cycle Analytics - Concede aos usuários acesso ao Revenue Cycle Analytics em Admin, para definir Sync Summary (Resumo da sincronização) e Attribution
* Funções de acesso - concede aos usuários acesso para gerenciar e editar funções, mas não aos usuários
* Acessar o insight de vendas - concede aos usuários acesso para gerenciar o insight de vendas em Admin, para definir o status, a configuração da API, a pontuação da pessoa e outras configurações
* Acesso ao logon único - concede aos usuários acesso para gerenciar o logon único em Admin, para habilitar o SAML e trabalhar com configurações SAML e URLs de página de redirecionamento
* Campanha inteligente de acesso - concede aos usuários acesso à Campanha inteligente em Administração, para restringir os limites em pessoas qualificadas
* API SOAP de acesso - concede aos usuários acesso para gerenciar APIs SOAP em serviços da Web em Administração
* Tags de acesso - concede aos usuários acesso a todas as tags personalizadas, exceto à tag do Canal
* Access Treasure Chest - Concede aos usuários acesso aos recursos experimentais no Treasure Chest na Admin
* Acessar usuários - concede aos usuários acesso para editar e gerenciar usuários (mas não funções) em Administração
* Acessar webhooks - concede usuários a webhooks em Admin, para configurar detalhes e mapeamentos de resposta
* Acessar espaços de trabalho e partições - concede aos usuários acesso para criar, editar e excluir espaços de trabalho e partições em Administração

## API de acesso  {#access-api}

Fornece aos usuários com a **API Acesso Somente** **função** às APIs individuais listadas abaixo.

* Aprovar ativos
* Campanha Execute
* Atividade somente leitura
* Metadados de Atividade somente leitura
* Ativos somente leitura
* Campanha somente leitura
* Empresa somente leitura
* Objeto personalizado somente leitura
* Pessoa somente leitura
* Conta nomeada Somente Leitura
* Oportunidade somente leitura
* Pessoa de Vendas Somente Leitura
* Atividade de leitura e gravação
* Metadados de Atividade de leitura e gravação
* Ativos de leitura e gravação
* Campanha de leitura e gravação
* Empresa de leitura e gravação
* Objeto personalizado de leitura e gravação
* Pessoa de leitura e gravação
* Conta nomeada Leitura-Gravação
* Oportunidade de Leitura-Gravação
* Pessoa de vendas de leitura/gravação

Análise de acesso

Concede aos usuários acesso às guias do Analytics, aos Insights de email, aos relatórios e aos três itens abaixo, a menos que estejam desmarcados.

* Acesse o Explorador de Receita - Desmarcar remove o acesso do usuário ao Gerenciador de Receita
* Excluir relatório - Desmarcar remove a capacidade do usuário de excluir relatórios
* Exportar dados do Analytics - A desverificação remove a capacidade do usuário de exportar dados do Analytics

## Acesse o calendário Presentations {#access-calendar-presentations}

Dá aos usuários acesso às apresentações do calendário?- permite a exibição do botão Presentations na parte inferior?

* Editar calendário Presentations - permite que os usuários editem apresentações no calendário

## Access Design Studio {#access-design-studio}

Fornece aos usuários acesso à guia Design Studio e à visualização da árvore, mas não aos detalhes.

* Acessar email

   * Editar email - concede aos usuários permissão para editar, criar e clonar emails

      * Tornar o email operacional - Concede aos usuários permissão para tornar o email operacional. Consulte: [Tornar um email operacional](../../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)
   * Aprovar email - permite que os usuários aprovem emails.
   * Excluir email - permite que os usuários excluam emails.
   * Definir domínio de marca - permite que os usuários trabalhem com domínios de marca. Consulte: [Adicionar vários domínios de marca](http://docs.marketo.com/display/docs/add+multiple+branding+domains)


* Acessar modelo de email

   * Aprovar modelo de e-mail
   * Excluir modelo de email
   * Editar modelo de e-mail - Editar, criar e clonar modelos de e-mail

* Formulário de acesso

   * Excluir formulário
   * Editar formulário - Editar, criar e clonar formulários

* Acessar imagem

   * Excluir imagem
   * Carregar imagem

* Landing page de acesso

   * Aprovar Landing page
   * Excluir Landing page
   * Editar Landing page - Editar, criar e clonar landings page

* Modelo de Landing page de acesso

   * Aprovar modelo de Landing page
   * Excluir modelo de Landing page
   * Editar modelo de Landing page - Editar, criar e clonar modelos de landing page

* Trecho de acesso

   * Aprovar trecho
   * Excluir trecho
   * Editar trecho

* Acessar o aplicativo social

   * Aprovar aplicativo social
   * Excluir aplicativo social
   * Editar aplicativo social

## Banco de Dados de Acesso {#access-database}

Visualização o banco de dados e visualização e edite listas inteligentes/estáticas.

* Segmentação de acesso

   * Aprovar segmentação
   * Excluir segmentação
   * Editar segmentação

* Importação avançada de Listas
* Excluir Pessoa
* Excluir Lista
* Editar pessoa - impede a edição manual e a execução de etapas de fluxo único; você ainda pode editar pessoas executando campanhas contra elas
* Exportar Pessoa - Exportar planilhas com do seu banco de dados listas
* Importar objeto personalizado
* Importar Lista
* Unir pessoas
* Executar ações de fluxo único - permite que os usuários executem a etapa de fluxo **Alterar valor** de dados em pessoas do banco de dados

* Dados da oportunidade de visualização - Oculta as informações da oportunidade na página de detalhes da pessoa

## Atividades de marketing de acesso {#access-marketing-activities}

Visualização na guia Atividades de marketing, campanhas e pastas de campanha.

* Acessar Mensagem SMS

   * Aprovar mensagem SMS
   * Excluir Mensagem SMS
   * Editar Mensagem SMS

* Notificação por push de acesso

   * Aprovar notificação por push
   * Excluir notificação por push
   * Editar notificação por push

* Prêmios Access
* Ativar Campanha do acionador
* Aprovar Programa de e-mail
* Clonar ativo de marketing
* Excluir ativo de marketing
* Editar restrições de Campanha
* Editar ativo de marketing
* Importar Programa
* Importação de lista
* Agendar Campanha em lote

Acessar SEO

* Administrar SEO
* SEO padrão

## Direcionamento e personalização {#targeting-and-personalization}

* Administrar personalização da Web
* Editor de Campanhas CRE
* Iniciador de Campanhas CRE
* Editor de Campanhas da Web
* Iniciador de Campanhas da Web

Administração do espaço de trabalho

* Acesso de administrador para um espaço de trabalho específico (somente se você tiver espaços de trabalho ativados)
* Mover ativos entre espaços de trabalho (somente se você tiver espaços de trabalho ativados)

Acessar aplicativo móvel
