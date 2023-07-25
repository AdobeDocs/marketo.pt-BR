---
unique-page-id: 37355534
description: Notas de versão - Janeiro de 2020 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Janeiro de 2020
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 1%

---

# Notas de versão: janeiro de 2020 {#release-notes-jan}

Os seguintes recursos estão incluídos na versão de janeiro de 2020. Verifique a edição do Marketo quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela ( ![(estrela)](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

**_Versões trimestrais_**

Os seguintes recursos serão lançados em **17 de janeiro de 2020**.

## Aplicativo de Adobe de Marketo Engage principal {#core-marketo-engage-adobe-application}

* [Seletor de ativos Adobe Experience Manager](/help/marketo/product-docs/adobe-experience-cloud-integrations/importing-assets-with-adobe-experience-manager.md): acesse rapidamente os ativos que se alinham à sua marca com os ativos AEM disponíveis diretamente no Marketo Engage. Observação: embora esse recurso esteja disponível em nossas experiências do Marketo Sky e do Classic, os recursos administrativos podem ser encontrados em nossa experiência do Classic. Você deve ser um cliente do AEM Assets e ter a versão 6.5 ou superior.

>[!NOTE]
>
>Atualmente, o Seletor de ativos de AEM é totalmente compatível apenas com o Firefox. Ele não é compatível com o Safari e pode não funcionar na versão mais recente do Chrome (v. 80), dependendo das configurações de cookie SameSite.

* **Microsoft Dynamics - Sincronizar lead ao CRM em tempo real**: sincronização em tempo real de clientes potenciais e contatos entre o Marketo Engage e o Microsoft Dynamics. Crie clientes potenciais ou contatos e os veja no Microsoft Dynamics imediatamente com a ação de fluxo &quot;Sincronizar pessoa com o Microsoft&quot;.
* **Mapeamento de campos adicionais do linkedIn Lead Gen Forms**: capture dados de clientes potenciais do LinkedIn Lead Gen Forms para criar experiências mais relevantes para pontos de contato de vendas e marketing. Puxe campos ocultos, campos de consentimento e o campo de teste de leads para o Marketo Engage.
* **API de dependências de modelo de email**: obtenha uma lista de ativos que dependem de um modelo de email para entender o escopo de possíveis alterações e as dependências de endereço para modelos que podem ser alteradas e excluídas mais rapidamente.
* **Melhorias no gerenciamento de várias instâncias**: Navegue até a instância necessária rapidamente com um menu suspenso rolável e alfabético de suas assinaturas.

## Marketing baseado em contas {#account-based-marketing}

![(estrela)](assets/yellow-star.png)

* **[Nova descoberta de conta (BETA)](https://docs.marketo.com/x/WQA6Ag) ![(estrela)](assets/yellow-star.png)**: use o Perfil da conta para descobrir novas contas de destino líquidas para sua estratégia ABM com base no modelo de perfil de cliente ideal baseado em IA. Visualize, selecione e importe novas contas recomendadas do, juntamente com seus indicadores de dados de ajuste e intenção baseados em IA, que ainda não existem no banco de dados de clientes potenciais e contas do Marketo Engage para o direcionamento ABM. Imediatamente disponível para qualificar clientes de Criação de perfil de conta.

<br> 

**_Lançamento durante todo o trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Bizible {#bizible}

![(estrela)](assets/yellow-star.png)

* **Integração com o Marketo Engage Leads**: reúna Vendas e Marketing com uma visualização unificada de leads na Bizible e na Marketo Engage. Com esta atualização, o Marketo Engage agora pode ser usado como uma fonte de dados de cliente potencial adicional, para que você não precise mais esperar que os clientes potenciais sincronizem com o CRM para relatar a geração de clientes potenciais.
* **Descubra melhorias**: obtenha mais dos nossos Discover Boards na Bizible com aprimoramentos desenvolvidos a partir do feedback do cliente, como a capacidade de detalhar registros transacionais de blocos e atributos, adicionar contagens de registros essenciais e métricas de custo por custo correspondentes e adicionar/remover filtros de painel para vários painéis. Você também será direcionado diretamente ao painel padrão ao fazer logon.

## Marketo Sky {#marketo-sky}

* [Edição de imagem](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio): Acesse os recursos de edição do Adobe sem precisar sair do Marketo Engage. Essa nova funcionalidade permite que você faça coisas facilmente, como aprimorar, cortar e adicionar texto a imagens diretamente no Design Studio.

## Sales Insight {#sales-insight}

* **Ações em massa do Salesforce Lightning**: aumente a eficiência das vendas e mantenha os compradores envolvidos com a capacidade de adicionar até 200 contatos/leads a campanhas e enviar emails de Marketo Engage em massa com o Salesforce Lightning.
* **Suporte móvel para Salesforce1**: agora você tem acesso móvel em qualquer lugar para todos os recursos do Sales Insight, como Interested Moments e Web Activities &amp; Emails, diretamente no aplicativo Salesforce1.
* **Aprimoramentos na interface**: interface atualizada com aprimoramentos na legibilidade e um design consistente com nossa experiência em Marketo Sky.

## SalesConnect {#sales-connect}

* **Componentes da grade**: otimize sua instância do Sales Connect com novas funcionalidades de personalização de grade. Escolha quais colunas serão exibidas, pesquise por colunas, selecione/desmarque todas as colunas e determine quantas linhas de dados você deseja ver em cada página.
* **[Bloqueio de conteúdo](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)**: maximize o alinhamento da marca com uma configuração em toda a assinatura que controla se os não administradores têm a capacidade de criar e editar modelos e campanhas.

>[!NOTE]
>
>* **Substituição de TLS 1.0 e 1.1**: em um esforço contínuo para integrar com a estrutura de lançamento do Adobe, estamos mudando a desativação do TLS 1.0 e do TLS 1.1 para 13 de janeiro de 2020. Você encontra informações mais detalhadas [aqui](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **Atualização do Munchkin ITP 2.1+**: devido a alterações na política de cookies do Safari, a capacidade do Munchkin de rastrear usuários em sessões no mesmo domínio será limitada pela ITP a 1 ou 7 dias com base no navegador e na versão usada pelo visitante. Para levar em conta isso, estamos implementando um novo serviço da web para permitir que os cookies do Munchkin sejam definidos com um cabeçalho Set-Cookie via resposta HTTP. Mais informações sobre como implementar este novo serviço podem ser encontradas [aqui](https://nation.marketo.com/docs/DOC-7351).

**_Webinário de lançamento do produto_** [Junte-se a nós](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) em 3 de março, às 11h (PT) / 14h (ET) para um webinário ao vivo hospedado por nossa equipe de produtos e saiba mais sobre os recursos incluídos nesta versão.
