---
unique-page-id: 37355534
description: Notas de versão - Janeiro de 2020 - Documentação da Marketo - Documentação do produto
title: Notas de versão - Janeiro de 2020
exl-id: 7b011c1a-1161-42f8-8bd0-4ee273928b59
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 1%

---

# Notas de versão: Jan 2020 {#release-notes-jan}

Os seguintes recursos estão incluídos na versão de 20 de janeiro. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela ( ![(star)](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestrais_**

Os seguintes recursos serão lançados em **17 de janeiro de 2020**.

## Aplicativo Marketo Engage Adobe Core {#core-marketo-engage-adobe-application}

* [Seletor](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/importing-assets-with-adobe-experience-manager.md) de ativos Adobe Experience Manager: Acesse rapidamente os ativos que se alinham à sua marca com AEM ativos disponíveis diretamente no Marketo Engage. Observação: Embora esse recurso esteja disponível em nossas experiências de Marketo Sky e clássica, os recursos administrativos podem ser encontrados em nossa experiência do Classic. Você deve ser um cliente do AEM Assets e ter a versão 6.5 ou superior.

>[!NOTE]
>
>Atualmente, AEM Seletor de ativos é totalmente compatível apenas com o Firefox. Ele não é compatível com o Safari e pode não funcionar na versão mais recente do Chrome (v. 80), dependendo das configurações de cookie do SameSite.

* **Microsoft Dynamics - Sincronizar lead para o CRM em tempo** real: Sincronização de leads em tempo real e contatos entre o Marketo Engage e o Microsoft Dynamics. Crie leads ou contatos e os veja no Microsoft Dynamics imediatamente com a ação de fluxo &quot;Sincronizar pessoa com a Microsoft&quot;.
* **Mapeamento** de campo adicional Forms da geração de leads do linkedIn: Capture dados de clientes potenciais do LinkedIn Lead Gen Forms para criar experiências mais relevantes para pontos de contato de vendas e marketing. Puxe campos ocultos, campos de consentimento e o campo de lead do teste para o Marketo Engage.
* **API** de dependências do modelo de email: Obtenha uma lista de ativos que dependem de um modelo de email para entender o escopo de possíveis alterações e as dependências de endereço para modelos podem ser alteradas e excluídas mais rapidamente.
* **Melhorias** no gerenciamento de várias instâncias: Navegue até a instância de que você precisa rapidamente com um menu suspenso rolável e alfabético de suas assinaturas.

## Marketing baseado em contas {#account-based-marketing}

![(estrela)](assets/yellow-star.png)

* **[Nova descoberta de conta (BETA)](https://docs.marketo.com/x/WQA6Ag) ![ (estrela)](assets/yellow-star.png)**: Use a Criação de perfil de conta para descobrir novas contas-alvo para sua estratégia de ABM com base em seu modelo de perfil de cliente ideal alimentado por IA. Exiba, selecione e importe novas contas recomendadas, juntamente com seus indicadores de dados de ajuste e intenção baseados em IA, que ainda não existem no banco de dados de cliente potencial e conta do Marketo Engage para direcionamento por ABM. Imediatamente disponível para clientes qualificados de Criação de perfis de conta.

<br> 

**_Lançamento em todo o trimestre_**

Os seguintes recursos estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Bizible {#bizible}

![(estrela)](assets/yellow-star.png)

* **Integração** de clientes potenciais do Marketo Engage: Reúna vendas e marketing junto com uma visão unificada de clientes potenciais em Bizible e Marketo Engage. Com essa atualização, o Marketo Engage agora pode ser usado como uma fonte de dados de lead adicional, de modo que não é mais necessário aguardar a sincronização dos leads com o CRM para gerar relatórios sobre a geração de leads.
* **Melhorias** do Discover: Obtenha mais de nossos Fóruns do Discover na Bizible com melhorias desenvolvidas a partir do feedback dos clientes, como a capacidade de analisar registros transacionais de blocos e atributos, adicionar contagens de registro essenciais e métricas de custo por correspondentes e adicionar/remover filtros de painel para vários painéis. Você também será direcionado ao painel padrão ao fazer logon.

## Marketo Sky {#marketo-sky}

* [Edição](https://experienceleague.adobe.com/docs/marketo/sky/design-studio/marketo-image-editor.html?lang=en#design-studio) de imagem: Acesse os recursos de edição do Adobe sem precisar sair do Marketo Engage. Essa nova funcionalidade permite que você faça coisas como aprimorar, recortar e adicionar texto a imagens diretamente no Design Studio.

## Sales Insight {#sales-insight}

* **Ações** em massa do Salesforce Lightning: Aumente a eficiência das vendas e mantenha os compradores envolvidos com a capacidade de adicionar até 200 contatos/leads a campanhas e enviar emails de Marketo Engage em massa com o Salesforce Lightning.
* **Suporte móvel para Salesforce1**: Agora você tem acesso móvel para todos os recursos de informações de vendas, como Momentos interessantes e Atividades da Web e Emails, diretamente no aplicativo Salesforce1.
* **Aprimoramentos** da interface do usuário: Atualização da interface com aprimoramentos à legibilidade e um design consistente com nossa experiência em Marketo Sky.

## SalesConnect {#sales-connect}

* **Componentes** de grade: Otimize sua instância de Conexão de Vendas com novas funcionalidades de personalização de grade. Escolha quais colunas exibir, pesquise por colunas, selecione/desmarque todas as colunas e determine quantas linhas de dados você deseja visualizar em cada página.
* **[Bloqueio](/help/marketo/product-docs/marketo-sales-connect/admin/content-lockdown.md)** de conteúdo: Maximize o alinhamento da marca com uma configuração de toda a assinatura que controla se os não administradores têm a capacidade de criar e editar modelos e campanhas.

>[!NOTE]
>
>* **Substituição** de TLS 1.0 e 1.1: Em um esforço contínuo de integração com a transferência da estrutura do Adobe, estamos descontinuando o TLS 1.0 e o TLS 1.1 para 13 de janeiro de 2020. Você encontra informações mais detalhadas [aqui](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).
>
>* **Atualização** do ITP 2.1+ Munchkin: Devido a alterações na política de cookies do Safari, a capacidade do Munchkin de rastrear usuários em sessões no mesmo domínio será limitada pelo ITP a 1 ou 7 dias com base na versão do navegador e do navegador usada pelo visitante. Para levar isso em conta, estamos implementando um novo serviço da Web para permitir que os cookies do Munchkin sejam definidos com um cabeçalho Set-Cookie por meio da resposta HTTP. Mais informações sobre como implementar este novo serviço podem ser encontradas [aqui](https://nation.marketo.com/docs/DOC-7351).


**_Versão do produto_** [WebinarAssocie-se ](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) em 3 de março às 11:00AM PT / 2:00PM ET para um webinário em tempo real hospedado pela nossa equipe de produtos e saiba mais sobre os recursos incluídos nesta versão.
