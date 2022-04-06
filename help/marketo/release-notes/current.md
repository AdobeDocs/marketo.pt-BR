---
description: Notas de versão atuais - Documentação do Marketo - Documentação do produto
title: Notas de versão atuais
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 621bb7db9485ef1cc559b5b161d5acb606bc4903
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Notas de versão: Maio de 2022 {#release-notes-may-22}

Abaixo você encontrará todos os recursos incluídos na versão de 22 de maio. Verifique sua edição do Adobe Marketo Engage para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestrais_**

Os seguintes recursos começarão a ser lançados em **6 de maio de 2022**, com uma distribuição em fases dos recursos restantes durante as semanas subsequentes (salvo indicação em contrário).

## Integração de CRM nativo {#native-crm-integration}

**Integração de Veva Nativa ao CRM (disponibilidade limitada)**: Melhore o envolvimento com os profissionais de saúde sincronizando a atividade entre o Veeva CRM e o Marketo Engage por meio da integração nativa. Essa integração permite que os profissionais de marketing criem experiências mais personalizadas e contínuas entre canais para os profissionais de saúde. Entre em contato com o Gerente de sucesso do cliente se estiver interessado em participar.

## Orquestração entre canais {#cross-channel-orchestration}

**Eventos de chatbot para chat dinâmico**: Utilize dados de comportamento mais detalhados para visitantes da Web, como tempo na página, tempo no site e porcentagem de rolagem da página para definir quando uma caixa de diálogo de bate-papo deve ser exibida.

**Incorporar PDF para bate-papo dinâmico**: Aumente o engajamento e compartilhe conteúdo significativo incorporando PDF às caixas de diálogo de bate-papo e meça o desempenho do conteúdo por meio do rastreamento da atividade de engajamento.

**Suporte de idioma estendido para bate-papo dinâmico**: A interface do usuário do Dynamic Chat agora também estará disponível em francês, alemão, japonês, português e espanhol. As caixas de diálogo de bate-papo também podem ser configuradas nesses idiomas.

**Excluir URLs para bate-papo dinâmico**: Controlar em quais de suas páginas da Web o Dynamic Chat é exibido com a capacidade de excluir URLs específicos dos critérios de direcionamento.

**Aprimoramentos na filtragem de atividade de bot de email**: Continue a proteger a integridade de seu banco de dados com a capacidade de identificar o comportamento de bot com base em links ocultos, agentes do usuário ou IPs e padrões de proximidade, além da identificação de correspondência da lista IAB existente. Visualize estatísticas de atividades de bot que permitem compreender o número de atividades de bot identificadas para cada tipo.

**Cabeçalho STS para links de rastreamento de email**: Atender às práticas recomendadas de segurança com a capacidade de aplicar cabeçalhos de Segurança de Transporte Seguro para garantir que o tráfego para links rastreados seja sempre seguro.

## Experiência da próxima geração {#next-generation-experience}

**Alternar Switch padrão para a experiência de última geração**: o switch de alternância será o padrão para a nova experiência em todas as telas em que estiver disponível, facilitando a descoberta dos designs atualizados e das melhorias de usabilidade.

**Tela atualizada na experiência de próxima geração**:

Estamos fornecendo a Exibição de detalhes do modelo de email no Design Studio na experiência da próxima geração, oferecendo melhorias atualizadas de design e usabilidade acessíveis por meio do switch de alternância.

## Automação de experiência {#experience-automation}

**Etapas de fluxo de autoatendimento (beta continuado)**: Expanda a conectividade entre o Marketo Engage e o resto da pilha com a capacidade de criar etapas de fluxo personalizadas para uso em Campanhas inteligentes. Os usuários e parceiros do Marketo Engage podem aproveitar essa funcionalidade para permitir o uso de serviços da Web externos em campanhas acionadoras, em lote e executáveis (em contraste com webhooks que só podem ser usados em campanhas acionadoras).

## Melhorias da API {#api-enhancements}

* **Acesso à API expandido para assinaturas ativadas por CRM**: Estamos expandindo o acesso à API para assinaturas que têm uma sincronização de CRM ativada para permitir que os usuários recuperem empresas, oportunidades e pessoas de vendas do Marketo Engage.
* **Suporte para tipos de dados &quot;ocultos&quot; no Forms**: Fornece a capacidade de gerenciar campos de formulário ocultos por meio da API.
* **Oferece suporte a valores de comparação múltiplos para isNot Form via Rules**: Gerencie a visibilidade de campos de formulário com base no fato de o valor de outro campo não ser um dos valores em uma determinada lista.
* **Permitir configuração de Exibir e Valores Enviados em Selecionar Listas Separadamente**: Defina o valor de exibição e o valor enviado em um campo separadamente. Por exemplo, mostre o nome de um hotel, mas envie uma ID interna para o backend.
* **Permitir configuração de desativação do rastreamento aberto ao criar ou atualizar email**: Crie um email com o rastreamento aberto desativado.

## Anúncios {#announcements}

**Verificação de email e exclusividade**: A partir de abril, a implementação da Verificação de email será iniciada. Nesse momento, os endereços de email de usuário do Marketo Engage exigirão verificação e exclusividade (isso não se aplica aos usuários somente de API). Os usuários autenticados do serviço de diretório terão seus emails verificados automaticamente quando sua assinatura for habilitada com a Verificação de email.

Verificação de email para assinaturas usando o recurso &quot;Logon na caixa de diálogo de usuário do convite&quot; ou que tenham um único email associado a vários usuários coincidirá com a versão de maio. As assinaturas com um único email associado a vários usuários serão ativadas com a Verificação de email e exigirão que esses usuários resolvam o conflito e usem um email exclusivo por usuário. Quando o recurso &quot;Logon na caixa de diálogo de usuário do convite&quot; estiver ativado, os usuários convidados por meio desse recurso precisarão ter um endereço de email exclusivo. Para usuários somente de API convidados por meio desse recurso, o endereço de email não precisa ser exclusivo.

**_Webinar da versão do produto_**

Junte-se a nós em 11 de maio de 2022, às 9h PT / 12h ET para um [webinário ao vivo](https://engage.marketo.com/2022_March_May_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} hospedado pela nossa equipe de produtos, onde você pode aprender a usar todas as inovações de produtos mais recentes.
