---
unique-page-id: 37355826
description: Notas de versão - 20 de fevereiro - Documentos da Marketo - Documentação do produto
title: Notas de versão - fevereiro de 2020
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%

---

# Notas de versão: Fev de 20 {#release-notes-feb}

Os seguintes recursos estão incluídos na versão de fevereiro de 20. Verifique sua edição do Marketo para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela ( ![(estrela)](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestrais_** Os seguintes recursos foram lançados em **21 de fevereiro de 2020**.

## Marketo Engage principal {#core-marketo-engage}

* **Ação de fluxo &quot;Alterar proprietário na Microsoft&quot; do Microsoft Dynamics**: Mantenha o controle dos dados do Microsoft Dynamics CRM com a capacidade de alterar um cliente potencial/proprietário de contato diretamente do Marketo Engage. Este é um aprimoramento do nosso recurso de Integração de CRM nativa.
* **APIs de gerenciamento de usuários**: Automatize o gerenciamento de usuários e funções por meio de sistemas externos de gerenciamento de identidade e organização. Este é um aprimoramento do nosso recurso de chamadas de API.
* **APIs do Esquema de objeto personalizado**: Gerencie e forneça automaticamente esquemas de objetos personalizados em várias instâncias no Marketo Engage para manter a consistência dos modelos de dados em todas as ferramentas de vendas e marketing. Com essa API, você pode definir e testar objetos personalizados em uma sandbox ou centro de excelência e provisionar para quantas instâncias forem necessárias. Este é um aprimoramento do nosso recurso de chamadas de APIs. Entre em contato com o representante do Marketo Engage para saber como obter acesso a esse aprimoramento.
* **APIs de regras de redirecionamento de página inicial**: Automatize o gerenciamento das regras de redirecionamento da landing page. Este é um aprimoramento do nosso recurso de chamadas de API.
* **Cache do descritor de formulário**: Estamos reduzindo o tempo de carregamento de formulários incorporados e melhorando a estabilidade geral dos aplicativos, armazenando formulários em cache como recursos. Observe que as aprovações feitas em formulários incorporados podem levar até quatro minutos para serem refletidas na Web. Este é um aprimoramento do nosso recurso Páginas de aterrissagem e Forms.

<br> 

**_Lançamento em todo o trimestre_**

Os seguintes recursos estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Bizible {#bizible}

![(estrela)](assets/yellow-star.png)

* **Segmentação com base em conta**: Analise a atribuição no nível da Conta com a capacidade de criar segmentos e filtros para quadros do Discover com base em atributos da Conta. Use esses segmentos para detalhar o desempenho de marketing com base em conta.
* **Salvar filtros**: Salve filtros específicos do painel exclusivos de cada usuário para analisar seus painéis de forma rápida e consistente.
* **Exportar para PDF**: Compartilhe insights valiosos em sua organização exportando Painéis Bizible como PDF.

## SalesConnect {#sales-connect}

* **Compor atualizações da janela**: Simplificamos o processo de seleção de modelos e envio de emails por meio do Sales Connect. Use a janela Compor em nosso cliente da Web e no Salesforce como um balcão único para vendedores, com a capacidade de salvar categorias de modelo, agendar emails, enviar emails em massa e enviar emails com rastreamento de visualização e cliques.
* **Atualizações do Centro de Comando**: Estamos recriando o Centro de Comando do Sales Connect para fornecer aos vendedores informações sobre todos os emails, chamadas e tarefas que foram iniciados pelo Sales Connect. Eles também podem visualizar informações como envolvimento por email e capacidade de entrega tudo a partir do Centro de Comando.

<br> 

## Anúncios {#announcements}

* **Centro de Sucesso do Marketo Engage**: Estamos lançando o Centro de Sucesso da Marketo em fevereiro de 2020. O Centro de sucesso é um centro de ajuda do produto que permite pesquisar documentos de produtos e a Comunidade, iniciar guias passo a passo, acessar conteúdo de adoção, como a Marketo University e vídeos de práticas recomendadas do peer e muito mais, diretamente da sua instância do Marketo Engage. **Observação**: Esse recurso será lançado como um beta na Austrália e Nova Zelândia e será implantado na América do Norte posteriormente no trimestre.

## Descontinuações {#deprecations}

* **Parâmetro &quot;_method&quot; da API de ativos**: Após setembro de 2020, os endpoints da API de ativos não aceitarão mais &quot;_method&quot; para transmitir os Parâmetros de consulta em um corpo do POST para ignorar as limitações de comprimento do URI. Para acomodar solicitações que exigiram esse parâmetro, o limite de URI para APIs de ativos será aumentado de 6KiB para 65KiB, de modo que URIs de solicitação longa possam ser enviadas.
* **Substituição do suporte ao Internet Explorer**: A partir do nosso lançamento realizado em 31 de julho de 2020, a interface do usuário do Marketo Engage não será mais compatível com o Internet Explorer.

**_Webinar da versão do produto_** [Junte-se a nós](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) em 3 de março, às 11:00 PT / 2:00 PM ET, para um webinário em tempo real hospedado pela nossa equipe de produtos, e saiba mais sobre os recursos incluídos nesta versão.
