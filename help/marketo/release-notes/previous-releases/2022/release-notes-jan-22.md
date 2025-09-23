---
description: Notas de versão - Janeiro de 2022 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Janeiro de 2022
exl-id: babc4e7f-3f11-4883-80c6-58e69c3e1ab4
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 4%

---

# Notas de versão: janeiro de 2022 {#release-notes-jan-22}

Os seguintes recursos estão incluídos na versão de janeiro de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

**_Versões Trimestrais_**

Os recursos a seguir serão lançados em **21 de janeiro de 2022**, com uma implantação em fases de cada recurso nas semanas seguintes (a menos que especificado de outra forma).

## Experiência de última geração {#modern-ux}

* **Screens atualizado na Experiência da Próxima Geração**: estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração, que oferecem um design atualizado e aprimoramentos de usabilidade acessíveis via switch de alternância:

   * Detalhes de Ativo da Página de Aterrissagem no [!UICONTROL Design Studio]
   * Detalhes de ativos da landing page em [!UICONTROL atividades de marketing]

## [!DNL Microsoft Dynamics] Integração {#microsoft-dynamics-integration}

* **Sincronização do Tipo de Campo Multiselect Optionset Geralmente Disponível**: sincronize o tipo de campo multiselect optionset de [!DNL Microsoft Dynamics] para aproveitar em Smart Lists e Campanhas Inteligentes para um direcionamento de público mais granular. Os exemplos incluem: tópicos/produtos de interesse, modos de comunicação preferidos e muito mais. Esta nova sincronização está disponível para [!DNL Microsoft Dynamics] versão 9.X (incluindo o Dynamics 365 Online).

* **Autenticação de Servidor para Servidor para[!DNL Microsoft Dynamics 365 Online]**: para aumentar a segurança, ofereceremos suporte a S2S (Servidor para Servidor) como um modo adicional de autenticação para o usuário de sincronização do Marketo Engage no Azure Ative Diretory para acesso não interativo ao [!DNL Microsoft Dynamics 365 Online]. Isso permite empregar a autenticação multifator, pois todas as autenticações e logons serão baseados no OAuth (somente ID do cliente e segredo do cliente).

>[!NOTE]
>
>O modo S2S é baseado no usuário do aplicativo em vez do usuário licenciado, o que salva o uso de uma licença adicional.

## Administração {#administration}

* **[Regras de validação de formulários](/help/marketo/product-docs/administration/settings/global-form-validation-rules.md)**: mantêm a integridade do banco de dados com a capacidade de bloquear o envio de formulários do Marketo Engage por domínios de email problemáticos ou indesejáveis. O painel Regra de validação de formulário global permite que os administradores definam uma inclui na lista de bloqueios de formulário ou habilitem uma lista predefinida de domínios de consumidores livres para bloquear formulários.

* **[Segurança de Cabeçalho de Página de Aterrissagem](/help/marketo/product-docs/administration/settings/landing-page-headers.md)**: os administradores podem gerenciar cabeçalhos de Segurança de Transporte Restrita e Opções de X-Frame em seus domínios de página de aterrissagem para aplicar requisitos de segurança rigorosos.

**_Liberando Durante o Trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Conector de destino do AEP Marketo Engage - Criar novos leads {#aep-marketo-engage-destination-connector}

Os clientes do Marketo Engage que também usam o Adobe Experience Platform (AEP) podem maximizar seu banco de dados com a capacidade de enviar registros de novas pessoas para o Marketo Engage a partir do AEP por meio do conector de destino do AEP. Ao enviar segmentos de público do AEP para o Marketo Engage, as pessoas dentro do segmento que ainda não existe no banco de dados do Marketo Engage [podem ser adicionadas automaticamente a ele](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/push-an-adobe-experience-platform-segment-to-a-marketo-static-list.md).

## [!DNL Sales Insight] {#sales-insight}

![(estrela)](assets/yellow-star.png)

**[!DNL Sales Insight]para [!DNL Salesforce] CRM**

* **Nova Coluna de Tipo para [!UICONTROL Melhores Opções]**: os vendedores obterão insights mais rápidos com uma nova coluna denominada &quot;Tipo&quot; para diferenciar clientes potenciais e contatos na página [!UICONTROL Melhores Opções].

* **[!DNL Salesforce]Atualização da API da Plataforma**: Em resposta à [!DNL Salesforce] desativação das versões 21.0 a 30.0 da API da Plataforma [!DNL Salesforce], o pacote [!DNL Sales Insight] foi atualizado com as APIs mais recentes.

* **Marca Atualizada**: todas as [!DNL Sales Insight] páginas estão sendo atualizadas para se alinharem à marca da Adobe.

**[!DNL Sales Insight]para[!DNL Microsoft Dynamics]**

* **Layout de conta atualizado**: os vendedores podem obter uma visão coletiva das principais atividades, como atividades de email, atividades da Web, momentos interessantes e alterações de pontuação para todos os contatos em uma conta.

## [!DNL Sales Connect] {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **Resultados e Motivos de Chamadas**: compreenda e rastreie com mais detalhes os esforços de saída de suas equipes de vendas com resultados de chamadas e opções de motivo de chamadas novas e totalmente personalizáveis. Além desses novos campos, estamos introduzindo uma nova governança para impor a seleção do motivo da chamada e do resultado enquanto os vendedores fazem chamadas, uma nova governança para habilitar ou desabilitar os motivos e resultados da chamada e um novo campo personalizado Motivo da Chamada e Resultado da Chamada [!DNL Salesforce] Atividade para registrar dados em [!DNL Salesforce]. [Clique aqui](https://nation.marketo.com/t5/product-blogs/sales-connect-enhancements-to-call-outcomes-q1-22-release/ba-p/319812) para saber mais.

* Personalização do Detalhe da Atividade **[!DNL Salesforce]**: capture mais dados da atividade de vendas e da tarefa em [!DNL Salesforce] personalizando quais informações são adicionadas ao campo de assunto da tarefa [!DNL Salesforce] quando uma atividade de vendas é registrada em [!DNL Salesforce] de [!DNL Sales Connect]. [Clique aqui](https://nation.marketo.com/t5/product-blogs/sales-connect-enahncements-to-activity-logging-to-salesforce-q1/ba-p/319819) para saber mais.

## Anúncios {#announcements}

* **Descontinuação do Marketo Sky**: em março, o Marketo Sky não estará mais disponível, pois concentraremos nossos recursos no fornecimento da experiência de usuário da próxima geração. Em um esforço para manter o acesso a uma funcionalidade exclusiva do Marketo Sky hoje, estamos trazendo a Expiração de ativos e a Substituição de prioridade da Campanha inteligente para a experiência principal em março. [Clique aqui](https://nation.marketo.com/t5/the-modern-ux/marketo-sky-deprecation-notice/ba-p/320115#M33) para saber mais.

* **Descontinuação de Pontos de Extremidade de Formulário**: as POSTs de formulário programático sem suporte para o ponto de extremidade leadCapture/save2 serão rejeitadas pelos Marketo Engage Forms. [Clique aqui](https://nation.marketo.com/t5/product-documents/updated-october-2021-upcoming-changes-to-the-marketo-engage-form/ta-p/306631) para saber mais.

* **Logon na Caixa de Diálogo Convidar Usuário**: em março, o recurso opcional existente &quot;Logon na Caixa de Diálogo Convidar Usuário&quot; será descontinuado. O recurso &quot;[!UICONTROL Logon na Caixa de Diálogo de Usuário Convidar]&quot; foi substituído pelo recurso de Universal ID, que é necessário para a futura Integração do Sistema do Adobe Identity Management e foi habilitado em agosto de 2021 em todas as assinaturas. Como resultado da desativação, o Marketo Engage aplicará somente um usuário a ser associado por endereço de email em uma assinatura.

**Domínios Marketo Engage - [!DNL Sales Insight] Configuração**: para domínios Marketo Engage que não têm certificado SSL provisionado e https://, as chamadas falharão com um erro de handshake SSL. Portanto, esses domínios serão encerrados. Como resultado, [!DNL Sales Insight] usuários com uma configuração mais antiga apontando para qualquer um desses domínios podem encontrar erros de texto explicativo do sistema nas páginas de cliente potencial, contato, conta, painéis de oportunidade ou global da Marketo. Recomendamos que você atualize sua [configuração do Marketo Engage](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) em [!DNL Salesforce] se encontrar esse erro. Você só precisa atualizar as credenciais do Marketo Engage realçadas na seção &quot;[!DNL Marketo Sales Insight] Config&quot; do documento.

**_Webinar de lançamento de produto_**

[Webinário da versão de janeiro de 2022 do Marketo Engage](https://engage.marketo.com/2022_January_Release_Webinar_DemandPage.html)
