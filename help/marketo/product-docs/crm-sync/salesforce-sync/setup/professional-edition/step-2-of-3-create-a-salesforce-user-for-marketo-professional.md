---
unique-page-id: 3571797
description: Etapa 2 de 3 - Criar um usuário do Salesforce para o Marketing (Professional) - Documentação do produto - Documentação do produto
title: Etapa 2 de 3 - Criar um usuário do Salesforce para o Marketing (Professional)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---


# Etapa 2 de 3: Criar um usuário do Salesforce para o Marketing (Professional) {#step-of-create-a-salesforce-user-for-marketo-professional}

>[!NOTE]
>
>Essas etapas devem ser concluídas por um administrador do Salesforce

>[!PREREQUISITES]
>
>[Etapa 1 de 3: Adicionar campos de marketing ao Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)

Neste artigo, você personalizará as permissões de campo com um Layout de página do Salesforce e criará um usuário de sincronização do Marketo-Salesforce.

## Definir layouts de página {#set-page-layouts}

O Salesforce Professional define a acessibilidade no nível do campo com Layouts de página, em vez dos Perfis do Salesforce Enterprise/Unlimited. Estas etapas permitirão que o usuário de sincronização de marketing atualize os campos personalizados.

1. Digite **layouts de página** na barra de pesquisa Navegação sem pressionar **Enter** e clique em **Layout de página** em **Leads**.

   ![](assets/image2016-2-26-12-3a58-3a32.png)

1. Clique em **Editar** ao lado de Layout principal.

   ![](assets/image2016-2-26-13-3a2-3a46.png)

1. Clique e arraste uma nova **Seção** para o layout da página.

   ![](assets/image2014-12-9-12-3a56-3a40.png)

1. Digite &quot;Marketo&quot; para **Nome da seção** e clique em **OK**.

   ![](assets/image2014-12-9-12-3a56-3a52.png)

1. Clique e arraste o campo **Data de aquisição** para a seção **Marketing**.

   ![](assets/image2014-12-9-12-3a57-3a0.png)

1. Repita a etapa acima para os seguintes campos:

   * Programa de aquisição
   * ID do Programa de aquisição
   * Opt out de email
   * Cidade Inferida
   * Empresa inferida
   * País Inferior
   * Área metropolitana inferida
   * Código de área do telefone inferior
   * Código postal inferido
   * Região do Estado Inferior
   * Pontuação principal
   * Quem indicou original
   * Mecanismo de pesquisa original
   * Frase de pesquisa original
   * Informações de origem originais
   * Tipo de origem original

   >[!NOTE]
   >
   >Esses campos precisam estar no layout da página para que o Marketo possa ler/gravar neles.

   >[!TIP]
   >
   >Crie duas colunas para os campos arrastando para baixo até o lado direito da página. É possível mover os campos de um lado para o outro para equilibrar as comprimentos das colunas.

1. Clique em **Salvar** ao terminar de adicionar campos.

   ![](assets/image2014-12-9-12-3a57-3a10.png)

1. Repita todas as etapas acima para o Salesforce **Contact Page Layout**.

   ![](assets/image2016-2-26-13-3a10-3a1.png)

1. Lembre-se de clicar em **Salvar** quando terminar com o **Layout de página de contato**.

   ![](assets/image2014-12-9-12-3a57-3a30.png)

   >[!NOTE]
   >
   >Certifique-se de que o campo **Evento de todos os dias** foi adicionado ao **Layout de página do Evento**.

## Criar usuário de sincronização {#create-sync-user}

O Marketo requer credenciais para acessar o Salesforce. Isso é feito melhor com um usuário dedicado criado com as etapas abaixo.

>[!NOTE]
>
>Se sua organização não tiver licenças adicionais do Salesforce, você poderá usar um usuário de marketing **com o perfil** Administrador do sistema **existente.**

1. Digite &quot;users&quot; na barra de pesquisa Navegador e clique em **Users** em **Gerenciar usuários**.

   ![](assets/image2014-12-9-12-3a57-3a42.png)

1. Clique em **Novo usuário**.

   ![](assets/image2014-12-9-12-3a58-3a1.png)

1. Preencha os campos obrigatórios e selecione **Licença de usuário: Salesforce**, defina o Perfil **: Administrador do sistema**, marque **Usuário de marketing** e clique em **Salvar**.

   ![](assets/image2014-12-9-12-3a58-3a11.png)

   >[!TIP]
   >
   >Verifique se o endereço de email digitado é válido. Você precisará fazer logon como o usuário de sincronização para redefinir a senha.

Excelente! Agora você tem uma conta que o Marketo pode usar para se conectar ao Salesforce. Vamos fazer isso.

>[!MORELIKETHIS]
>
>[Etapa 3 de 3: Connect Marketing e Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-3-of-3-connect-marketo-and-salesforce-professional.md)
