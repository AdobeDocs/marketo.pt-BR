---
description: Adicionar acesso do Sales Insight aos perfis - Documentação do Marketo - Documentação do produto
title: Adicionar Acesso ao Sales Insight aos Perfis
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 4%

---

# Adicionar [!DNL Sales Insight] Acesso a Perfis {#add-sales-insight-access-to-profiles}

Veja como criar um perfil com acesso ao [!DNL Sales Insight] ao remover o acesso de outros perfis. Isso é para usuários que já instalaram o [[!DNL Sales Insight] pacote do AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Se você já tiver concedido acesso de [!DNL Sales Insight] a todos os perfis, deverá [remover o acesso em nível de perfil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} para usar este conjunto de permissões.

## Criar um Novo Perfil para [!DNL Sales Insight] {#create-a-new-profile-for-sales-insight}

Se você tiver um perfil dedicado para os usuários do [!DNL Sales Insight], ignore esta etapa.

1. Em [!DNL Salesforce], vá para a página Configuração.

1. Procure perfis na Localização Rápida e selecione a opção **[!UICONTROL Perfil]**.

1. Clique no botão **[!UICONTROL Novo Perfil]** na parte superior da página.

1. Escolha um perfil para clonar e dê um nome a ele (por exemplo: Usuário do Sales Insight).

1. Clique em **[!UICONTROL Salvar]** quando terminar.

## Adicionar [!DNL Sales Insight] Permissões {#add-sales-insight-permissions}

1. Volte para a sua Lista de perfis.

1. Clique no link **[!UICONTROL Editar]** para o novo perfil recém-criado (ou qualquer outro perfil existente ao qual você deseja conceder acesso de [!DNL Sales Insight]).

1. Na página de edição, será necessário alterar algumas configurações.

   **Para perfis com acesso permitido[!DNL Sales Insight]**:

   * Em Configurações da guia, altere as guias do Marketo para Padrão Ativado
   * Nas Permissões de objeto personalizado, marque Ler, Criar, Editar e Excluir na Configuração do [!DNL Marketo Sales Insight] (se o usuário precisar ter acesso às configurações - normalmente usadas para administradores)

   **Para perfis que não têm permissão para acessar[!DNL Sales Insight]**:

   * Em Configurações da guia, altere as guias do Marketo para Guia oculta
   * Nas Permissões de Objeto Personalizado, desmarque Ler, Criar, Editar, e Excluir na Configuração [!DNL Marketo Sales Insight]

1. Clique em **[!UICONTROL Salvar]** quando terminar.

## Criar Layout para [!DNL Sales Insight] {#create-layout-for-sales-insight}

1. Vá para a página Instalação e clique em **[!UICONTROL Instalação do aplicativo]** > **[!UICONTROL Personalizar]** > **[!UICONTROL Clientes potenciais]** > **[!UICONTROL Layouts de página]**. Clique no botão **[!UICONTROL Novo]**.

1. Clonar seu layout de escolha e dar ao layout um nome apropriado (por exemplo: Layout de Insight de Vendas).

1. Clique em **[!UICONTROL Salvar]** quando terminar.

1. Repita essas etapas para os layouts de página de [!UICONTROL Contatos], [!UICONTROL Oportunidades] e [!UICONTROL Contas]&#39;.

## Atribuir perfil ao layout {#assign-profile-to-layout}

1. Volte para a seção Layouts de página e clique no botão **[!UICONTROL Atribuição de layout de página]**.

1. Selecione **[!UICONTROL Editar atribuição]**.

1. Selecione o perfil [!DNL Sales Insight] na lista e o layout [!DNL Sales insight] na lista suspensa &quot;[!UICONTROL Selecionar layout da página]&quot;.

1. Clique em **[!UICONTROL Salvar]** quando terminar.

1. Repita essas etapas para os layouts de página de [!UICONTROL Contatos], [!UICONTROL Oportunidades] e [!UICONTROL Contas]&#39;.

## Outras alterações {#other-changes}

Aqui estão alguns outros locais onde [!DNL Sales Insight] itens podem aparecer. Você terá que removê-los completamente, já que não pode usar Perfis para limitar o acesso deles:

* Remover botões [!DNL Sales Insight] dos Layouts de Pesquisa para [!UICONTROL Contatos], [!UICONTROL Clientes Potenciais] e [!UICONTROL Contas]
* Remover [!DNL Sales Insight] colunas das listas de contatos e clientes potenciais
