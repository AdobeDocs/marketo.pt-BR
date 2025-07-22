---
unique-page-id: 9437903
description: Criar um  [!DNL Dynamics] Filtro de sincronização - Documentação do Marketo - Documentação do produto
title: Criar um Filtro de Sincronização  [!DNL Dynamics]  Personalizado
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 1%

---

# Criar um filtro de sincronização [!DNL Dynamics] personalizado {#create-a-custom-dynamics-sync-filter}

Não deseja sincronizar tudo no Dynamics CRM com o Marketo Engage? Não se preocupe! O Marketo permite configurar um filtro de sincronização e sincronizar apenas parte de seus registros.

## Visão geral {#overview}

Para configurar um filtro de sincronização [!DNL Dynamics]:

1. Crie um campo personalizado de Duas Opções (booleano) chamado new_synctomkto no Dynamics CRM para qualquer objeto (cliente potencial, contato, conta, oportunidade e outras entidades personalizadas).
1. Atribua um valor Sim/Não a esse campo.

Essas alterações devem ser feitas no Dynamics CRM, não no banco de dados ou no Marketo.

>[!CAUTION]
>
>Se você não atribuir o campo e deixá-lo em branco/NULO, ele será sincronizado, mas não será atualizado. Os registros com um valor de campo em branco/NULO no Dynamics CRM mostrarão esse valor de campo no Marketo como &quot;falso&quot;.

O Marketo procura esse campo durante a sincronização automática em segundo plano e determina em quais registros sincronizar com base nessa lógica:

| Valor do campo | Sincronizar com o Marketo? |
|---|---|
| O campo não existe | Sim |
| O campo está vazio | Sim |
| O campo tem valor Sim | Sim |
| O campo tem o valor Não | Não |

>[!CAUTION]
>
>A única maneira de instruir o Marketo a ignorar um registro é definir explicitamente o valor do campo como **Não**. O Marketo ainda sincroniza registros mesmo se os valores dos campos estiverem vazios.

>[!PREREQUISITES]
>
>Instale a versão mais recente do Plug-in do Marketo (3.0.0.1 ou posterior). Vá para Marketo > [!UICONTROL Admin] > [!DNL Microsoft Dynamics] > [!UICONTROL Baixar Solução da Marketo].

## Criar campo SyncToMkto {#create-synctomkto-field}

1. Faça logon no Dynamics CRM. Clique em **Configurações** e em **Personalizações**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Clique em **[!UICONTROL Personalizar o sistema]**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Clique em ![](assets/image2015-8-10-21-3a44-3a23.png) próximo a **[!UICONTROL Entidades]**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Clique em ![](assets/image2015-8-10-21-3a44-3a23.png) ao lado de **[!UICONTROL Lead]** e selecione **[!UICONTROL Campos]**. Depois clique em **[!UICONTROL Novo]**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Insira **SyncToMkto** no campo **[!UICONTROL Nome para Exibição]** e selecione **[!UICONTROL Duas Opções]** como o **[!UICONTROL Tipo de Dados]**. Em seguida, clique em **[!UICONTROL Salvar e fechar]**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Escolha qualquer nome para exibição para este campo, mas o campo Nome deve ser exatamente **new_synctomkto**. Você deve usar **novo** como prefixo padrão. Se você alterou o padrão, acesse aqui para [redefinir o prefixo padrão para os nomes de campo personalizados](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md){target="_blank"}. Você pode alterá-la de volta após criar os novos campos.

   >[!NOTE]
   >
   >Se você tiver configurado um fluxo de trabalho assíncrono, o registro obterá o valor SyncToMkto padrão definido no campo e o valor correto será obtido alguns segundos depois, quando o fluxo de trabalho terminar de ser executado. Se o valor padrão for definido como Sim, esses registros serão criados no Marketo e se tornarão obsoletos. Use **Não** como valor padrão para evitar isso.

1. Repita esse processo e crie o campo **SyncToMkto** para quaisquer outras entidades nas quais você deseja limitar a sincronização, como contato, conta, oportunidade e entidades personalizadas.

## Selecione o filtro no Marketo {#select-the-filter-in-marketo}

Mesmo que você já tenha feito a sincronização inicial, acesse e selecione os campos a serem sincronizados com o Marketo.

1. Vá para Admin e selecione **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **[!UICONTROL Editar]** em Detalhes da Sincronização de Campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e marque-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer item. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Ótimo, agora você ativou o filtro de sincronização do Marketo.

## Crie um Fluxo de Trabalho [!DNL Dynamics] para Atribuir Valores de Filtro de Sincronização Automaticamente {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Você sempre pode atribuir um valor manualmente aos campos SyncToMkto para seus registros. Mas por que não aproveitar o poder de um Fluxo de Trabalho [!DNL Dynamics] e atribuir automaticamente um valor ao campo SyncToMkto quando um registro é criado ou atualizado?

>[!NOTE]
>
>Você não pode fazer isso no nível do banco de dados. Isso deve ser feito no CRM manualmente ou usando um workflow.
>
>Um fluxo de trabalho [!DNL Dynamics] funciona somente em novos registros criados a partir de agora, não em dados históricos. Use uma atualização em lote para mover registros existentes.

1. Vá para o Dynamics CRM. Clique em **Configurações** e depois em **Processos**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Insira um nome para o fluxo de trabalho e selecione **[!UICONTROL Fluxo de trabalho]** como [!UICONTROL Categoria] e **[!UICONTROL Líder]** como [!UICONTROL Entidade]. Depois clique em **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Crie regras para atribuir um valor verdadeiro ou falso ao campo **SyncToMkto** com base na preferência da sua organização. Clique em **[!UICONTROL Salvar e fechar]**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Defina uma Ação padrão depois de clicar em **[!UICONTROL Adicionar etapa]** para adicionar uma Condição de verificação. Isto define os registros que você não quer sincronizar com **Não**. Caso contrário, eles serão sincronizados.

1. Selecione o workflow e clique em **[!UICONTROL Ativar]**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Consulte [Regras de Filtro de Sincronização Personalizada para um Endereço de Email](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"} para configurar regras para sincronizar apenas registros de pessoas com endereços de email.

## Detalhes do Filtro de Sincronização {#sync-filter-details}

Estes são alguns detalhes de implementação que pensamos que você deveria saber:

* Iniciar uma Operação de Sincronização

  Quando o valor **SyncToMkto** muda de **Não** para **Sim**, [!DNL Dynamics] notifica o Marketo imediatamente para começar a sincronizar este registro. Se o registro já existir, o Marketo o atualizará. Caso contrário, o Marketo criará o registro.

  >[!TIP]
  >
  >Uma operação `Create [StartSync]` é adicionada ao Log do Marketo quando isso ocorre.

* Parar uma operação de sincronização

  Quando um registro altera seu valor SyncToMkto de Sim para Não, a Marketo é notificada para interromper a sincronização desse registro. No entanto, o registro não é excluído. Em vez disso, ele pára de obter atualizações e se torna obsoleto.

>[!MORELIKETHIS]
>
>* [Filtro de Sincronização do Microsoft Dynamics: Qualificar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md){target="_blank"}
>* [Filtro de Sincronização do Microsoft Dynamics: Mesclar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md){target="_blank"}
>* [Regras de Filtro de Sincronização Personalizado para um Endereço de Email](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md){target="_blank"}
