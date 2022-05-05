---
description: Etapa 1 de 3 - Adicionar campos do Marketo a todos os documentos do CRM - Marketo - Documentação do produto
title: Etapa 1 de 3 - Adicionar campos do Marketo a cada CRM
exl-id: a9a59e76-a7a4-4391-8169-922bd6acfb6d
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 7%

---

# Etapa 1 de 3: Adicionar campos do Marketo a cada CRM {#step-1-of-3-add-marketo-fields-to-veeva-crm}

>[!PREREQUISITES]
>
>Sua instância de Veva CRM deve ter acesso às APIs do Salesforce para sincronizar dados entre o Marketo Engage e Veeva CRM.

O Marketo Engage usa um conjunto de campos para capturar determinados tipos de informações relacionadas ao marketing. Se você desejar esses dados no Veeva CRM, siga as instruções abaixo.

`1.` Crie um campo personalizado em Veeva CRM nos objetos de contato: Pontuação

`2.` Se desejar, é possível criar campos adicionais (consulte a tabela abaixo).

Todos esses campos personalizados são opcionais e não são necessários para sincronizar o Marketo Engage e Veeva CRM.

## Adicionar campos do Marketo a cada CRM {#add-marketo-fields-to-veeva-crm}

Adicione três campos personalizados nos objetos lead e contact em Veeva CRM listados acima. Se desejar adicionar mais, consulte a tabela de campos disponíveis no final desta seção.

Execute as etapas a seguir para o campo Score para adicioná-lo.

1. Faça logon no CRM de Veeva e clique em **Configuração**.

   ![](assets/step-1-of-3-add-marketo-fields-1.png)

1. Clique em Objetos e campos e selecione Gerenciador de objetos.

   ![](assets/step-1-of-3-add-marketo-fields-2.png)

1. Na barra de pesquisa, procure por Contato.

   ![](assets/step-1-of-3-add-marketo-fields-3.png)

1. Clique no objeto Contact .

1. Selecione Campos e Relações.

1. Clique em **Novo**.

   ![](assets/step-1-of-3-add-marketo-fields-4.png)

1. Escolha o tipo de campo apropriado (para Pontuação — número).

   ![](assets/step-1-of-3-add-marketo-fields-5.png)

1. Clique em **Próximo**.

   ![](assets/step-1-of-3-add-marketo-fields-6.png)

1. Insira o Rótulo do campo, o Comprimento e o Nome do campo, conforme mostrado na tabela abaixo.

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
>Cada CRM anexa __c aos Nomes de Campo quando os usa para criar Nomes de API.

![](assets/step-1-of-3-add-marketo-fields-7.png)

>[!NOTE]
>
>Os campos de texto e número exigem um comprimento, mas os campos de Data/Hora não o exigem. Uma descrição é opcional.

1. Clique em **Próximo**.

   ![](assets/step-1-of-3-add-marketo-fields-8.png)

1. Especifique as configurações de acesso e clique em **Próximo**.

1. Defina todas as funções como Visível e Somente leitura.

1. Desmarque a caixa de seleção Somente leitura do perfil do usuário de sincronização:

* Se você tiver um usuário com o perfil de um Administrador do sistema como o usuário de sincronização, desmarque a caixa de seleção Somente leitura do perfil Administrador do sistema (como mostrado abaixo).
* Se você criou um perfil personalizado para o usuário de sincronização, desmarque a caixa de seleção Somente leitura desse perfil personalizado.

   ![](assets/step-1-of-3-add-marketo-fields-9.png)

1. Escolha os layouts de página que devem exibir o campo .

1. Clique em **Salvar e Novo** para voltar e criar cada um dos outros dois campos personalizados.

1. Clique em **Salvar** quando terminar com os três.

   ![](assets/step-1-of-3-add-marketo-fields-10.png)

>[!NOTE]
>
>Ao adicionar o campo ao objeto Contato , eles também são adicionados à conta de pessoa.

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
   <td>mkto71_Inferred_City</td>
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
>Os valores nos campos atribuídos automaticamente pelo Marketo não estarão disponíveis imediatamente em Veeva CRM quando o novo campo for criado. A Marketo sincronizará os dados com Veeva CRM na próxima atualização do registro em qualquer sistema (ou seja, uma atualização para qualquer um dos campos sincronizados entre o Marketo e Veeva CRM).
