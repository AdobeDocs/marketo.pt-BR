---
title: Trabalho com o Experience Manager Assets
description: Saiba como você pode usar ativos de imagem de um repositório conectado do AEM Assets ao criar conteúdo no Adobe Marketo Engage.
hide: true
hidefromtoc: true
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# Trabalhar com ativos do Experience Manager

Quando o Adobe Experience Manager Assets as a Cloud Service é integrado ao Adobe Marketo Engage, você pode descobrir e acessar facilmente ativos digitais para uso em seu conteúdo de marketing. À medida que você cria seu conteúdo, os ativos podem ser acessados a partir do item _[!UICONTROL Assets]_ na navegação à esquerda e ao criar conteúdo de email para uma jornada de conta. Também é possível fazer upload de ativos para o repositório as a Cloud Service conectado do AEM Assets diretamente do Adobe Journey Optimizer B2B edition.

>[!NOTE]
>
>Atualmente, somente os ativos de imagem do Adobe Experience Manager Assets são compatíveis com o Adobe Journey Optimizer B2B edition. As alterações nos ativos devem ser feitas pelo repositório central da Adobe Experience Manager Assets. [Saiba mais](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/manage-digital-assets)

Quando você usa esses ativos digitais, as alterações mais recentes no Assets as a Cloud Service se propagam automaticamente para campanhas de email ao vivo por meio de referências vinculadas. Se as imagens forem excluídas no Adobe Experience Manager Assets as a Cloud Service, elas serão exibidas com uma referência quebrada nos emails. Quando os ativos atualmente usados nas jornadas da conta são modificados ou excluídos, os autores da jornada são notificados sobre as alterações na imagem e a lista de jornadas que usam a imagem. Todas as alterações nos ativos devem ser feitas no repositório central da Adobe Experience Manager Assets.

## Usar o AEM Assets como fonte de imagem

Se o ambiente tiver uma ou mais conexões de repositórios Assets, você poderá designar o AEM Assets como fonte para ativos ao criar ou exibir detalhes de um email, modelo de email ou fragmento visual.

* Ao criar um novo conteúdo, escolha `AEM Assets` como o item **[!UICONTROL Image Source]** na caixa de diálogo.

CAPTURA DE TELA

* Ao abrir um recurso de conteúdo existente, escolha `AEM Assets` no painel _[!UICONTROL Corpo]_ à direita.

CAPTURA DE TELA

## Acessar ativos para criação

>[!IMPORTANT]
>
>Um administrador deve adicionar usuários que precisam de acesso ao Assets aos perfis do produto Usuários do cliente do Assets e/ou Usuários do Assets. [Saiba mais](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/security/ims-support#managing-products-and-user-access-in-admin-console)

No editor de conteúdo visual, clique no ícone _Seletor de ativos_ na barra lateral esquerda. Isso altera o painel Ferramentas para uma lista de ativos disponíveis no repositório selecionado.

CAPTURA DE TELA

Se você tiver mais de um repositório AEM conectado, clique na seta de menu de **[!UICONTROL Repositório]** para escolher o repositório que deseja usar.

CAPTURA DE TELA

Há vários métodos para adicionar um ativo de imagem à tela visual:

* Arraste e solte uma miniatura de imagem da navegação à esquerda.

CAPTURA DE TELA

* Adicione um componente de imagem à tela e clique em **[!UICONTROL Procurar]** para abrir a caixa de diálogo _[!UICONTROL Selecionar Assets]_.

  Na caixa de diálogo, é possível escolher uma imagem do repositório selecionado.

  Há várias ferramentas disponíveis para ajudá-lo a localizar o ativo que você precisa.

CAPTURA DE TELA

* Altere o **[!UICONTROL Repositório]** na parte superior direita.

* Clique em **[!UICONTROL Gerenciar ativos]** na parte superior direita para abrir o repositório do Assets em outra guia do navegador e usar as ferramentas de gerenciamento do AEM Assets.

* Clique no seletor de _Tipo de exibição_ na parte superior direita para alterar a exibição para **[!UICONTROL Exibição de Lista]**, **[!UICONTROL Exibição de Grade]**, **[!UICONTROL Exibição de Galeria]** ou **[!UICONTROL Exibição em Cascata]**.

* Clique no ícone _Ordem de classificação_ para alterar a ordem de classificação entre crescente e decrescente.

* Clique na seta de menu **[!UICONTROL Classificar por]** para alterar os critérios de classificação para **[!UICONTROL Nome]**, **[!UICONTROL Tamanho]** ou **[!UICONTROL Modificado]**.

* Clique no ícone _Filtro_ na parte superior esquerda para filtrar os itens exibidos de acordo com seus critérios.

* Insira texto no campo Pesquisar para filtrar os itens exibidos para uma correspondência do nome do ativo.

CAPTURA DE TELA
