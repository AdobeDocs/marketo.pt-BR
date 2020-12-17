---
unique-page-id: 9437903
description: Criar um filtro personalizado de sincronização dinâmica - Documentos do marketing - Documentação do produto
title: Criar um filtro personalizado de sincronização dinâmica
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---


# Criar um Filtro de Sincronização Dinâmica Personalizado {#create-a-custom-dynamics-sync-filter}

Não quer sincronizar tudo no seu Dynamics CRM para o Marketing? Não se preocupe! O Marketo permite que você configure um filtro de sincronização e sincronize apenas parte de seus registros.

## Visão geral {#overview}

Para configurar um filtro de sincronização do Dynamics:

1. Crie um campo personalizado de duas opções (booleano) chamado new_synctomkto no Dynamics CRM para qualquer objeto (lead, contato, conta, oportunidade e outras entidades personalizadas).
1. Atribua um valor Sim/Não a esse campo ou deixe-o em branco.

>[!NOTE]
>
>Você deve fazer essas alterações no Dynamics CRM, não no banco de dados ou no Marketo.

O Marketo procura esse campo durante a sincronização automática em segundo plano e determina em quais registros sincronizar com base nessa lógica:

| Valor do campo | Sincronizar com o Marketo? |
|---|---|
| O campo não existe | Sim |
| O campo está vazio | Sim |
| O campo tem valor Sim | Sim |
| O campo tem o valor Não | Não |

>[!CAUTION]
>
>A única maneira de dizer ao Marketo para ignorar um registro é definir explicitamente o valor do campo como **No**. O Marketo ainda sincroniza registros mesmo se os valores de campo estiverem vazios.

>[!PREREQUISITES]
>
>Instale a versão mais recente do Plug-in do Marketo (3.0.0.1 ou posterior). Acesse Marketo > Admin > Microsoft Dynamics > Baixar solução de marketing.

## Criar campo SyncToMkto {#create-synctomkto-field}

1. Faça logon no Dynamics CRM. Clique em **Configurações** e, em seguida, clique em **Personalizações**.

   ![](assets/image2015-8-10-21-3a40-3a9.png)

1. Clique em **Personalizar o sistema**.

   ![](assets/image2015-8-10-21-3a42-3a15.png)

1. Clique em ![](assets/image2015-8-10-21-3a44-3a23.png) ao lado de **Entidades**.

   ![](assets/image2015-8-10-21-3a43-3a39.png)

1. Clique em ![](assets/image2015-8-10-21-3a44-3a23.png) ao lado de **Lead **e selecione **Campos**. Em seguida, clique em **Novo**.

   ![](assets/image2015-8-10-21-3a49-3a49.png)

1. Digite **SyncToMkto** no campo **Nome de exibição** e selecione **Duas opções** como **Tipo de dados**. Em seguida, clique em **Salvar e Fechar**.

   ![](assets/image2015-9-8-10-3a25-3a33.png)

   >[!NOTE]
   >
   >Escolha qualquer nome de exibição para esse campo, mas o campo Nome deve ser exatamente **new_synctomkto**. Você deve usar **new** como o prefixo padrão. Se você tiver alterado o padrão, acesse [redefina o prefixo padrão para os nomes de campos personalizados](create-a-custom-dynamics-sync-filter/set-a-default-custom-field-prefix.md). É possível alterá-la novamente depois de criar os novos campos.

   >[!NOTE]
   >
   >Se você tiver um fluxo de trabalho assíncrono configurado, o registro obterá o valor padrão SyncToMkto configurado no campo e obterá o valor correto alguns segundos depois, quando o fluxo de trabalho terminar de ser executado. Se o valor padrão estiver definido como Sim, esses registros serão criados no Marketo e se tornarão obsoletos. Use **No** como valor padrão para evitar isso.

1. Repita esse processo e crie o campo **SyncToMkto** para quaisquer outras entidades nas quais você deseja limitar a sincronização, como contato, conta, oportunidade e entidades personalizadas.

## Selecione o Filtro em Marketo {#select-the-filter-in-marketo}

Mesmo se você já tiver feito a sincronização inicial, entre e selecione os campos a serem sincronizados com o Marketo.

1. Vá para Admin e selecione **MIcrosoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Role para baixo até o campo e verifique-o. O nome real deve ser new_synctomkto, mas o Nome de exibição pode ser qualquer coisa. Clique em **Salvar**.

   ![](assets/image2015-10-9-9-3a56-3a23.png)

Ótimo, agora você habilitou o filtro de sincronização para o Marketo.

## Criar um fluxo de trabalho dinâmico para atribuir valores de filtro de sincronização automaticamente {#create-a-dynamics-workflow-to-assign-sync-filter-values-automatically}

Você sempre pode atribuir manualmente um valor aos campos SyncToMkto para seus registros. Mas por que não aproveitar o poder de um Fluxo de Trabalho Dinâmico e atribuir automaticamente um valor ao campo SyncToMkto quando um registro é criado ou atualizado?

>[!NOTE]
>
>Não é possível fazer isso no nível do banco de dados. Isso deve ser feito no CRM manualmente ou usando um fluxo de trabalho.
>
>Um fluxo de trabalho Dinâmico funciona somente em novos registros criados em andamento, não em dados históricos. Use uma atualização em lote para mover-se sobre registros existentes.

1. Vá para o Dynamics CRM. Clique em **Configurações** e, em seguida, clique em **Processos**.

   ![](assets/image2015-8-11-8-3a42-3a10.png)

1. Clique em **Novo**.

   ![](assets/image2015-8-11-8-3a43-3a46.png)

1. Insira um nome para o fluxo de trabalho e selecione **Fluxo de trabalho** como a categoria e **Lead** como a Entidade. Em seguida, clique em **OK**.

   ![](assets/image2015-8-11-8-3a45-3a46.png)

1. Crie regras para atribuir um valor verdadeiro ou falso ao campo **SyncToMkto** com base na preferência da sua organização. Clique em **Salvar e Fechar**.

   ![](assets/setsynctomkto-fix.png)

   >[!NOTE]
   >
   >Defina uma ação padrão depois de clicar em **Adicionar etapa** para adicionar uma condição de verificação. Isso define os registros que você não deseja sincronizar como **No**. Caso contrário, eles serão sincronizados.

1. Selecione o fluxo de trabalho e clique em **Ativar**.

   ![](assets/image2015-8-11-8-3a57-3a29.png)

   >[!TIP]
   >
   >Consulte [Regras de Filtro de Sincronização Personalizado para um Endereço de Email](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md) para configurar regras para sincronizar somente registros de pessoas com endereços de email.

## Detalhes do filtro de sincronização {#sync-filter-details}

Veja alguns detalhes de implementação que achamos que você deve saber:

1. Start de uma operação de sincronização

   Quando o valor **SyncToMkto** mudar de **No** para **Yes**, o Dynamics notifica imediatamente o Marketo ao start para sincronizar este registro. Se o registro já existir, o Marketo o atualizará. Caso contrário, Marketo criará o registro.

   >[!TIP]
   >
   >Uma operação **Create [StartSync]** é adicionada ao Log de marketing quando isso acontece.

1. Parar uma operação de sincronização

   Quando um registro altera seu valor SyncToMkto de Yes para No, Marketo é notificado para parar a sincronização desse registro. No entanto, o registro não é excluído, em vez disso, interrompe a obtenção de atualizações e torna-se obsoleto.

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Filtro de Sincronização do Microsoft Dynamics: Qualificar](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-qualify.md)
>* [Filtro de Sincronização do Microsoft Dynamics: Mesclar](create-a-custom-dynamics-sync-filter/microsoft-dynamics-sync-filter-merge.md)
>* [Regras de filtro de sincronização personalizada para um endereço de email](create-a-custom-dynamics-sync-filter/custom-sync-filter-rules-for-an-email-address.md)

>



