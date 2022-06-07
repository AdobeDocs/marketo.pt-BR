---
description: Campos personalizados do membro do programa - Documentos do Marketo - Documentação do produto
title: Campos personalizados do membro do programa
hide: true
hidefromtoc: true
source-git-commit: 09e9ee74c32f81fdc826454266d3e16826a09eae
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Sincronização de Campo Personalizado do Membro do Programa {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>Criação de [Campos personalizados do membro do programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target=&quot;_blank&quot;}

>[!NOTE]
>
>O objeto Membro do programa pode ter até 20 campos personalizados. Esses campos estão disponíveis para qualquer programa.

## Mapear campos do Salesforce para campos personalizados do membro do programa {#map-salesforce-fields-to-program-member-custom-fields}

1. No Marketo, clique em **Administrador**.

   ![](assets/program-member-custom-field-sync-1.png)

1. Clique em **Salesforce**, depois clique em **Editar** ao lado de Sincronização de campo personalizado do membro do programa.

   ![](assets/program-member-custom-field-sync-2.png)

1. Use a caixa de pesquisa para localizar os campos do Salesforce que deseja mapear. Neste exemplo, estamos usando Não chamar.

   ![](assets/program-member-custom-field-sync-3.png)

1. Clique no menu suspenso .

   ![](assets/program-member-custom-field-sync-4.png)

1. Escolha o Campo Personalizado do Membro do Programa Marketo desejado para mapear.

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >A lista suspensa mostrará apenas os Campos Personalizados do Membro do Programa que correspondem ao tipo de dados do campo Salesforce .

1. Para mapeamentos de campo adicionais, desmarque a caixa de pesquisa e repita as etapas de 3 a 5.

1. Clique em **Salvar** quando concluído.

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >As alterações nos dados do membro do programa nos campos mapeados serão sincronizadas entre o Marketo e o Salesforce a partir de agora.

   >[!NOTE]
   >
   >Se você renomear ou alterar o tipo de dados de um campo no Salesforce, removeremos qualquer mapeamento desse campo com o Campo Personalizado do Membro do Programa. Mas você pode remapeá-lo com o novo campo após a revisão.

## Desmapear Campos do Salesforce a partir de Campos Personalizados do Membro do Programa {#unmap-salesforce-fields-from-program-member-custom-fields}

Se você quiser liberar um campo para substituí-lo ou apenas fazer uma alteração geral, é necessário realizar um desmapeamento primeiro. Veja como.

1. No Marketo, clique em **Administrador**.

   ![](assets/program-member-custom-field-sync-7.png)

1. Clique em **Salesforce**, depois clique em **Editar** ao lado de Sincronização de campo personalizado do membro do programa.

   ![](assets/program-member-custom-field-sync-8.png)

1. Use a caixa de pesquisa para localizar os campos que deseja desmapear. Neste exemplo, estamos usando Não chamar.

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >Você pode selecionar a variável **Mapeado** caixa de seleção para ver apenas os campos mapeados.

1. Desmapeie clicando no botão **X** ao lado do campo .

   ![](assets/program-member-custom-field-sync-10.png)

1. O mapeamento foi removido. Clique em **Salvar**.

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
      <td>Lista de opções de seleção múltipla</td>
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
>* [Alterar Dados do Membro do Programa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target=&quot;_blank&quot;}
>* [Exibir dados na grade Membro do Programa](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target=&quot;_blank&quot;}

