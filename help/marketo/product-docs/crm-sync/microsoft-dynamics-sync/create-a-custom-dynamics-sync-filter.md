---
unique-page-id: 9437903
description: Criar um filtro de sincronização dinâmico personalizado - Documentos do Marketo - Documentação do produto
title: Criar um filtro de sincronização dinâmico personalizado
exl-id: 6b0d878a-9c55-4e73-9923-11140e83bb37
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# Criar um filtro de sincronização dinâmico personalizado {#create-a-custom-dynamics-sync-filter}

Não quer sincronizar tudo no seu Dynamics CRM para o Marketo? Não se preocupe! O Marketo permite configurar um filtro de sincronização e sincronizar apenas parte dos registros.

## Visão geral {#overview}

Para configurar um filtro de sincronização do Dynamics:

1. Crie um campo personalizado de Duas opções (booleano) chamado new_synctomkto em seu Dynamics CRM para qualquer objeto (lead, contato, conta, oportunidade e outras entidades personalizadas).
1. Atribua a este campo um valor Sim/Não ou deixe-o em branco.

>[!NOTE]
>
>Você deve fazer essas alterações no Dynamics CRM, não no banco de dados ou no Marketo.

O Marketo procura esse campo durante a sincronização automática em segundo plano e determina em quais registros sincronizar com base nessa lógica:

| Valor do campo | Sincronizar com o Marketo? |
|---|---|
| O campo não existe | Sim |
| Campo vazio | Sim |
| O campo tem o valor Sim | Sim |
| Campo com valor Não | Não |

>[!CAUTION]
>
>A única maneira de dizer ao Marketo para ignorar um registro é definir o valor do campo explicitamente como **No**. O Marketo ainda sincroniza registros, mesmo se os valores de campo estiverem vazios.

>[!PREREQUISITES]
>
>Instale a versão mais recente do plug-in do Marketo (3.0.0.1 ou posterior). Acesse Marketo > Admin > Microsoft Dynamics > Baixar solução Marketo.

## Criar campo SyncToMkto {#create-synctomkto-field}

1. Faça logon no Dynamics CRM. Clique em **Configurações** e em **Personalizações**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Clique em **Personalizar o sistema**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Clique em ![](assets/image2015-8-10-21-3a44-3a23.png) ao lado de **Entidades**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Clique em ![](assets/image2015-8-10-21-3a44-3a23.png) ao lado de **Lead** e selecione **Campos**. Em seguida, clique em **New**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Insira **SyncToMkto** no campo **Nome de Exibição** e selecione **Duas opções** como o **Tipo de Dados**. Em seguida, clique em **Salvar e fechar**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Escolha qualquer nome de exibição para esse campo, mas o campo Nome deve ser exatamente **new_synctomkto**. Você deve usar **new** como o prefixo padrão. Se tiver alterado o padrão, acesse [redefinir o prefixo padrão dos nomes de campo personalizados](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md). É possível alterá-lo novamente depois de criar os novos campos.

   >[!NOTE]
   >
   >Se você tiver um fluxo de trabalho assíncrono configurado, o registro obterá o valor padrão SyncToMkto que você configurou no campo e obterá o valor correto alguns segundos depois, quando o fluxo de trabalho terminar de ser executado. Se o valor padrão estiver definido como Sim, esses registros serão criados no Marketo e se tornarão obsoletos. Use **No** como o valor padrão para evitar isso.

1. Repita esse processo e crie o campo **SyncToMkto** para quaisquer outras entidades nas quais deseja limitar a sincronização, como contato, conta, oportunidade e entidades personalizadas.

## Selecione o filtro no Marketo {#select-the-filter-in-marketo}

Mesmo que já tenha feito a sincronização inicial, entre e selecione os campos a serem sincronizados com o Marketo.

1. Vá para Admin e selecione **MIcrosoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e verifique-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer coisa. Clique em **Salvar**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Ótimo, agora você ativou o filtro de sincronização para o Marketo.

## Criar um fluxo de trabalho dinâmico para atribuir valores do filtro de sincronização automaticamente {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Você sempre pode atribuir manualmente um valor aos campos SyncToMkto para seus registros. Mas por que não aproveitar o potencial de um fluxo de trabalho dinâmico e atribuir automaticamente um valor ao campo SyncToMkto quando um registro é criado ou atualizado?

>[!NOTE]
>
>Não é possível fazer isso no nível do banco de dados. Isso deve ser feito no CRM manualmente ou usando um workflow.
>
>Um fluxo de trabalho Dynamics funciona somente em novos registros criados a partir de agora, não em dados históricos. Use uma atualização em lote para mover os registros existentes.

1. Vá para Dynamics CRM. Clique em **Settings** e depois clique em **Processes**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Clique em **Novo**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Insira um nome para o workflow e selecione **Workflow** como a categoria e **Lead** como a Entidade. Em seguida, clique em **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Crie regras para atribuir um valor verdadeiro ou falso ao campo **SyncToMkto** com base na preferência da sua organização. Clique em **Salvar e fechar**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Defina uma Ação Padrão depois de clicar em **Adicionar Etapa** para adicionar uma Condição de Verificação. Isso define os registros que você não deseja sincronizar para **No**. Caso contrário, serão sincronizados.

1. Selecione o workflow e clique em **Ativate**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Consulte [Regras de Filtro de Sincronização Personalizado para um Endereço de Email](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md) para configurar regras para sincronizar apenas registros para pessoas com endereços de email.

## Detalhes do filtro de sincronização {#sync-filter-details}

Estes são alguns detalhes de implementação que achamos que você deve saber:

1. Iniciar uma Operação de Sincronização

   Quando o valor **SyncToMkto** muda de **Não** para **Sim**, o Dynamics notifica imediatamente o Marketo para iniciar a sincronização deste registro. Se o registro já existir, o Marketo o atualizará. Caso contrário, o Marketo criará o registro.

   >[!TIP]
   >
   >Uma operação `Create [StartSync]` é adicionada ao Log do Marketo quando isso ocorre.

1. Parar uma Operação de Sincronização

   Quando um registro altera seu valor SyncToMkto de Sim para Não, a Marketo é notificada para parar de sincronizar esse registro. No entanto, o registro não é excluído, em vez disso, ele para de receber atualizações e se torna obsoleto.

>[!MORELIKETHIS]
>
>* [Filtro de Sincronização do Microsoft Dynamics: Qualificar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Filtro de Sincronização do Microsoft Dynamics: Mesclar](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [Regras de Filtro de Sincronização Personalizado para um Endereço de Email](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)

