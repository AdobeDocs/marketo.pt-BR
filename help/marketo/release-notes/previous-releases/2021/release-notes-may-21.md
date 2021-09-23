---
description: Notas de versão - maio de 2021 - Documentação da Marketo - Documentação do produto
title: Notas de versão - maio de 2021
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '1481'
ht-degree: 0%

---

# Notas de versão: Maio de 2021 {#release-notes-may-21}

Os seguintes recursos estão incluídos na versão de 21 de maio. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestrais_**

Os seguintes recursos serão lançados em **7 de maio de 2021**.

## Experiências baseadas em conta {#Account-based-eaperiences}

* **Smart Lists de conta (disponibilidade geral)** ![](assets/yellow-star.png): Identifique e qualifique dinamicamente contas com os atributos de conta e pessoa desejados para direcionar em campanhas de marketing entre canais e envie alertas oportunos para Vendas para fechar negócios mais rapidamente. Esse novo recurso permite a automação robusta de estratégias de marketing baseadas em conta. As Listas inteligentes de contas estão disponíveis para clientes com Gerenciamento de conta do Target que estão na experiência de usuário de próxima geração.

## Experiência do usuário de próxima geração {#next-generation-user-experience}

Com a visualização de pesquisa global, os profissionais de marketing podem visualizar rapidamente onde um ativo compartilhado existe em sua instância. As guias Navegador exibem o local para melhorar a navegação nas Atividades de Marketing ou no Design Studio. Os filtros de pesquisa global e em árvore adicionais ajudam a refinar seus critérios de pesquisa. A funcionalidade de arrastar e soltar na árvore foi reativada, permitindo que você mova pastas e ativos de forma rápida e eficiente nas áreas do aplicativo principal. Os ícones recém-atualizados (que atendem aos padrões de acessibilidade do Adobe) e os rótulos de status permitem que os profissionais de marketing diferenciem pastas e ativos de forma rápida e fácil na árvore e identifiquem o status de programas e ativos.

## Automação de experiência {#experience-automation}

* **Executar etapas** do fluxo da campanha: Simplifique os workflows de criação de campanha e melhore o desempenho da campanha com uma nova etapa de fluxo para Campanhas inteligentes. Crie e salve campanhas de modelo centralizadas para tarefas repetitivas em seu espaço de trabalho, como normalização do código de país, a serem chamadas e executadas a partir de qualquer Campanha inteligente através da nova etapa de fluxo &quot;Executar campanha&quot;. As campanhas vinculadas serão executadas na ordem designada e garantirão a conclusão da tarefa antes de avançar para a próxima etapa do fluxo. Edite rapidamente o fluxo em apenas uma campanha centralizada para atualizar cada Campanha inteligente que está usando para simplificar o gerenciamento de dados, a pontuação de clientes potenciais e os workflows de roteamento.

## Orquestração entre canais {#cross-channel-orchestration}

* **Campos de dados confidenciais no Forms**: As informações de identificação pessoal (PII) do cliente do Protect não são exibidas nos formulários Adobe Marketo Engage, definindo campos de dados como confidenciais e restringindo o preenchimento do formulário para esses campos. Sempre que um visitante visualizar um formulário na landing page, os campos definidos como confidenciais não mostrarão dados pré-preenchidos.

* **Bloquear Envio** de Formulário de Spam: Protect seu banco de dados do Adobe Marketo Engage a partir de dados inúteis que podem causar alertas inválidos para vendas, acionar registros de campanha e criar atividades indesejadas. O novo mecanismo de validação rejeita envios de formulários inválidos e interrompe os ataques de bot. Seus dados são mais limpos e suas campanhas de marketing são executadas conforme o esperado, minimizando o risco de enviar leads não qualificados para vendas.

* **Aviso** de aprovação do programa de email: Impedir o envio de emails incorretos quando as novas edições forem feitas em um programa aprovado anteriormente.  O aviso atua como garantia quando um profissional de marketing aplica alterações a um email já aprovado, mas depois esquece de aprovar as alterações mais recentes e envia o email para um grande público sem conteúdo, conteúdo incorreto ou conteúdo antigo.

* **Atividade** Filtrar e-mail Bots: Evite alertas de vendas não intencionais e relatórios de email imprecisos por meio do novo recurso de filtragem de atividades de bot de email. Identifique e filtre aberturas e cliques que podem ser associados a bots de email inspecionando links que levam a acionadores falsos e alertas de vendas, ou relatórios incorretos.

## Melhorias da API {#api-enhancements}

Várias atualizações críticas para APIs em massa e em potencial, incluindo a capacidade de exportar dados de objetos personalizados em massa, associar empresa ao lead em massa, a capacidade de filtrar a extração de atividade em massa com base em um atributo principal e a capacidade de criar e atualizar a associação ao programa.

* **Aninhar programas** de evento: No Adobe Marketo Engage, você pode criar, clonar ou mover programas de evento em outros tipos de programas. Essa funcionalidade agora é permitida na API de ativos.

* **API** do programa de exclusão aprimorada: Permite que aplicativos integrados excluam programas contendo tipos adicionais de ativos, sem exigir que os usuários façam isso manualmente do Adobe Marketo Engage.

* **Associação** do Programa: Os profissionais de marketing podem consultar todos os registros de membros do programa para um programa selecionado, considerando critérios diferentes, como o status de membro do programa. Compartilhe essas informações com um aplicativo externo, uma ferramenta de inteligência de negócios ou o Adobe Experience Cloud para melhorar a segmentação e criar um envolvimento mais direcionado.

* **Extração** de Objeto Personalizado em Massa: A exportação de dados em massa complementa os recursos de importação que os analistas de dados já estão desfrutando no Adobe Marketo Engage. Agora eles podem extrair dados armazenados no Adobe de primeiro nível Objetos personalizados em massa, carregar esses dados em outro aplicativo, data warehouse ou ferramenta BI (Business Intelligence) para obter melhores insights sobre os dados na instância do Adobe Marketo Engage.  A movimentação de dados em massa do objeto personalizado é bidirecional e pode ser agendada em um momento conveniente.

* **API** de metadados de campos personalizados: Economize tempo ao automatizar a criação de campos personalizados ao configurar as integrações do Adobe Marketo Engage com um aplicativo de terceiros. Essa automação beneficia especialmente os clientes com várias instâncias de Marketo Engage Adobe que agora podem simplificar a criação de campos personalizados, antes necessários para o trabalho manual em cada instância. Simplifique a criação de campos personalizados e economize tempo nessa atividade que consome recursos.

* **API** de extração de atividade em massa: Obtenha controle sobre a quantidade e o tipo de dados ao executar extrações em massa. Filtre pontos de dados desnecessários e controle o número de chamadas de API necessárias para extrair dados de atividade em massa.  Por exemplo, selecione emails abertos, visite uma página da Web ou altere na pontuação de lead e deixe para trás outras alterações de valor que não deseja analisar. Simplifique o processo para diminuir o número de chamadas de API e limpeza de dados.

* **API** de cliente potencial: Identifique leads no Marketo Engage Adobe que têm Adobe ECID (Experience Cloud ID) associado a eles.  Os clientes do Adobe Marketo Engage podem criar uma lista de leads a partir de uma campanha selecionada e usar as ECIDs (Experience Cloud ID) para criar relatórios no Adobe Analytics para essa lista específica. A integração entre o Adobe Marketo Engage e o Adobe Experience Cloud abre oportunidades ilimitadas para segmentação, direcionamento e relatórios.

* **API** de importação de leads em massa: Controlar a importação de leads em massa e os recursos necessários. Esse aprimoramento cria associação entre o cliente potencial e a empresa durante o processo de importação de leads em massa. Aumente a eficiência do trabalho com dados e diminua o uso se a API chamar.

* **Integração baseada em API da Web para clientes** do Microsoft Dynamics Online: A API da Web do MS Dynamics foi introduzida com a versão 8.0 REST protocol e implementa OData (Open Data Protocol) v4. OData é um padrão OASIS (Organization for the Advancing of Structure Information Standards) para a construção e o consumo de serviços RESTful em relação a dados avançados. Os clientes do Adobe Marketo Engage que exigem integração com o Microsoft Dynamics usando este método estão sendo migrados para a conexão baseada em API da Web do SOAP (Simple Object Access Protocol).

## Ambiente de dados de marketing {#marketing-data-environment}

* **Exportação** XLSX: Atualizamos os recursos de exportação em todo o produto para oferecer suporte ao XLSX no lugar do XLS. Isso significa que em qualquer lugar do produto em que a exportação de XLS é atualmente compatível, essa opção será substituída por uma opção para exportar para XLSX. Essa alteração afetará os nomes de arquivo de todas as exportações de relatórios e outros dados do Excel do Adobe Marketo Engage.

* **Pesquisar por ID** de lead: Acesse rapidamente a pesquisa de registro de cliente potencial por ID de cliente potencial Adobe no banco de dados de cliente potencial ou na lista estática. Na janela Localização rápida, basta digitar `[id]` com o número correspondente e, em seguida, as informações de lead serão exibidas. Os usuários podem revisar rapidamente os detalhes do cliente potencial, da empresa ou da oportunidade.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integração com o LinkedIn Lead Gen Forms (Beta)**: Obtenha visibilidade profunda do investimento e do ROI do seu canal LinkedIn com a solução de atribuição Bizible premium. Por meio da mais recente integração com o Forms principal da LinkedIn, a Bizible obtém informações sobre formulários que foram enviados na plataforma LinkedIn. Esses preenchimentos de formulário são comparados com leads de sua instância do CRM (Gerenciamento de Relacionamento com o Cliente) ou do Adobe Marketo Engage para que sejam elegíveis para atribuição e possam ser rastreados em relação a seus outros envolvimentos de marketing.

## Anúncios {#announcements}

* **Plataformas** de troca de documentos do produto Marketo: Temos o prazer de anunciar que o Marketo Product Docs entrou na Adobe Experience League na sexta-feira, 7 de maio. Você ainda poderá usar o URL: docs.marketo.com, e se você tiver artigos existentes marcados, será redirecionado. Todos os documentos do produto estão disponíveis na nova plataforma, com melhorias planejadas para o fim deste ano.

* **Administração de usuário simplificada e logon único com base no sistema** de identidade do Adobe: A partir de julho de 2021, os novos clientes do Adobe Marketo Engage serão integrados usando credenciais de usuário do Adobe. A migração dos clientes atuais para o sistema de identidade integrado não ocorrerá até meados de 2022 e nenhuma ação do cliente será necessária até novo aviso. O logon único permite que os administradores de TI/segurança gerenciem várias instâncias de produto do Adobe Marketo Engage juntamente com outras soluções do Experience Cloud, bem como configure o SSO (Shared Services Organization) por meio de um console comum. Os administradores podem gerenciar convenientemente grupos de usuários e direitos de usuário por meio de um Admin Console comum.

**_Webinar da versão do produto_**

Quer saber mais sobre esses recursos e aprimoramentos? Certifique-se de [registrar-se agora](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html) para se juntar a nós em 13 de maio às 9h PT / 12h ET para um webinário ao vivo com nossa equipe de produtos para aprofundar essas inovações.
