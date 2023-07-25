---
description: Notas de versão - maio de 2021 - Documentação do Marketo - Documentação do produto
title: Notas de versão - maio de 2021
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1446'
ht-degree: 0%

---

# Notas de versão: maio de 2021 {#release-notes-may-21}

Os seguintes recursos estão incluídos na versão de maio de 2021. Verifique a edição do Marketo quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

**_Versões trimestrais_**

Os seguintes recursos serão lançados em **7 de maio de 2021**.

## Experiências baseadas em conta {#Account-based-eaperiences}

* **Smart Lists da conta (disponibilidade geral)** ![](assets/yellow-star.png): identifique e qualifique dinamicamente contas com os atributos de conta e pessoa desejados para direcionar em campanhas de marketing entre canais e envie alertas oportunos às Vendas para fechar negócios mais rapidamente. Esse novo recurso permite a automação robusta de estratégias de marketing baseadas em conta. As Smart Lists de conta estão disponíveis para clientes com Gerenciamento de conta do Target que estão na experiência de usuário de última geração.

## Experiência do usuário de última geração {#next-generation-user-experience}

Com a visualização da pesquisa global, os profissionais de marketing podem ver rapidamente onde um ativo compartilhado existe em sua instância. As guias do navegador exibem o local para melhorar a navegação nas Atividades de marketing ou no Design Studio. Filtros adicionais de árvore e pesquisa global ajudam a refinar seus critérios de pesquisa. A funcionalidade de arrastar e soltar na árvore foi restabelecida, permitindo mover pastas e ativos de maneira rápida e eficiente nas áreas principais do aplicativo. Ícones recém-atualizados (que atendem aos padrões de acessibilidade do Adobe) e selos de status permitem que os profissionais de marketing façam uma distinção entre pastas e ativos de maneira rápida e fácil na árvore e identifiquem o status de programas e ativos.

## Automação de experiência {#experience-automation}

* **Executar Etapas De Fluxo De Campanha**: simplifique os workflows de criação de campanha e melhore o desempenho da campanha com uma nova etapa de fluxo para Campanhas inteligentes. Crie e salve campanhas de modelo centralizadas para tarefas repetitivas no seu espaço de trabalho, como normalização de código de país, para serem chamadas e executadas a partir de qualquer Campanha inteligente por meio da nova etapa de fluxo &quot;Executar Campanha&quot;. Campanhas vinculadas serão executadas no pedido designado e garantirão a conclusão da tarefa antes de avançar para a próxima etapa do fluxo. Edite rapidamente o fluxo em apenas uma campanha centralizada para atualizar cada Campanha inteligente que a utiliza para simplificar o gerenciamento de dados, a pontuação de clientes potenciais e os fluxos de trabalho de roteamento.

## Orquestração entre canais {#cross-channel-orchestration}

* **Campos de dados sensíveis no Forms**: as informações de identificação pessoal (PII) do cliente do Protect são exibidas nos formulários do Adobe Marketo Engage definindo campos de dados como sigilosos e restringindo o preenchimento prévio do formulário para esses campos. Sempre que um visitante visualizar um formulário na página de aterrissagem, os campos definidos como confidenciais não mostrarão dados pré-preenchidos.

* **Bloquear envios de formulários de spam**: o Protect usa o banco de dados Adobe Marketo Engage de dados inválidos que podem causar alertas inválidos para vendas, acionar listas de pendências de campanha e criar atividades indesejadas. O novo mecanismo de validação rejeita envios de formulários inválidos e interrompe os ataques de bot. Seus dados estão mais limpos e suas campanhas de marketing são executadas conforme o esperado, minimizando o risco de enviar leads não qualificados para as vendas.

* **Aviso de aprovação do programa de email**: impede o envio de emails incorretos quando as novas edições são feitas em um programa aprovado anteriormente.  O aviso atua como uma proteção quando um profissional de marketing aplica alterações em um email que já foi aprovado, mas então se esquece de aprovar as alterações mais recentes e envia o email para um grande público sem conteúdo, conteúdo incorreto ou conteúdo antigo.

* **Filtrar atividade de bots de email**: evite alertas de vendas não intencionais e relatórios de email imprecisos por meio do novo recurso de filtragem de atividades do bot de email. Identifique e filtre aberturas e cliques que podem ser associados a bots de email que inspecionam links que levam a acionadores e alertas de vendas falsos ou relatórios incorretos.

## Aprimoramentos na API {#api-enhancements}

Várias atualizações críticas para APIs em massa e de cliente potencial, incluindo a capacidade de exportar dados de objetos personalizados em massa, associar a empresa ao cliente potencial em massa, a capacidade de filtrar a extração de atividade em massa com base em um atributo principal e a capacidade de criar e atualizar a associação ao programa.

* **Aninhar programas de evento**: No Adobe Marketo Engage, você pode criar, clonar ou mover programas de eventos em outros tipos de programas. Essa funcionalidade agora é permitida na API de ativos.

* **API de programa de exclusão aprimorada**: permite que aplicativos integrados excluam programas contendo tipos adicionais de ativos, sem exigir que os usuários o façam manualmente no Adobe Marketo Engage.

* **Membros do programa**: os profissionais de marketing podem consultar todos os registros de membros de um programa selecionado de acordo com critérios diferentes, como status de membros de programas. Compartilhe essas informações com um aplicativo externo, uma ferramenta de business intelligence ou a Adobe Experience Cloud para segmentar e melhorar a segmentação e criar um envolvimento mais direcionado.

* **Extração de Objeto Personalizado em Massa**: a exportação de dados em massa complementa os recursos de importação que os analistas de dados já estão desfrutando no Adobe Marketo Engage. Agora é possível extrair dados armazenados em objetos personalizados de primeiro nível do Adobe Marketo Engage em massa e carregá-los em outro aplicativo, data warehouse ou ferramenta BI (Business Intelligence) para obter melhores insights sobre os dados na instância do Adobe Marketo Engage.  O movimento de dados em massa de objeto personalizado é bidirecional e pode ser agendado em um momento conveniente.

* **API de metadados de campos personalizados**: economize tempo automatizando a criação de campos personalizados enquanto configura as integrações do Adobe Marketo Engage com um aplicativo de terceiros. Essa automação beneficia especialmente os clientes com várias instâncias do Adobe Marketo Engage que agora podem simplificar a criação de campos personalizados que costumavam exigir trabalho manual em cada instância. Simplifique a criação de campos personalizados e economize tempo nessa atividade que consome recursos.

* **API de extração de atividade em massa**: obtenha controle sobre a quantidade e o tipo de dados ao executar extrações em massa. Filtre pontos de dados desnecessários e controle o número de chamadas de API necessárias para extrair dados da atividade em massa.  Por exemplo, selecione emails abertos, visite uma página da Web ou altere a pontuação de lead e deixe para trás outras alterações no valor que você não deseja analisar. Simplifique o processo para diminuir o número de chamadas de API e a limpeza de dados.

* **API do lead**: Identifique clientes potenciais no Adobe Marketo Engage que tenham Adobe ECID (ID de Experience Cloud) associada a eles.  Os clientes do Adobe Marketo Engage podem criar uma lista de clientes potenciais a partir de uma campanha selecionada e usar as ECIDs (Experience Cloud ID) para criar relatórios no Adobe Analytics para essa lista específica. A integração entre o Adobe Marketo Engage e o Adobe Experience Cloud abre oportunidades ilimitadas para segmentação, direcionamento e relatórios.

* **API de importação de leads em massa**: controlar a importação de clientes potenciais em massa e os recursos necessários. Esse aprimoramento cria associação entre lead e empresa durante o processo de importação de lead em massa. Aumente a eficiência e o desempenho do trabalho com dados e diminua o uso se as chamadas de API.

* **Integração baseada em API da Web para clientes do Microsoft Dynamics Online**: a API da Web do MS Dynamics foi introduzida com o protocolo REST versão 8.0 e implementa OData (Open Data Protocol) v4. OData é um padrão da OASIS (Organization for the Advancement of Structured Information Standards) para desenvolver e consumir serviços RESTful a partir de dados avançados. Os clientes do Adobe Marketo Engage que requerem integração com o Microsoft Dynamics usando esse método estão sendo migrados no momento para a conexão baseada em API da Web do SOAP (Simple Object Access Protocol).

## Ambiente de dados de marketing {#marketing-data-environment}

* **Exportação XLSX**: atualizamos os recursos de exportação em todo o produto para oferecer suporte ao XLSX em vez do XLS. Isso significa que em qualquer lugar do produto no qual a exportação XLS é suportada no momento, essa opção será substituída por uma opção para exportar para XLSX. Essa alteração afetará os nomes de arquivos de todas as exportações de relatórios e outros dados do Excel pelo Adobe Marketo Engage.

* **Pesquisar por ID de cliente potencial**: acesse rapidamente a pesquisa de registros de clientes potenciais pelo ID de clientes potenciais da Adobe Marketo Engage no banco de dados de clientes potenciais ou na lista estática. Na janela Localização Rápida, basta digitar `[id]` com o número correspondente, as informações do lead serão exibidas. Os usuários podem revisar rapidamente os detalhes da oportunidade, da empresa ou do cliente potencial.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integração com o LinkedIn Lead Gen Forms (Beta)**: obtenha mais visibilidade sobre o investimento e o ROI do seu canal do LinkedIn com a solução de atribuição Bizible premium. Por meio da mais recente integração com o Lead Gen Forms da LinkedIn, a Bizible obtém insights sobre formulários que foram enviados na plataforma LinkedIn. Esses preenchimentos de formulário são comparados com clientes potenciais da sua instância do CRM (Customer Relationship Management) ou Adobe Marketo Engage para que sejam qualificados para atribuição e possam ser rastreados em relação a outros contratos de marketing.

## Anúncios {#announcements}

* **Plataformas de switching de documentos do produto Marketo**: estamos animados em anunciar que os Documentos de produto do Marketo ingressaram na Adobe Experience League a partir de sexta-feira, 7 de maio. Você ainda poderá usar o URL: docs.marketo.com e, se tiver algum artigo existente marcado, será redirecionado. Todos os documentos do produto estão disponíveis na nova plataforma, com melhorias planejadas para o final deste ano.

* **Administração simplificada de usuários e logon único fornecidos pelo sistema de identidade do Adobe**: a partir de julho de 2021, os novos clientes da Adobe Marketo Engage serão integrados usando as credenciais de usuário do Adobe. A migração dos clientes atuais para o sistema de identidade integrado não ocorrerá até meados de 2022 e nenhuma ação do cliente será necessária até aviso em contrário. O logon único permite que os administradores de TI/segurança gerenciem várias instâncias de produtos da Adobe Marketo Engage juntamente com outras soluções de Experience Cloud, além de configurar o SSO (Shared Services Organization) por meio de um console comum. Os administradores podem gerenciar convenientemente grupos de usuários e direitos de usuário por meio de um Admin Console comum.

**_Webinário de lançamento do produto_**

[Webinário da versão de Marketo Engage de maio de 2021](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
