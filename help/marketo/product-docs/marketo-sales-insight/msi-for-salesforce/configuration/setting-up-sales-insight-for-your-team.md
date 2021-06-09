---
description: Configuração do insight de vendas para sua equipe - Documentos da Marketo - Documentação do produto
title: Configuração do insight de vendas para sua equipe
exl-id: 269f9093-f530-4e3b-aac7-e317976cf0f0
source-git-commit: ecceb1a3aff3a2088379f8f4f2ac33e566f90e21
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Configuração do insight de vendas para sua equipe {#setting-up-sales-insight-for-your-team}

Veja como criar um perfil com acesso ao Sales Insight e remover o acesso de outros perfis. Isso é para usuários que já instalaram o [pacote de AppExchange do Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md).

## Criar um novo perfil para o Sales Insight {#create-a-new-profile-for-sales-insight}

Se você tiver um perfil dedicado para seus usuários do Sales Insight, ignore esta etapa.

1. No Salesforce, acesse a página Configuração.

1. Procure perfis em Localização rápida e selecione a opção **Perfil**.

1. Clique no botão **Novo perfil** na parte superior da página.

1. Escolha um perfil para clonar e dê um nome a ele (por exemplo: Usuário do Sales Insight).

1. Clique em **Salvar** quando terminar.

## Adicionar permissões de insight de vendas {#add-sales-insight-permissions}

1. Volte para a lista Perfis.

1. Clique no link **Edit** para o novo perfil que você acabou de criar (ou em qualquer outro perfil existente ao qual você deseja conceder acesso ao Sales Insight).

1. Na página de edição, será necessário alterar algumas configurações.

   **Para perfis com permissão de acesso ao Sales Insight**:

   * Em Configurações da guia, altere as guias Marketo para Padrão ativado
   * Em Permissões de objeto personalizado, marque a opção Ler, Criar, Editar e Excluir na Configuração do Marketo Sales Insight (se o usuário precisar ter acesso às configurações - normalmente usadas para administradores)

   **Para perfis que não têm acesso ao Sales Insight**:

   * Em Configurações da guia, altere as guias Marketo para Guia Oculto
   * Em Permissões de objeto personalizado, desmarque Ler, Criar, Editar e Excluir na Configuração do Marketo Sales Insight


1. Clique em **Salvar** quando terminar.

## Criar layout para o Insight de vendas {#create-layout-for-sales-insight}

1. Vá para a página Configuração e clique em **Configuração do Aplicativo** > **Personalizar** > **Leads** > **Esquemas de Página**. Em seguida, clique no botão **New**.

1. Clona o layout escolhido e dê um nome apropriado ao layout (por exemplo: Layout de insight de vendas).

1. Clique em **Salvar** quando terminar.

1. Repita essas etapas para os layouts da página Contatos, Oportunidades e Contas.

## Atribuir perfil ao layout {#assign-profile-to-layout}

1. Volte para a seção Layouts de página e clique no botão **Atribuição de layout de página** .

1. Selecione **Editar Atribuição**.

1. Selecione o seu perfil Sales Insight na lista e, em seguida, selecione o seu layout Sales Insight no menu suspenso &quot;Select Page Layout&quot;.

1. Clique em **Salvar** quando terminar.

1. Repita essas etapas para os layouts da página Contatos, Oportunidades e Contas.

## Outras alterações {#other-changes}

Aqui estão alguns outros lugares onde os itens de Insight de vendas podem aparecer. Você terá que removê-los imediatamente, já que não pode usar Perfis para limitar o acesso:

* Remover botões de insight de vendas de layouts de pesquisa para contatos, clientes potenciais e contas
* Remover colunas de informações de vendas das listas de contatos e clientes potenciais
