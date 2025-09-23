---
unique-page-id: 37355826
description: Notas de versão - 20 de fevereiro - Documentação do Marketo - Documentação do produto
title: Notas de versão - fevereiro de 20
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 2%

---

# Notas de versão: fevereiro de 2020 {#release-notes-feb}

Os seguintes recursos estão incluídos na versão de fevereiro de 2020. Verifique a edição do Marketo quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela ( ![(estrela)](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

**_Versões Trimestrais_** Os seguintes recursos foram lançados em **21 de fevereiro de 2020**.

## Marketo Engage principal {#core-marketo-engage}

* **[!DNL Microsoft Dynamics]Ação de Fluxo &quot;Alterar Proprietário no Microsoft&quot;**: mantenha o controle dos dados do CRM do [!DNL Microsoft Dynamics] com a capacidade de alterar um proprietário de cliente potencial/contato diretamente do Marketo Engage. Isso é um aprimoramento do nosso recurso de Integração nativa de CRM.
* **APIs de gerenciamento de usuários**: automatize o gerenciamento de usuários e funções por meio de sistemas externos de gerenciamento de identidades e organizações. Isso é um aprimoramento do recurso Chamadas de API.
* **APIs de esquema de objeto personalizado**: gerencie e provisione automaticamente esquemas de objeto personalizados em instâncias no Marketo Engage para manter os modelos de dados consistentes em suas ferramentas de vendas e marketing. Com essa API, você pode definir e testar objetos personalizados em uma sandbox ou centro de excelência e provisionar para quantas instâncias forem necessárias. Isso é um aprimoramento do recurso Chamadas de APIs. Entre em contato com seu representante da Marketo Engage para saber como obter acesso a esse aprimoramento.
* **APIs de Regras de Redirecionamento de Página de Aterrissagem**: Automatize o gerenciamento de regras de redirecionamento de página de aterrissagem. Isso é um aprimoramento do recurso Chamadas de API.
* **Cache do Descritor de Formulário**: estamos reduzindo o tempo de carregamento de formulários inseridos e aprimorando a estabilidade geral do aplicativo, armazenando formulários em cache como recursos. Observe que as aprovações feitas em formulários incorporados podem levar até quatro minutos para serem refletidas na Web. Isso é um aprimoramento do recurso Landing Pages e Forms.

<br> 

**_Liberando Durante o Trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

## [!DNL Bizible] {#bizible}

![(estrela)](assets/yellow-star.png)

* **Segmentação baseada em conta**: analise a atribuição no nível da conta com a capacidade de criar segmentos e filtros para quadros do Discover com base em atributos da conta. Use esses segmentos para detalhar seu desempenho de marketing baseado em conta.
* **Salvando Filtros**: Salve filtros específicos do painel exclusivos para cada usuário para analisar seus painéis de maneira rápida e consistente.
* **Exportar para o PDF**: compartilhe insights valiosos em sua organização exportando Painéis Bizible como PDFs.

## [!DNL Sales Connect] {#sales-connect}

* **Compor Atualizações da Janela**: simplificamos o processo para selecionar modelos e enviar emails por meio do [!DNL Sales Connect]. Use a janela Compor no cliente da Web e no Salesforce como um balcão único para vendedores, com a capacidade de salvar categorias de modelo, agendar emails, enviar emails em massa e enviar emails com rastreamento de visualização e clique.
* **Atualizações do Command Center**: estamos reconstruindo o [!DNL Sales Connect] Command Center para fornecer aos vendedores insight todos os seus Emails, Chamadas e Tarefas que foram iniciados a partir de [!DNL Sales Connect]. Eles também podem exibir informações como envolvimento de email e capacidade de delivery, tudo no Centro de comando.

<br> 

## Anúncios {#announcements}

* **Centro de Sucesso do Marketo Engage**: iniciaremos o Centro de Sucesso do Marketo em fevereiro de 2020. O Centro de sucesso é um centro de ajuda no produto que permite pesquisar em Documentos de produto e na Comunidade, iniciar guias tutoriais, acessar conteúdo de adoção, como a Marketo University e vídeos de práticas recomendadas de colegas, e muito mais, diretamente da instância do Marketo Engage. **Observação**: este recurso será iniciado como um beta na ANZ e será implantado na América do Norte posteriormente neste trimestre.

## Descontinuações {#deprecations}

* **Parâmetro &quot;_method&quot; da API de ativos**: a partir de setembro de 2020, os endpoints da API de ativos não aceitarão mais &quot;_method&quot; para transmitir os Parâmetros de consulta em um corpo POST para ignorar as limitações de comprimento de URI. Para acomodar solicitações que exigem esse parâmetro, o limite do URI para APIs de ativos será aumentado de 6 KiB para 65 KiB, para que URIs de solicitações longas possam ser enviadas.
* **Desativação do suporte ao Internet Explorer**: a partir do lançamento realizado em 31 de julho de 2020, a interface do usuário do Marketo Engage não será mais compatível com o Internet Explorer.

**_Webinário de lançamento do produto_** [Junte-se a nós](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) em 3 de março às 11:00AM PT / 2:00PM ET para um webinário ao vivo hospedado por nossa equipe de produtos e saiba mais sobre os recursos incluídos nesta versão.
