---
unique-page-id: 2360368
description: Saiba como configurar o Marketo Sales Insight nas edições Salesforce Enterprise/Unlimited.
title: Configurar o Insight de vendas do Marketo no Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: 95dda7d6e09f0e64fbce8e5bd39613f10ebde382
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 5%

---

# Configurar o [!DNL Marketo Sales Insight] no [!DNL Salesforce] Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Configure o Marketo Sales Insight no Salesforce Enterprise/Unlimited editions seguindo as etapas abaixo.

>[!PREREQUISITES]
>
>[Instalar [!DNL Marketo Sales Insight] Pacote no [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Permissões de administrador são necessárias.**

## Configurar o Sales Insight no Marketo Engage {#configure-sales-insight-in-marketo}

1. Para obter suas credenciais do Marketo Sales Insight no Marketo Engage, vá para a área **[!UICONTROL Administrador]** e selecione **[!UICONTROL Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Clique em **[!UICONTROL Editar Configuração de API]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Insira uma chave secreta de API de sua escolha e clique em **[!UICONTROL Salvar]**. NÃO use um E comercial (`&`) na chave secreta da API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >Sua chave secreta de API é como uma senha para sua organização e deve ser segura.

1. Para preencher as credenciais, clique em **[!UICONTROL Exibir]** no painel _[!UICONTROL Configuração da API Rest]_.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Quando você vir uma caixa de diálogo de confirmação, clique em **[!UICONTROL OK]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Mantenha essa janela aberta. Essas informações serão necessárias posteriormente para a configuração do Salesforce.

## Preencher novas credenciais da API Rest {#populate-new-rest-api-credentials}

1. Ao preencher as credenciais da API Rest pela primeira vez, o botão _Exibir_ será alterado para _Editar_. Clique no botão **Editar**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5a.png)

1. Uma mensagem é exibida confirmando que você deseja regenerar as credenciais da API. Clique em **Salvar**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5b.png){width="800" zoomable="yes"}

1. Depois que as novas credenciais forem preenchidas, atualize-as na guia _Configuração do Marketo_ da sua instância do Salesforce.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5c.png)

## Configurar [!DNL Sales Insight] em [!DNL Salesforce] {#configure-sales-insight-in-salesforce}

1. No Salesforce, clique em **[!UICONTROL Instalação]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Procure por &quot;site remoto&quot; e selecione **[!UICONTROL Configurações do Site Remoto]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Clique em **[!UICONTROL Novo Site Remoto]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Insira o Nome do Site Remoto (pode ser algo semelhante a `MarketoSoapAPI`). Insira a URL do Site Remoto, que é a sua URL do Marketo Host no painel _[!UICONTROL Configuração da API Soap]_ no Marketo Engage. Clique em **[!UICONTROL Salvar]**. Agora você criou configurações de site remoto para a API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Clique novamente em **[!UICONTROL Novo Site Remoto]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Insira o Nome do Site Remoto (pode ser algo semelhante a `MarketoAPI`). Insira o URL do Site Remoto, que é o URL da API no painel _[!UICONTROL Configuração da API Rest]_ no Marketo Engage. Clique em **[!UICONTROL Salvar]**. Agora você criou configurações de site remoto para a API Rest.

   >[!NOTE]
   >
   >_Você_ escolhe seu **[!UICONTROL Nome do Site Remoto]** (`MarketoAPI` é usado aqui). A **[!UICONTROL URL do Site Remoto]** pode ser encontrada no campo Host do Marketo da caixa de diálogo Editar Configuração da API da Etapa 3 na seção &quot;Configurar Sales Insight no Marketo&quot;.

## Conceder acesso ao perfil de usuários do Sales Insight a objetos padrão do Salesforce {#grant-sales-insight-users-profile-access}

Devido aos aprimoramentos de segurança do Salesforce, os pacotes do AppExchange não podem mais conceder permissão a objetos padrão e o acesso deve ser concedido aos objetos relevantes do Salesforce no perfil do usuário do Salesforce. Para conceder as permissões necessárias, siga estas etapas.

1. Clique em **[!UICONTROL Instalação]**.

1. Pesquise &quot;Perfis&quot; em Localização rápida.

1. Clique em **[!UICONTROL Editar]** ao lado do perfil que seus usuários do Salesforce estão usando.

1. Na seção _[!UICONTROL Permissão de Objeto Padrão]_, habilite o acesso de **[!UICONTROL Leitura]** para os seguintes objetos: [!UICONTROL Cliente Potencial], [!UICONTROL Contato], [!UICONTROL Conta] e [!UICONTROL Oportunidade].

1. Clique em **[!UICONTROL Salvar]**.

## Personalizar layouts de página {#customize-page-layouts}

1. Clique em **[!UICONTROL Instalação]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Procure por &quot;layout de página&quot; e selecione o **[!UICONTROL Layout de Página]** em **[!UICONTROL Clientes potenciais]**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Clique em **[!UICONTROL Visualforce Pages]** à esquerda. Arraste **[!UICONTROL Seção]** para o layout abaixo da seção _[!UICONTROL Links Personalizados]_.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Insira &quot;Marketo Sales Insight&quot; como o **[!UICONTROL Nome da Seção]**, selecione **[!UICONTROL 1-Coluna]** e clique em **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arraste e solte **[!UICONTROL Lead]** na nova seção.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >O nome dessa caixa é alterado com base no tipo de objeto. Por exemplo, se você estiver modificando o layout de página para Contatos, ele exibirá Contato.

1. Clique duas vezes no bloco **[!UICONTROL Lead]** que você acabou de adicionar.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Edite a altura para **450** pixels e clique em **[!UICONTROL OK]**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Marque **[!UICONTROL Mostrar barras de rolagem]** se precisar de acesso para rolar pelas atividades.

   >[!TIP]
   >
   >A altura recomendada para os objetos Contas e Oportunidades é de 410 pixels.

1. Clique em **[!UICONTROL Campos]** à esquerda. Em seguida, pesquise e arraste o rótulo **[!UICONTROL Urgency]** para o layout **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Repita a etapa acima também para esses campos.

   * Último momento interessante
   * Data do último momento interessante
   * Desc. do último momento interessante
   * Fonte do último momento interessante
   * Tipo do último momento interessante
   * Última atividade por vendas
   * Último engajamento por vendas
   * ID de contato MSI
   * Pontuação relativa
   * Valor de pontuação relativa
   * Urgência
   * Valor de urgência
   * Exibir no Marketo

1. Clique em **[!UICONTROL Salvar]** quando terminar.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita as etapas de 5 a 7 para adicionar seções de página do Visualforce e campos do Sales Insight para **[!UICONTROL Contato]**, **[!UICONTROL Conta]** e **[!UICONTROL Oportunidade]**.

1. Repita as etapas 8 a 10 para adicionar esses campos do Sales Insight para **[!UICONTROL Contato]**. Certifique-se de salvar as alterações.

   * Último momento interessante
   * Data do último momento interessante
   * [!UICONTROL Última Descrição de Momento Interessante]
   * [!UICONTROL Último Source de Momento Interessante]
   * [!UICONTROL Último tipo de momento interessante]
   * [!UICONTROL Última Atividade do Marketo por Vendas]
   * [!UICONTROL Último contrato de vendas do Marketo]
   * [!UICONTROL Pontuação de lead MKTO]
   * [!UICONTROL Pontuação relativa]
   * [!UICONTROL Valor de Pontuação Relativo]
   * [!UICONTROL Sales Insight] - Abre a página da lista completa de contatos
   * [!UICONTROL Urgência]
   * [!UICONTROL Valor de Urgência]

## Mapear campos de pessoa personalizados {#map-custom-person-fields}

Os campos de pessoa do Marketo devem ser mapeados para campos de contato do Salesforce para garantir que a conversão funcione corretamente. Siga estas etapas para mapeá-las.

1. Clique em **[!UICONTROL Instalação]**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Pesquise por &quot;campos&quot; na barra de pesquisa e clique em **[!UICONTROL Campos]** em **[!UICONTROL Clientes potenciais]**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Clique em **[!UICONTROL Mapear campos de cliente em potencial]**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Clique na lista suspensa à direita de **[!UICONTROL Envolvimento]**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Selecione **[!UICONTROL Contact.Engagement]** na lista.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Repita e mapeie esses campos também.

   | Campo personalizado da pessoa do Marketo | Campo personalizado do contato da Salesforce |
   |--- |--- |
   | `Engagement` | `Contact.Engagement` |
   | `Relative Score Value` | `Contact.Relative Score Value` |
   | `Urgency Value` | `Contact.Urgency Value` |
   | `Last Interesting Moment Date` | `Contact.Last Interesting Moment Date` |
   | `Last Interesting Moment Desc` | `Contact.Last Interesting Moment Desc` |
   | `Last Interesting Moment Source` | `Contact.Last Interesting Moment Source` |
   | `Last Interesting Moment Type` | `Contact.Last Interesting Moment Type` |

1. Clique em **[!UICONTROL Salvar]** quando terminar.

## Guia de configuração do Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. No Salesforce, clique em **+** no final da barra de guias e clique em **[!UICONTROL Configuração do Marketo Sales Insight]**.

1. Copie as credenciais do painel API Soap na [página de Administração do Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e cole-as na seção API Soap da página de Configuração [!DNL Salesforce] [!DNL Sales Insight].

1. Copie as credenciais do painel API Rest na [página Administrador do Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e cole-as na seção API Rest da página Configuração [!DNL Salesforce] [!DNL Sales Insight].

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

Você poderá ver os campos do Marketo Sales Insight para clientes potenciais, contatos, contas e oportunidades.

>[!NOTE]
>
>Se o teste de diagnóstico falhar, [adicionar mais campos ao layout de página](https://nation.marketo.com:443/t5/knowledgebase/how-to-repair-marketo-sales-insight-setup-configuration-problems/ta-p/248218){target="_blank"} poderá corrigir o problema.

>[!NOTE]
>
>Para contas do, o Sales Insight inclui todos os emails, mas somente os momentos interessantes mais recentes, a atividade da Web e as alterações de pontuação.

>[!MORELIKETHIS]
>
>* [Prioridade, Urgência, Pontuação Relativa e Melhores Opções](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Adicionar a guia Marketo a [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Adicionar Acesso do Sales Insight aos Perfis](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
