---
description: Sincronização de campo personalizado do membro do programa - Documentação do Marketo - Documentação do produto
title: Sincronização de Campo Personalizado de Membro do Programa
exl-id: 7facfc79-a411-4ad9-b847-2002763af5bb
feature: Programs
source-git-commit: e49860ae611f2f77789bb491aeccbee46a911a2c
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 8%

---

# Sincronização de Campo Personalizado de Membro do Programa {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>* Criação de [Campos Personalizados de Membros do Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target="_blank"}
>* [Sincronizar uma campanha do Salesforce com um programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}

>[!NOTE]
>
>O objeto Membro do programa pode ter até 20 campos personalizados. Esses campos estão disponíveis para qualquer programa.

## Mapear campos do Salesforce para campos personalizados de membros do programa {#map-salesforce-fields-to-program-member-custom-fields}

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/program-member-custom-field-sync-1.png)

1. Clique em **[!DNL Salesforce]** e, em seguida, clique em **[!UICONTROL Editar]** ao lado de Sincronização de campo personalizado do membro do programa.

   ![](assets/program-member-custom-field-sync-2.png)

1. Use a caixa de pesquisa para localizar os campos do Salesforce que deseja mapear. Neste exemplo, estamos usando Do Not Call.

   ![](assets/program-member-custom-field-sync-3.png)

1. Clique na lista suspensa.

   ![](assets/program-member-custom-field-sync-4.png)

1. Escolha o Campo Personalizado de Membro do Programa Marketo que deseja mapear.

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >O menu suspenso mostrará apenas os Campos personalizados do membro do programa que correspondem ao tipo de dados do campo Salesforce.

1. Para mapeamentos de campo adicionais, desmarque a caixa de pesquisa e repita as etapas de 3 a 5.

1. Clique em **[!UICONTROL Salvar]** quando terminar.

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >As alterações nos dados dos membros do programa nos campos mapeados serão sincronizadas entre o Marketo e o Salesforce a partir de agora.

   >[!NOTE]
   >
   >Se você renomear ou alterar o tipo de dados de um campo no Salesforce, removeremos qualquer mapeamento desse campo com o Campo personalizado do membro do programa. Mas você pode remapeá-lo com o novo campo após a revisão.

## Desmapear campos do Salesforce dos campos personalizados do membro do programa {#unmap-salesforce-fields-from-program-member-custom-fields}

Se você quiser liberar um campo para substituí-lo ou apenas fazer uma alteração geral, execute um cancelamento de mapeamento primeiro. Veja como.

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/program-member-custom-field-sync-7.png)

1. Clique em **[!DNL Salesforce]** e, em seguida, clique em **[!UICONTROL Editar]** ao lado de Sincronização de campo personalizado do membro do programa.

   ![](assets/program-member-custom-field-sync-8.png)

1. Use a caixa de pesquisa para localizar os campos que deseja desmapear. Neste exemplo, estamos usando Do Not Call.

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >É possível selecionar a variável **[!UICONTROL Mapeado]** para ver apenas os campos mapeados.

1. Desmapeie clicando no ícone **X** ao lado do campo.

   ![](assets/program-member-custom-field-sync-10.png)

1. O mapeamento foi removido. Clique em **[!UICONTROL Salvar]**.

   ![](assets/program-member-custom-field-sync-11.png)

## Mapeamento de tipo de dados {#data-type-mapping}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Tipo de dados SFDC</th>
      <th>Tipo de Dados do Campo Personalizado do Membro do Programa</th>
    </tr>
    <tr>
      <td>Texto</td>
      <td>Sequência de caracteres</td>
    </tr>
    <tr>
      <td>Lista de seleção</td>
      <td>Sequência de caracteres</td>
    </tr>
    <tr>
      <td>Seleção múltipla da lista de opções</td>
      <td>Sequência de caracteres</td>
    </tr>
    <tr>
      <td>Telefone</td>
      <td>Sequência de caracteres</td>
    </tr>
    <tr>
      <td>Email</td>
      <td>Sequência de caracteres</td>
    </tr>
    <tr>
      <td>Número(m)</td>
      <td>Inteiro</td>
    </tr>
    <tr>
      <td>Número(m,n)</td>
      <td>Flutuante</td>
    </tr>
    <tr>
      <td>Caixa de seleção</td>
      <td>Booleano</td>
    </tr>
    <tr>
      <td>URL</td>
      <td>URL</td>
    </tr>
    <tr>
      <td>Data</td>
      <td>Data</td>
    </tr>
    <tr>
      <td>Datetime</td>
      <td>Datetime</td>
    </tr>
    <tr>
      <td>Pesquisa (referência)</td>
      <td>Sequência de caracteres</td>
    </tr>
    <tr>
      <td>Base64</td>
      <td>Sequência de caracteres</td>
    </tr>
  </tbody>
</table>

>[!MORELIKETHIS]
>
>* [Alterar dados dos membros do programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target="_blank"}
>* [Exibir dados na grade de Membros do Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target="_blank"}
>* [Sincronização do SFDC - Sincronização do Campaign](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
