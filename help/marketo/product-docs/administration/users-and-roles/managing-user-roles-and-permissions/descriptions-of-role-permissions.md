---
unique-page-id: 6848747
description: Descrições de permissões de função - Documentos do Marketo - Documentação do produto
title: Descrições das permissões de função
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---


# Descrições de permissões de função {#descriptions-of-role-permissions}

Abaixo está uma lista de todas as permissões disponíveis que você pode atribuir às suas funções. As permissões geralmente são associadas a áreas funcionais específicas dentro do Marketo e podem ajudar você a controlar quais áreas e funcionalidades diferentes os usuários têm acesso.

Algumas informações adicionais sobre permissões:

* A permissão de &quot;Acesso&quot; dá permissão de função para visualizar e, às vezes, editar essa parte do aplicativo.
* Para que uma função tenha acesso às subpermissões (&quot;Criar&quot;, &quot;Excluir&quot; etc.), ela deve ter permissão de &quot;Acesso&quot; para essa parte do aplicativo. Por exemplo, se você quiser dar a alguém permissão para Editar campanhas, elas devem ter permissão geral para acessar atividades de marketing.
* É possível ver ações ou ativos que você não tem permissão para usar. No entanto, se você tentar acessá-los, verá uma mensagem avisando sobre seu acesso limitado.

## Permissões disponíveis {#available-permissions}

Ao [criar ou editar uma função](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md), você pode selecionar qual das seguintes permissões permitir essa função marcando as caixas apropriadas.

![](assets/createnewrole.png)

## Administrador de acesso {#access-admin}

Exiba e faça alterações nas configurações na seção Minha conta de Administração.

* Trilha de auditoria de acesso - concede aos usuários acesso à trilha de auditoria de ativos e à trilha de auditoria de administração
* Canais de acesso - concede aos usuários acesso somente para modificar a tag do Canal, não outras tags personalizadas
* Limite de comunicação de acesso - Fornece aos usuários acesso para ativar um limite de comunicação em Administração
* Access CRM - concede aos usuários acesso ao CRM, como Salesforce ou Microsoft Dynamics, em Administração
* Acesse [Data.com](https://Data.com) - Concede aos usuários acesso à ação de fluxo Data.com
* Acessar administrador de email - concede usuários ao administrador de email para alterar configurações padrão, como cancelar a assinatura e domínios de marca
* Acessar parceiros de evento - concede aos usuários acesso ao LaunchPoint em Admin
* Gerenciamento de campo de acesso - concede aos usuários acesso ao Gerenciamento de campo na Administração
* Acessar upload de arquivo - Oferece aos usuários a capacidade de carregar imagens e arquivos no Design Studio
* Acessar páginas de aterrissagem - Fornece aos usuários acesso às páginas de aterrissagem no Administrador
* Local de acesso - concede aos usuários acesso ao local na Administração para definir o idioma padrão, a localidade, o fuso horário e a moeda
* Histórico de logon de acesso - concede aos usuários acesso ao histórico de logon do usuário na trilha de auditoria
* Configurações de logon de acesso - concede aos usuários acesso às Configurações de logon em Administração para configurações de Segurança, Restrições de IP e Relatório de lista inteligente
* Acesso à atividade personalizada do Marketo - concede aos usuários acesso às atividades personalizadas do Marketo na administração
* Acessar objeto personalizado do Marketo - concede aos usuários acesso aos objetos personalizados do Marketo na Administração
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

## API de acesso {#access-api}

Fornece aos usuários com a **API Somente** **Função** acesso às APIs individuais listadas abaixo.

* Aprovar ativos
* Executar campanha
* Atividade somente leitura
* Metadados de atividade somente leitura
* Ativos somente leitura
* Campanha somente leitura
* Empresa somente leitura
* Objeto Personalizado Somente Leitura
* Pessoa Somente Leitura
* Conta Nomeada Somente Leitura
* Oportunidade somente leitura
* Pessoa de Vendas Somente Leitura
* Atividade de leitura e gravação
* Metadados de atividade de leitura e gravação
* Ativos de leitura e gravação
* Campanha de leitura-gravação
* Empresa de leitura e gravação
* Objeto personalizado de leitura e gravação
* Pessoa de Leitura-Escrita
* Conta Nomeada de Leitura-Gravação
* Oportunidade de Leitura e Gravação
* Pessoa de Vendas de Leitura e Gravação

## Acessar o Analytics {#access-analytics}

Fornece aos usuários acesso às guias do Analytics, aos Insights de email, aos relatórios e aos três itens abaixo, a menos que estejam desmarcados.

* Acesse o Explorador de Receita - Desmarcar remove o acesso do usuário ao Explorador de Receita
* Excluir relatório - Desmarcar remove a capacidade do usuário de excluir relatórios
* Exportar dados do Analytics - A desverificação remove a capacidade do usuário de exportar dados do Analytics

## Acessar apresentações de calendário {#access-calendar-presentations}

Concede aos usuários acesso às Apresentações do calendário - ativa a exibição do botão Apresentações na parte inferior.

* Editar Apresentações do Calendário - Permite que os usuários editem apresentações no Calendário

## Acesse o Design Studio {#access-design-studio}

Fornece aos usuários acesso à guia Design Studio e à visualização da árvore, mas não aos detalhes.

* Acessar Email
   * Editar email - Concede aos usuários permissão para editar, criar e clonar emails
      * Tornar o email operacional - Concede aos usuários permissão para tornar o email operacional. Consulte: [Tornar um Email Operacional](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)

      * Aprovar email - Permite que os usuários aprovem emails.
      * Excluir email - permite que os usuários excluam emails.
      * Definir domínio de marca - Permite que os usuários trabalhem com domínios de marca. Consulte: [Adicionar um Domínio de Marca Adicional](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/add-an-additional-branding-domain.md)

* Acessar modelo de email

   * Aprovar modelo de email
   * Excluir modelo de email
   * Editar modelo de email - Editar, criar e clonar modelos de email

* Formulário de acesso

   * Excluir formulário
   * Editar formulário - Editar, criar e clonar formulários

* Acessar imagem

   * Excluir imagem
   * Carregar imagem

* Acessar página de aterrissagem

   * Aprovar página de aterrissagem
   * Excluir página de aterrissagem
   * Editar página de aterrissagem - Editar, criar e clonar páginas de aterrissagem

* Acessar modelo de página inicial

   * Aprovar modelo de página inicial
   * Excluir modelo de página inicial
   * Editar modelo de página de aterrissagem - Editar, criar e clonar modelos de página de aterrissagem

* Snippet de acesso

   * Aprovar trecho
   * Excluir trecho
   * Editar trecho

* Acessar o aplicativo social

   * Aprovar aplicativo social
   * Excluir aplicativo social
   * Editar aplicativo social

## Acessar Banco de Dados {#access-database}

Visualize o banco de dados, bem como visualize e edite listas inteligentes/estáticas.

* Segmentação de acesso

   * Aprovar segmentação
   * Excluir segmentação
   * Editar segmentação

* Importação de lista avançada
* Excluir pessoa
* Excluir lista
* Editar Pessoa - Impede a edição manual e a execução de etapas de fluxo único; você ainda pode editar pessoas executando campanhas contra elas
* Exportar Pessoa - Exporte planilhas com a a partir de suas listas de bancos de dados
* Importar objeto personalizado
* Importar Lista
* Unir Pessoas
* Executar ações de fluxo único - Permite que os usuários executem a etapa de fluxo **Alterar valor de dados** em pessoas do banco de dados

* Exibir dados da oportunidade - oculta as informações da oportunidade na página de detalhes da pessoa

## Acesse as atividades de marketing {#access-marketing-activities}

Exiba a guia Marketing Activities , as campanhas e as pastas de campanha.

* Acessar mensagem SMS

   * Aprovar mensagem SMS
   * Excluir mensagem SMS
   * Editar mensagem SMS

* Acessar notificações por push

   * Aprovar notificação por push
   * Excluir notificação por push
   * Editar notificação por push

* Prêmios de acesso
* Ativar campanha do acionador
* Aprovar programa de email
* Clone o ativo de marketing
* Excluir ativo de marketing
* Editar restrições de campanha
* Editar ativo de marketing
* Programa de importação
* Importar lista
* Programar campanha em lote

Acessar SEO

* Administrar SEO
* SEO padrão

## Direcionamento e personalização {#targeting-and-personalization}

* Administrar personalização da Web
* Editor de Campanha CRE
* CRE Campaign Launcher
* Editor de Campanha Web
* Iniciador de campanha da Web

Administração do Workspace

* Acesso de administrador para um espaço de trabalho específico (somente se você tiver espaços de trabalho ativados)
* Mover ativos entre espaços de trabalho (somente se você tiver espaços de trabalho ativados)
