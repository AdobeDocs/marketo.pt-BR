---
description: Notas de versão - Janeiro de 2022 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Janeiro de 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 1%

---

# Notas de versão: janeiro de 2022 {#release-notes-jan-22}

Os seguintes recursos estão incluídos na versão de janeiro de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

**_Versões Trimestrais_**

Os recursos a seguir serão lançados em **21 de janeiro de 2022**, com uma implantação em fases de cada recurso nas semanas seguintes (a menos que especificado de outra forma).

## Experiência de última geração {#modern-ux}

* **Screens atualizado na Experiência da Próxima Geração**: estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração, que oferecem um design atualizado e aprimoramentos de usabilidade acessíveis via switch de alternância:

   * Detalhes de ativos de landing page no Design Studio
   * Detalhes de ativos de landing page em atividades de marketing

## Integração do Microsoft Dynamics {#microsoft-dynamics-integration}

* **Sincronização do tipo de campo Multiselect Optionset Geralmente disponível**: sincronize o tipo de campo multiselect optionset do Microsoft Dynamics para aproveitar as Smart Lists e as Smart Campaigns para um direcionamento mais granular de público-alvo. Os exemplos incluem: tópicos/produtos de interesse, modos de comunicação preferidos e muito mais. Essa nova sincronização está disponível para o Microsoft Dynamics versão 9.X (incluindo o Dynamics 365 Online).

* **Autenticação de Servidor para Servidor para Microsoft Dynamics 365 Online**: para maior segurança, ofereceremos suporte a Servidor para Servidor (S2S) como um modo adicional de autenticação para o usuário de sincronização de Marketo Engage no Azure Ative Diretory para acesso não interativo ao Microsoft Dynamics 365 Online. Isso permite empregar a autenticação multifator, pois todas as autenticações e logons serão baseados no OAuth (somente ID do cliente e segredo do cliente).

>[!NOTE]
>
>O modo S2S é baseado no usuário do aplicativo em vez do usuário licenciado, o que salva o uso de uma licença adicional.

## Administração {#administration}

* **[Regras de validação de formulário](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: mantêm a integridade do banco de dados com a capacidade de impedir que domínios de email problemáticos ou indesejáveis enviem formulários Marketo Engage. O painel Regra de validação de formulário global permite que os administradores definam uma inclui na lista de bloqueios de formulário ou habilitem uma lista predefinida de domínios de consumidores livres para bloquear formulários.

* **[Segurança de Cabeçalho de Página de Aterrissagem](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: os administradores podem gerenciar cabeçalhos de Segurança de Transporte Restrita e Opções de X-Frame em seus domínios de página de aterrissagem para aplicar requisitos de segurança rigorosos.

**_Liberando Durante o Trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Conector de destino do AEP Marketo Engage - Criar novos clientes em potencial {#aep-marketo-engage-destination-connector}

Os clientes do Marketo Engage que também usam o Adobe Experience Platform (AEP) podem maximizar seu banco de dados com a capacidade de enviar registros de novas pessoas para o Marketo Engage por meio do conector de destino do AEP. Ao enviar segmentos de público do AEP para o Marketo Engage, as pessoas dentro do segmento que ainda não existe no banco de dados do Marketo Engage [podem ser adicionadas automaticamente a ele](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

**Sales Insight for Salesforce CRM**

* **Nova Coluna do Tipo para Melhores Opções**: os vendedores obterão insights mais rápidos com uma nova coluna chamada &quot;Tipo&quot; para diferenciar clientes potenciais e contatos na página Melhores Opções.

* **Atualização da API da plataforma Salesforce**: em resposta à desativação da API da plataforma Salesforce versões 21.0 a 30.0, o pacote Sales Insight foi atualizado com as APIs mais recentes.

* **Marca atualizada**: todas as páginas de Insight de vendas estão sendo atualizadas para se alinharem à marca do Adobe.

**Sales Insight for Microsoft Dynamics**

* **Layout de conta atualizado**: os vendedores podem obter uma visão coletiva das principais atividades, como atividades de email, atividades da Web, momentos interessantes e alterações de pontuação para todos os contatos em uma conta.

## Sales Connect {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **Resultados e Motivos de Chamadas**: compreenda e rastreie com mais detalhes os esforços de saída de suas equipes de vendas com resultados de chamadas e opções de motivo de chamadas novas e totalmente personalizáveis. Além desses novos campos, estamos introduzindo uma nova governança para aplicar a seleção de motivo e resultado da chamada enquanto os vendedores fazem chamadas, uma nova governança para ativar ou desativar motivos e resultados da chamada, e um novo campo personalizado Motivo da chamada e Atividade de resultado da chamada do Salesforce para registrar dados no Salesforce. [Clique aqui](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) para saber mais.

* **Personalização dos Detalhes da Atividade do Salesforce**: capture mais dados da atividade de vendas e da tarefa no Salesforce personalizando quais informações são adicionadas ao campo de assunto da tarefa do Salesforce quando uma atividade de vendas é registrada no Salesforce a partir do Sales Connect. [Clique aqui](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) para saber mais.

## Anúncios {#announcements}

* **Descontinuação do Marketo Sky**: em março, o Marketo Sky não estará mais disponível, pois concentraremos nossos recursos no fornecimento da experiência de usuário da próxima geração. Em um esforço para manter o acesso à funcionalidade exclusiva do Marketo Sky hoje, estamos trazendo a Expiração de ativos e a Substituição de prioridade da Campanha inteligente para a experiência principal em março. [Clique aqui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para saber mais.

* **Descontinuação de Pontos de Extremidade de Formulário**: POSTs de formulário programático sem suporte para o ponto de extremidade leadCapture/save2 serão rejeitados por formulários Marketo Engage. [Clique aqui](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) para saber mais.

**Domínios Marketo Engage - Configuração do Sales Insight**: para domínios Marketo Engage que não têm certificado SSL provisionado e https://, as chamadas falharão com um erro de handshake SSL. Portanto, esses domínios serão encerrados. Como resultado, os usuários do Sales Insight com uma configuração mais antiga apontando para qualquer um desses domínios podem encontrar erros de chamada do sistema em suas páginas de cliente potencial, de contato, de conta, de painéis de oportunidade ou globais da Marketo. Recomendamos que você atualize sua [configuração de Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) no Salesforce se encontrar esse erro. Você só precisa atualizar as credenciais de Marketo Engage realçadas na seção &quot;Configuração do Marketo Sales Insight&quot; do documento.

**_Webinar de lançamento de produto_**

[Webinário da versão do Marketo Engage de janeiro de 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
