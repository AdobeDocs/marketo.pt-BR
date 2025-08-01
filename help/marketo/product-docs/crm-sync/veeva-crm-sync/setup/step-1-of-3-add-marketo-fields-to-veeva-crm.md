---
description: Etapa 1 de 3 - Adicionar campos do Marketo ao [!DNL Veeva] CRM - Documentação do Marketo - Documentação do produto
title: Etapa 1 de 3 - Adicionar campos do Marketo ao [!DNL Veeva] CRM
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 8%

---

# Etapa 1 de 3: Adicionar Campos Marketo ao CRM [!DNL Veeva] {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>Sua instância do CRM [!DNL Veeva] deve ter acesso às APIs do Salesforce para sincronizar dados entre o Marketo Engage e o CRM [!DNL Veeva].

O Marketo Engage usa um conjunto de campos para capturar determinados tipos de informações relacionadas a marketing. Se desejar esses dados no [!DNL Veeva] CRM, siga as instruções abaixo.

`1.` Crie um campo personalizado no CRM [!DNL Veeva] nos objetos de contato: Pontuação

`2.` Você pode criar campos adicionais, se desejar (consulte a tabela abaixo).

Todos esses campos personalizados são opcionais e não são necessários para sincronizar o Marketo Engage e o [!DNL Veeva] CRM.

## Adicionar Campos do Marketo ao CRM [!DNL Veeva] {#add-marketo-fields-to-veeva-crm}

Adicione um campo personalizado ao cliente potencial e aos objetos de contato no [!DNL Veeva] CRM listados acima. Se quiser adicionar mais, consulte a tabela de campos disponíveis no final desta seção.

Execute as seguintes etapas para que o campo Score o adicione.

1. Faça logon no [!DNL Veeva] CRM e clique em **[!UICONTROL Instalação]**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. Clique em **[!UICONTROL Objetos e Campos]** e selecione **[!UICONTROL Gerenciador de Objetos]**.

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. Na barra de pesquisa, pesquise por &quot;Contato&quot;.

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. Clique no objeto **[!UICONTROL Contato]**.

1. Selecione **[!UICONTROL Campos e Relações]**.

1. Clique em **[!UICONTROL Novo]**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. Escolha o tipo de campo apropriado (para Pontuação - número).

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. Insira o **[!UICONTROL Rótulo do campo]**, **[!UICONTROL Comprimento]** e **[!UICONTROL Nome do campo]** para o campo, conforme mostrado na tabela abaixo.

<table>
 <tbody>
  <tr>
   <th>Rótulo do campo
   <th>Nome do campo
   <th>Tipo de dados
   <th>Atributos do campo
  </tr>
  <tr>
   <td>Pontuação</td>
   <td>mkto71_Lead_Score</td>
   <td>Número</td>
   <td>Comprimento 10<br/>
Casas decimais 0</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>O CRM [!DNL Veeva] anexa __c a Nomes de campos quando os usa para criar Nomes de API.

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>Os campos de texto e número exigem comprimento, mas os campos de Data/Hora não. Uma descrição é opcional.

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. Especifique as configurações de acesso e clique em **[!UICONTROL Avançar]**.

1. Defina todas as funções como **[!UICONTROL Visível]** e **[!UICONTROL Somente Leitura]**.

1. Desmarque a caixa de seleção **[!UICONTROL Somente Leitura]** para o perfil do seu usuário de sincronização:

* Se você tiver um usuário com o perfil de Administrador do Sistema como o usuário de sincronização, desmarque a caixa de seleção [!UICONTROL Somente Leitura] do perfil de Administrador do Sistema (como mostrado abaixo).
* Se você criou um perfil personalizado para o usuário de sincronização, desmarque a caixa de seleção [!UICONTROL Somente Leitura] para esse perfil personalizado.

  ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. Escolha os layouts de página que devem exibir o campo.

1. Clique em **[!UICONTROL Salvar e Novo]** para voltar e criar cada um dos outros dois campos personalizados.

1. Clique em **[!UICONTROL Salvar]** quando terminar com todos os três.

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>Ao adicionar o campo ao objeto de Contato, eles também são adicionados ao objeto de Conta de pessoa.

OPCIONAL: Use o procedimento acima para qualquer campo personalizado adicional da tabela abaixo.

<table>
 <tbody>
  <tr>
   <th>Rótulo do campo
   <th>Nome do campo
   <th>Tipo de dados
   <th>Atributos do campo
  </tr>
  <tr>
   <td>Cidade indicada</td>
   <td>mkto71_Cidade_inferida</td>
   <td>Texto</td>
   <td>Comprimento 255</td>
  </tr>
  <tr>
   <td>Empresa indicada</td>
   <td>mkto71_Inferred_Company</td>
   <td>Texto</td>
   <td>Comprimento 255</td>
  </tr>
  <tr>
   <td>País indicado</td>
   <td>mkto71_Inferred_Country</td>
   <td>Texto</td>
   <td>Comprimento 255</td>
  </tr>
  <tr>
   <td>Área metropolitana indicada</td>
   <td>mkto71_Inferred_Metropolitan_Area</td>
   <td>Texto</td>
   <td>Comprimento 255</td>
  </tr>
  <tr>
   <td>Código de área telefônica indicado</td>
   <td>mkto71_Inferred_Phone_Area_Code</td>
   <td>Texto</td>
   <td>Comprimento 255</td>
  </tr>
  <tr>
   <td>Código postal indicado</td>
   <td>mkto71_Inferred_Postal_Code</td>
   <td>Texto</td>
   <td>Comprimento 255</td>
  </tr>
  <tr>
   <td>Estado/região indicado</td>
   <td>mkto71_Inferred_State_Region</td>
   <td>Texto</td>
   <td>Comprimento 255</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Os valores nos campos atribuídos automaticamente pelo Marketo não estarão imediatamente disponíveis no CRM [!DNL Veeva] quando o novo campo for criado. O Marketo sincronizará os dados com o CRM do [!DNL Veeva] na próxima atualização do registro em qualquer sistema (ou seja, uma atualização para qualquer um dos campos sincronizados entre o Marketo e o CRM do [!DNL Veeva]).
