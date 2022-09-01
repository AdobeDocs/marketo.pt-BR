---
unique-page-id: 6848747
description: Descrições de permissões de função - Documentos do Marketo - Documentação do produto
title: Descrições das permissões de função
exl-id: 00963cd9-2d53-455f-bc6f-42a573468ff9
source-git-commit: 1f5a6ab994ccb81ff32f39ac32eef6a37aeab192
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 19%

---

# Descrições das permissões de função {#descriptions-of-role-permissions}

Abaixo está uma lista de todas as permissões disponíveis que você pode atribuir às suas funções. As permissões geralmente são associadas a áreas funcionais específicas dentro do Marketo e podem ajudar você a controlar a quais áreas e funcionalidades diferentes os usuários têm acesso.

Algumas informações adicionais sobre permissões:

* A permissão de &quot;Acesso&quot; dá permissão de função para visualizar e, às vezes, editar essa parte do aplicativo.
* Para que uma função tenha acesso às subpermissões (&quot;Criar&quot;, &quot;Excluir&quot; etc.), ela deve ter permissão de &quot;Acesso&quot; para essa parte do aplicativo. Por exemplo, se você quiser dar a alguém permissão para Editar campanhas, elas devem ter permissão geral para acessar atividades de marketing.
* É possível ver ações ou ativos que você não tem permissão para usar. No entanto, se você tentar acessá-los, verá uma mensagem avisando sobre seu acesso limitado.

## Permissões disponíveis {#available-permissions}

Quando você [criar ou editar uma função](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), é possível selecionar qual das seguintes permissões permitir essa função, marcando as caixas apropriadas.

![](assets/createnewrole.png)

## Acessar administrador  {#access-admin}

Exiba e faça alterações nas configurações na seção Minha conta de Administração.

* Trilha de auditoria de acesso - concede aos usuários acesso à trilha de auditoria de ativos e à trilha de auditoria de administração
* Canais de acesso - concede aos usuários acesso somente para modificar a tag do Canal, não outras tags personalizadas
* Limite de comunicação de acesso - Fornece aos usuários acesso para ativar um limite de comunicação em Administração
* Acesso ao CRM - concede aos usuários acesso ao CRM, como Salesforce ou Microsoft Dynamics, em Administração
* Acesso [Data.com](https://Data.com) - Concede aos usuários acesso à ação de fluxo Data.com
* Acessar administrador de email - concede usuários ao administrador de email para alterar configurações padrão, como cancelar a assinatura e domínios de marca
* Acessar parceiros de evento - concede aos usuários acesso ao LaunchPoint em Admin
* Gerenciamento de campo de acesso - concede aos usuários acesso ao Gerenciamento de campo na Administração
* Acessar upload de arquivo - Oferece aos usuários a capacidade de carregar imagens e arquivos no Design Studio
* Acessar páginas de aterrissagem - Fornece aos usuários acesso às páginas de aterrissagem no Administrador
* Local de acesso - concede aos usuários acesso ao local na Administração para definir o idioma padrão, a localidade, o fuso horário e a moeda
* Histórico de logon de acesso - concede aos usuários acesso ao histórico de logon do usuário na trilha de auditoria
* Configurações de logon de acesso - concede aos usuários acesso às Configurações de logon em Administração para configurações de Segurança, Restrições de IP e Relatório de lista inteligente
* Acesse a atividade personalizada do Marketo - concede aos usuários acesso às atividades personalizadas do Marketo em Administração
* Acessar objeto personalizado do Marketo - concede aos usuários acesso aos objetos personalizados do Marketo em Administração
* Access Munchkin - O GIveicula aos usuários acesso ao Munchkin no Admin, para definir o código de rastreamento, o rastreamento de pessoas e ativar a configuração da API
* Acesse a Análise do ciclo de receita - concede aos usuários acesso à Análise do ciclo de receita em Administração, para definir o Resumo e a atribuição de sincronização
* Funções de acesso - concede aos usuários acesso para gerenciar e editar funções, mas não aos usuários
* Acessar insight de vendas - concede aos usuários acesso para gerenciar Insight de vendas em Administração, para definir status, configuração de API, Pontuação de pessoas e outras configurações
* Acesso ao Logon único - Fornece aos usuários acesso para gerenciar o Logon Único no Admin, para ativar o SAML e trabalhar com configurações do SAML e URLs de Página de Redirecionamento
* Acessar o Smart Campaign - concede aos usuários acesso ao Smart Campaign na Administração, para restringir os limites em pessoas qualificadas
* Acessar API SOAP - Fornece aos usuários acesso para gerenciar APIs SOAP em Serviços da Web em Administração
* Tags de acesso - concede aos usuários acesso a todas as tags personalizadas, exceto à tag de Canal
* Access Treasure Chest - Concede aos usuários acesso aos recursos experimentais no Treasure Chest na Admin
* Acessar usuários - concede aos usuários acesso para editar e gerenciar usuários (mas não funções) no Administrador
* Acessar Webhooks - Oferece usuários aos Webhooks no Admin, para definir detalhes e mapeamentos de resposta
* Acessar espaços de trabalho e partições - Concede aos usuários acesso para criar, editar e excluir espaços de trabalho e partições em Administração

## API de acesso  {#access-api}

Oferece aos usuários o **Somente API** **Função** acesso às APIs individuais listadas abaixo.

* Aprovar ativos
* Executar campanha
* Atividade somente de leitura
* Metadados de atividade somente de leitura
* Ativos somente de leitura
* Campanha somente de leitura
* Empresa somente de leitura
* Objeto personalizado somente de leitura
* Pessoa somente leitura
* Conta nomeada somente de leitura
* Oportunidade somente de leitura
* Pessoa de vendas somente de leitura
* Atividade de leitura-gravação
* Metadados de atividade de leitura e gravação
* Ativos de leitura-gravação
* Campanha de leitura-gravação
* Empresa de leitura-gravação
* Objeto personalizado de leitura-gravação
* Pessoa com leitura/gravação
* Conta nomeada de leitura e gravação
* Oportunidade de leitura-gravação
* Pessoa de vendas de leitura-gravação

## Acessar análises {#access-analytics}

Fornece aos usuários acesso às guias do Analytics, aos Insights de email, aos relatórios e aos três itens abaixo, a menos que estejam desmarcados.

* Acesse o Explorador de Receita - Desmarcar remove o acesso do usuário ao Explorador de Receita
* Excluir relatório - Desmarcar remove a capacidade do usuário de excluir relatórios
* Exportar dados do Analytics - A desverificação remove a capacidade do usuário de exportar dados do Analytics

## Acessar apresentações de calendários {#access-calendar-presentations}

Concede aos usuários acesso às Apresentações do calendário - permite a exibição do botão Presentations na parte inferior.

* Editar Presentations do Calendário - Permite que os usuários editem apresentações no Calendário

## Acessar Estúdio de desenvolvimento {#access-design-studio}

Fornece aos usuários acesso à guia Design Studio e à visualização da árvore, mas não aos detalhes.

* Acessar e-mail
   * Editar email - Concede aos usuários permissão para editar, criar e clonar emails
      * Tornar o email operacional - Concede aos usuários permissão para tornar o email operacional. Consulte: [Tornar um email operacional](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * Aprovar email - Permite que os usuários aprovem emails.
      * Excluir email - permite que os usuários excluam emails.
      * Definir domínio de marca - Permite que os usuários trabalhem com domínios de marca. Consulte: [Adicionar um domínio de marca adicional](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

* Acessar modelo de e-mail

   * Aprovar modelo de e-mail
   * Excluir modelo de e-mail
   * Editar modelo de email - Editar, criar e clonar modelos de email

* Acessar formulário

   * Aprovar formulário
   * Excluir formulário
   * Editar formulário - Editar, criar e clonar formulários

* Acessar imagem

   * Excluir imagem
   * Carregar imagem

* Acessar página

   * Aprovar página
   * Excluir página
   * Editar página de aterrissagem - Editar, criar e clonar páginas de aterrissagem

* Acessar modelo de página

   * Aprovar modelo de página
   * Excluir modelo de página
   * Editar modelo de página de aterrissagem - Editar, criar e clonar modelos de página de aterrissagem

* Acessar bloco de conteúdo

   * Aprovar bloco de conteúdo
   * Excluir bloco de conteúdo
   * Editar bloco de conteúdo

* Acessar aplicativo social

   * Aprovar aplicativo social
   * Excluir aplicativo social
   * Editar aplicativo social

## Acessar banco de dados {#access-database}

Visualize o banco de dados, bem como visualize e edite listas inteligentes/estáticas.

* Acessar segmentação

   * Aprovar segmentação
   * Excluir segmentação
   * Editar segmentação

* Excluir pessoa
* Excluir lista
* Editar Pessoa - Impede a edição manual e a execução de etapas de fluxo único; você ainda pode editar pessoas executando campanhas contra elas
* Exportar Pessoa - Exporte planilhas com a a partir de suas listas de bancos de dados
* Importar objeto personalizado
* Importar lista
* Mesclar pessoas
* Executar ações de fluxo único - Permite que os usuários executem **Alterar valor de dados** etapa de fluxo em pessoas do banco de dados

* Exibir dados da oportunidade - oculta as informações da oportunidade na página de detalhes da pessoa

## Acessar atividades de marketing {#access-marketing-activities}

Exiba a guia Marketing Activities , as campanhas e as pastas de campanha.

* Acessar mensagem de SMS

   * Aprovar mensagem de SMS
   * Excluir mensagem de SMS
   * Editar mensagem de SMS

* Acessar notificação por push

   * Aprovar notificação por push
   * Excluir notificação por push
   * Editar notificação por push

* Acessar prêmios
* Ativar campanha com gatilho
* Aprovar programa de e-mail
* Clonar ativo de marketing
* Excluir ativo de marketing
* Editar restrições de campanha
* Editar ativo de marketing
* Importar programa
* Importação de lista
* Programar campanha em lote

Acessar SEO

* Administrar SEO
* SEO padrão

## Direcionamento e personalização {#targeting-and-personalization}

* Administrar personalização na Web
* Editor de campanhas de CRE
* Iniciador de campanhas de CRE
* Editor de campanhas on-line
* Iniciador de campanhas on-line

Administração da área de trabalho

* Acesso de administrador para um espaço de trabalho específico (somente se você tiver espaços de trabalho ativados)
* Mover ativos entre espaços de trabalho (somente se você tiver espaços de trabalho ativados)
