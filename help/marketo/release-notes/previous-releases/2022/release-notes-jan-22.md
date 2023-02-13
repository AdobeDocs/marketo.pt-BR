---
description: Notas de versão - Janeiro de 2022 - Documentação da Marketo - Documentação do produto
title: Notas de versão - Janeiro de 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: ec783ee58e3c249da036d4770231eb9d7ef61bbd
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 3%

---

# Notas de versão: Janeiro de 2022 {#release-notes-jan-22}

Os seguintes recursos estão incluídos na versão de 22 de janeiro. Verifique sua edição do Adobe Marketo Engage para ver a disponibilidade dos recursos.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante de Marketo Engage para saber mais.

**_Versões trimestrais_**

Os seguintes recursos começarão a ser lançados em **21 de janeiro de 2022**, com uma implantação em fases de cada recurso nas semanas seguintes (salvo indicação em contrário).

## Experiência da próxima geração {#modern-ux}

* **Telas atualizadas na experiência de próxima geração**: Estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração que oferecem melhorias atualizadas de design e usabilidade acessíveis por meio do switch de alternância:

   * Detalhes do ativo da página de aterrissagem no Design Studio
   * Detalhes do ativo da página de aterrissagem nas atividades de marketing

## Integração do Microsoft Dynamics {#microsoft-dynamics-integration}

* **Sincronização do Tipo de Campo de Conjunto de Opções Multisseleção Geralmente Disponível**: Sincronize o tipo de campo de conjunto de opções multisseleções do Microsoft Dynamics para aproveitar as Smart Lists e as Campanhas inteligentes para obter um direcionamento de público-alvo mais granular. Os exemplos incluem: tópicos/produtos de interesse, modos de comunicação preferidos e muito mais. Esta nova sincronização está disponível para o Microsoft Dynamics versão 9.X (incluindo o Dynamics 365 Online).

* **Autenticação de servidor para servidor para Microsoft Dynamics 365 Online**: Para maior segurança, agora oferecemos suporte ao Servidor para Servidor (S2S) como um modo adicional de autenticação para o usuário de sincronização de Marketo Engage no Azure Ative Diretory para acesso não interativo ao Microsoft Dynamics 365 Online. Isso permite usar a autenticação de vários fatores, pois todas as autenticações e logon serão baseadas no OAuth (somente a ID do cliente e o segredo do cliente).

>[!NOTE]
>
>O modo S2S é baseado no Usuário do aplicativo em vez do Usuário licenciado, o que salva o uso de uma licença adicional.

## Administração {#administration}

* **[Regras de validação do formulário](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: Mantenha a integridade do banco de dados com a capacidade de bloquear domínios de email problemáticos ou indesejáveis de enviar formulários Marketo Engage. O painel Regra de validação de formulário global permite que os administradores definam uma  lista de bloqueios ou habilitem uma lista predefinida de domínios de consumidores livres para bloquear formulários.

* **[Segurança do cabeçalho da página de aterrissagem](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: Os administradores podem gerenciar cabeçalhos Strict Transport Security e X-Frame Options em seus domínios de página de aterrissagem para impor requisitos de segurança rigorosos.

**_Lançamento em todo o trimestre_**

Os seguintes recursos estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Conector de destino AEP Marketo Engage - Criar novos leads {#aep-marketo-engage-destination-connector}

Os clientes do Marketo Engage que também usam o Adobe Experience Platform (AEP) podem maximizar seu banco de dados com a capacidade de enviar registros de pessoas novos para o Marketo Engage a partir do AEP por meio do conector de destino do AEP. Ao enviar segmentos de público-alvo do AEP para o Marketo Engage, pessoas no segmento que ainda não existem no banco de dados do Marketo Engage [pode ser adicionado automaticamente a ele](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

**Insight de vendas para o Salesforce CRM**

* **Nova Coluna de Tipo para Melhores Melhores Opções**: Os vendedores obterão insights mais rápidos com uma nova coluna chamada &quot;Tipo&quot; para diferenciar entre leads e contatos na página Melhores Melhores Melhores.

* **Atualização da API da Salesforce Platform**: Em resposta à aposentação do Salesforce nas versões 21.0 a 30.0 da API da plataforma Salesforce, o pacote Sales Insight foi atualizado com as APIs mais recentes.

* **Marca atualizada**: Todas as páginas de Insight de vendas estão sendo atualizadas para se alinharem à marca de Adobe.

**Insight de vendas para o Microsoft Dynamics**

* **Layout de conta atualizado**: Os vendedores podem obter uma visualização coletiva das principais atividades, como: atividades de email, atividades da web, momentos interessantes e alterações de pontuação para todos os contatos de uma conta.

## SalesConnect {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **Resultados da chamada e motivos**: Entenda e rastreie os esforços de saída de suas equipes de vendas com mais detalhes com o novo resultado da chamada totalmente personalizável e opções de motivo da chamada. Além desses novos campos, estamos introduzindo uma nova governança para impor o motivo da chamada e a seleção dos resultados enquanto os vendedores estão fazendo chamadas, nova governança para ativar ou desativar os motivos e resultados da chamada, e um novo campo personalizado Motivo da chamada e Atividade de saída do Salesforce para registrar dados no Salesforce. [Clique aqui](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) para saber mais.

* **Personalização de detalhes da atividade do Salesforce**: Capture mais dados de atividade de vendas e tarefa no Salesforce personalizando quais informações são adicionadas ao campo de assunto de tarefa do Salesforce quando uma atividade de vendas é registrada no Salesforce a partir do Sales Connect. [Clique aqui](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) para saber mais.

## Anúncios {#announcements}

* **Descontinuação do Marketo Sky**: Em março, o Marketo Sky não estará mais disponível à medida que concentramos nossos recursos no fornecimento da experiência do usuário da próxima geração. Em um esforço para manter o acesso à funcionalidade exclusiva do Marketo Sky hoje, estamos trazendo a Expiração de ativos e a Substituição de prioridade de campanha inteligente para a experiência principal em março. [Clique aqui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para saber mais.

* **Substituição de pontos de extremidade de formulário**: Os POSTs de formulário programático não aceitos no ponto de extremidade leadCapture/save2 serão rejeitados por Marketo Engage forms. [Clique aqui](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) para saber mais.

**Domínios do Marketo Engage - Configuração do Sales Insight**: Para domínios Marketo Engage que não têm certificado SSL provisionado e https://, as chamadas falharão com um erro de handshake SSL. Portanto, esses domínios serão encerrados. Como resultado, os usuários do Sales Insight com uma configuração mais antiga apontando para qualquer um desses domínios podem encontrar erros de chamada do sistema em sua página Principal, Contato, Conta, Painéis de Oportunidade ou Marketo Global. Recomendamos que você atualize seu [Configuração do Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) no Salesforce se encontrar esse erro. Você só precisa atualizar as credenciais do Marketo Engage destacadas na seção &quot;Configuração do Marketo Sales Insight&quot; do documento.

**_Webinar da versão do produto_**

[Webinar da versão do Marketo Engage de janeiro de 2022](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
