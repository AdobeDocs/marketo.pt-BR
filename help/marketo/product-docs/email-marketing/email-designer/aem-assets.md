---
title: Trabalho com o Experience Manager Assets
description: Saiba como usar ativos de imagem de um repositório conectado do AEM Assets ao criar conteúdo no Adobe Marketo Engage.
level: Beginner, Intermediate
feature: Email Designer
exl-id: c2172042-a35c-4179-bf81-6e96323bd4d4
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 1%

---

# Trabalhar com ativos da Experience Manager {#work-with-experience-manager-assets}

Conecte sua conta do _Adobe Experience Manager Assets as a Cloud Service_ à sua instância do Adobe Marketo Engage para que você possa aproveitar seu repositório do AEM Asset no Marketo Engage Email Designer.

>[!NOTE]
>
>Atualmente, apenas ativos de imagem do _Adobe Experience Manager Assets_ são suportados no Marketo Engage. As alterações nos ativos devem ser feitas pelo repositório central da Adobe Experience Manager Assets. [Saiba mais](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets){target="_blank"}

## Link para os serviços em nuvem da AEM {#link-to-your-aem-cloud-services}

Antes de usar esse recurso, primeiro vincule o AEM Cloud Services ao Adobe Marketo Engage.

+++Vincular serviços em nuvem da AEM e Marketo Engage

>[!NOTE]
>
>**Permissões de administrador necessárias**

1. No Marketo Engage, vá para a área **Admin** e selecione **Adobe Experience Manager** na árvore de navegação esquerda.

   ![Selecione o Adobe Experience Manager na seção de Administrador](assets/access-the-ai-assistant-content-accelerator-1.png){width="800" zoomable="yes"}

1. Clique em **Editar** ao lado de _Adobe Experience Manager Cloud Services_.

   ![Clique em EDITAR](assets/access-the-ai-assistant-content-accelerator-2.png){width="400" zoomable="yes"}

1. Selecione um ou mais repositórios.

   ![Selecione um repositório](assets/access-the-ai-assistant-content-accelerator-3.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >* Somente repositórios que foram associados na mesma organização IMS que sua assinatura do Marketo Engage são listados.
   >
   >* O Marketo Engage só oferece suporte a repositórios do nível de Delivery. Se você usa a camada Autor e deseja convertê-la, contate o [Suporte da Adobe Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-manager/content/overview/help-resources).

1. Você deve adicionar um [certificado de credencial de serviço](https://experienceleague.adobe.com/pt-br/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) para configurar o repositório. Clique no botão **+ Adicionar certificado**.

   ![Adicionar um certificado](assets/access-the-ai-assistant-content-accelerator-4.png){width="800" zoomable="yes"}

1. Arraste e solte o certificado (somente arquivo JSON) ou selecione-o no computador. Clique em **Adicionar** quando terminar.

   ![Localize o certificado no computador](assets/access-the-ai-assistant-content-accelerator-5.png){width="600" zoomable="yes"}

1. O repositório configurado é exibido abaixo, juntamente com o status e a expiração. Clique no botão de reticências (**...**) para exibir o certificado. Caso contrário, você está pronto.

   ![O certificado foi adicionado](assets/access-the-ai-assistant-content-accelerator-6.png){width="700" zoomable="yes"}

Agora, todas as imagens da biblioteca de gerenciamento de ativos digitais nesse repositório podem ser acessadas no Marketo Engage Email Designer.

+++

## Trabalhar com ativos do AEM {#working-with-aem-assets}

Quando você usa esses ativos digitais, as alterações mais recentes no _Assets as a Cloud Service_ propagam-se automaticamente para campanhas de email em tempo real por meio de referências vinculadas. Se as imagens forem excluídas no _Adobe Experience Manager Assets as a Cloud Service_, elas serão exibidas com uma referência corrompida em seus emails. Quando os ativos que estão sendo usados no momento no Marketo Engage são modificados ou excluídos, os autores de email são notificados sobre as alterações na imagem. Todas as alterações nos ativos devem ser feitas no repositório central da Adobe Experience Manager Assets.

### Usar o AEM Assets como fonte de imagem {#use-aem-assets-as-the-image-source}

Se o ambiente tiver uma ou mais conexões do repositório de ativos, você poderá designar o AEM Assets como fonte para ativos ao criar ou exibir detalhes de um email, modelo de email ou fragmento visual.

* Ao criar novo conteúdo, escolha `AEM Assets` como o item **[!UICONTROL Image Source]** na caixa de diálogo.

![Selecione AEM Assets como a fonte da imagem na caixa de diálogo de criação](assets/work-with-experience-manager-assets-1.png){width="400" zoomable="yes"}

* Ao abrir um recurso de conteúdo existente, escolha `AEM Assets` na seção _[!UICONTROL Corpo]_ à direita.

![Selecione o AEM Assets como fonte de imagem nas propriedades](assets/work-with-experience-manager-assets-2.png){width="700" zoomable="yes"}

### Acessar ativos para criação {#access-assets-for-authoring}

>[!IMPORTANT]
>
>Um administrador deve adicionar usuários que precisam de acesso aos ativos aos perfis do produto Usuários do consumidor do Assets e/ou Usuários do Assets. [Saiba mais](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

No editor de conteúdo visual, clique no ícone _Seletor de ativos do Experience Manager_ na barra lateral esquerda. Isso altera o painel Ferramentas para uma lista de ativos disponíveis no repositório selecionado.

![Clique no ícone do seletor do Assets para acessar os ativos da imagem](assets/work-with-experience-manager-assets-3.png){width="700" zoomable="yes"}

Se você tiver mais de um repositório AEM conectado, clique no botão **[!UICONTROL Gerenciar como]** para escolher o repositório que deseja usar.

![Escolha um repositório do AEM Assets para acessar os ativos da imagem](assets/work-with-experience-manager-assets-4.png){width="700" zoomable="yes"}

Escolha o repositório desejado.

![Escolha um repositório do AEM Assets para acessar os ativos da imagem](assets/work-with-experience-manager-assets-5.png){width="500" zoomable="yes"}

Há vários métodos para adicionar um ativo de imagem à tela visual:

* Arraste e solte uma miniatura de imagem da navegação à esquerda.

![Escolha um repositório do AEM Assets para acessar os ativos da imagem](assets/work-with-experience-manager-assets-6.png){width="700" zoomable="yes"}

* Adicione um componente de imagem à tela e clique em **[!UICONTROL Procurar]** para abrir a caixa de diálogo _[!UICONTROL Selecionar Assets]_.

  Na caixa de diálogo, é possível escolher uma imagem do repositório selecionado.

  Há várias ferramentas disponíveis para ajudá-lo a localizar o ativo que você precisa.

![Use a ferramenta na caixa de diálogo Selecionar Assets para localizar e selecionar um ativo de imagem](assets/work-with-experience-manager-assets-7.png){width="700" zoomable="yes"}

* Altere o **[!UICONTROL Repositório]** na parte superior direita.

* Clique em **[!UICONTROL Gerenciar ativos]** na parte superior direita para abrir o repositório do Assets em outra guia do navegador e usar as ferramentas de gerenciamento do AEM Assets.

* Clique no seletor de _Tipo de exibição_ na parte superior direita para alterar a exibição para **[!UICONTROL Exibição de Lista]**, **[!UICONTROL Exibição de Grade]**, **[!UICONTROL Exibição de Galeria]** ou **[!UICONTROL Exibição em Cascata]**.

* Clique no ícone _Ordem de classificação_ para alterar a ordem de classificação entre crescente e decrescente.

* Clique na seta de menu **[!UICONTROL Classificar por]** para alterar os critérios de classificação para **[!UICONTROL Nome]**, **[!UICONTROL Tamanho]** ou **[!UICONTROL Modificado]**.

* Clique no ícone _Filtro_ na parte superior esquerda para filtrar os itens exibidos de acordo com seus critérios.

* Insira texto no campo Pesquisar para filtrar os itens exibidos para uma correspondência do nome do ativo.

![Use os filtros e o campo de pesquisa para localizar o ativo](assets/work-with-experience-manager-assets-8.png){width="700" zoomable="yes"}
