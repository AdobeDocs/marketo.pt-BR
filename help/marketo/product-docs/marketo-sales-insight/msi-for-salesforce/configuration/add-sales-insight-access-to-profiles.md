---
description: Adicionar acesso ao Sales Insight aos perfis - Documentação do Marketo - Documentação do produto
title: Adicionar acesso ao Sales Insight aos perfis
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 3%

---

# Adicionar acesso ao Sales Insight aos perfis {#add-sales-insight-access-to-profiles}

Veja como criar um perfil com acesso ao Sales Insight e remover o acesso de outros perfis. Isso é para usuários que já instalaram o [pacote de AppExchanges do Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.

>[!IMPORTANT]
>
>Se você já tiver concedido acesso ao Sales Insight a todos os perfis, deverá [remover o acesso em nível de perfil](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/remove-sales-insight-access.md){target="_blank"} para usar este conjunto de permissões.

## Criar um novo perfil para o Sales Insight {#create-a-new-profile-for-sales-insight}

Se você tiver um perfil dedicado para seus usuários do Sales Insight, ignore esta etapa.

1. No Salesforce, acesse a página Configuração.

1. Procure perfis na Localização Rápida e selecione a opção **Perfil**.

1. Clique no botão **Novo Perfil** na parte superior da página.

1. Escolha um perfil para clonar e dê um nome a ele (por exemplo: Usuário do Sales Insight).

1. Clique em **Salvar** quando terminar.

## Adicionar permissões de insight de vendas {#add-sales-insight-permissions}

1. Volte para a sua Lista de perfis.

1. Clique no link **Editar** para o novo perfil recém-criado (ou qualquer outro perfil existente ao qual você deseja conceder acesso ao Sales Insight).

1. Na página de edição, será necessário alterar algumas configurações.

   **Para perfis que têm acesso permitido ao Sales Insight**:

   * Em Configurações da guia, altere as guias do Marketo para Padrão Ativado
   * Em Permissões de objeto personalizado, marque Ler, Criar, Editar e Excluir na configuração do Marketo Sales Insight (se o usuário precisar ter acesso às configurações - normalmente usadas para administradores)

   **Para perfis que não têm acesso ao Sales Insight**:

   * Em Configurações da guia, altere as guias do Marketo para Guia oculta
   * Em Permissões de objeto personalizado, desmarque Ler, Criar, Editar e Excluir na configuração do Marketo Sales Insight

1. Clique em **Salvar** quando terminar.

## Criar layout para insights de vendas {#create-layout-for-sales-insight}

1. Vá para a página Instalação e clique em **Instalação do aplicativo** > **Personalizar** > **Clientes potenciais** > **Layouts de página**. Clique no botão **Novo**.

1. Clonar o layout de escolha e dar ao layout um nome apropriado (por exemplo: Layout de insight de vendas).

1. Clique em **Salvar** quando terminar.

1. Repita essas etapas para os layouts de página de Contatos, Oportunidades e Contas.

## Atribuir perfil ao layout {#assign-profile-to-layout}

1. Volte para a seção Layouts de página e clique no botão **Atribuição de layout de página**.

1. Selecione **Editar atribuição**.

1. Selecione o perfil Sales Insight na lista e, em seguida, selecione o layout Sales insight na lista suspensa &quot;Select Page Layout&quot;.

1. Clique em **Salvar** quando terminar.

1. Repita essas etapas para os layouts de página de Contatos, Oportunidades e Contas.

## Outras alterações {#other-changes}

Estes são alguns outros locais onde os itens do Sales Insight podem aparecer. Você terá que removê-los completamente, já que não pode usar Perfis para limitar o acesso deles:

* Remover botões de Insight de vendas de Layouts de pesquisa para contatos, clientes potenciais e contas
* Remover colunas de Insight de vendas das listas de contatos e clientes potenciais
