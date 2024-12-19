---
unique-page-id: 2360362
description: Etapa 1 de 3 - Adicionar campos do Marketo à Salesforce (Enterprise/Unlimited) - Documentação do Marketo - Documentação do produto
title: Etapa 1 de 3 - Adicionar campos do Marketo à Salesforce (Enterprise/Unlimited)
exl-id: bcfba281-0d4b-42c3-b52a-ce1c3da884ba
feature: Salesforce Integration
source-git-commit: 989804463f44afbf35ab11c0f23c37b0d328e652
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 9%

---

# Etapa 1 de 3: Adicionar campos do Marketo à Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>Você deve ter acesso às APIs do Salesforce para sincronizar entre o Marketo Engage e o Salesforce.

O Marketo usa um conjunto de campos para capturar determinados tipos de informações relacionadas a marketing. Se quiser esses dados no Salesforce, siga as instruções abaixo.

1. Crie três campos personalizados no Salesforce no cliente potencial e objetos de contato: Pontuação, Programa de aquisição e Data de aquisição.
1. Mapeie esses campos personalizados entre clientes potenciais e contatos para que, na conversão no Salesforce, os valores continuem.
1. Você pode criar outros campos adicionais, se necessário (consulte a tabela abaixo).

Todos esses campos personalizados são opcionais e não são necessários para sincronizar o Marketo e o Salesforce. Como prática recomendada, é recomendado criar campos para Pontuação, Programa de aquisição e Data de aquisição.

## Adicionar campos do Marketo à Salesforce {#add-marketo-fields-to-salesforce}

Adicione três campos personalizados aos objetos de cliente potencial e contato no Salesforce listados acima. Se quiser adicionar mais, consulte a tabela de campos disponíveis no final desta seção.

Execute as etapas a seguir para cada um dos três campos personalizados para adicioná-los. Comece com Pontuação.

1. Faça logon no Salesforce e clique em **[!UICONTROL Instalação]**.

   ![](assets/image2016-5-23-13-3a15-3a21.png)

1. No menu [!UICONTROL Build], à esquerda, clique em **[!UICONTROL Personalizar]** e selecione **[!UICONTROL Clientes Potenciais]**. Clique em **[!UICONTROL Campos]**.

   ![](assets/image2016-5-23-13-3a20-3a5.png)

1. Clique em **[!UICONTROL Novo]** na seção Campos personalizados e relações na parte inferior da página.

   ![](assets/image2016-5-26-14-3a41-3a40.png)

1. Escolha o tipo de campo apropriado (para Pontuação - número; Programa de aquisição - texto; Data de aquisição - Data/hora).

   ![](assets/choose-field-type-2-hand.png)

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/image2016-5-26-14-3a51-3a14.png)

1. Insira o [!UICONTROL Rótulo do campo], [!UICONTROL Comprimento] e [!UICONTROL Nome do campo] para o campo, conforme mostrado na tabela abaixo.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Rótulo do campo 
    </div></th> 
   <th> 
    <div>
      Nome do campo 
    </div></th> 
   <th> 
    <div>
      Tipo de dados 
    </div></th> 
   <th> 
    <div>
      Atributos do campo 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Pontuação</td> 
   <td>mkto71_Lead_Score</td> 
   <td>Número</td> 
   <td>Comprimento 10<br>Casas decimais 0 </td> 
  </tr> 
  <tr> 
   <td>Data da aquisição</td> 
   <td>mkto71_Acquisition_Date</td> 
   <td>Data/hora</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programa de aquisição</td> 
   <td>mkto71_Acquisition_Program</td> 
   <td>Texto</td> 
   <td>Comprimento 255</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>O Salesforce anexa __c a Nomes de campos quando os usa para criar Nomes de API.

![](assets/image2016-5-26-14-3a55-3a33.png)

>[!NOTE]
>
>Os campos de texto e número exigem comprimento, mas os campos de Data/Hora não. Uma descrição é opcional.

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/image2016-5-23-14-3a50-3a5.png)

1. Especifique as configurações de acesso e clique em **[!UICONTROL Avançar]**:

   * Definir todas as funções como **[!UICONTROL Visível]** e **[!UICONTROL Somente Leitura]**

   * Desmarque a caixa de seleção **[!UICONTROL Somente Leitura]** para o perfil do seu usuário de sincronização:

      * Se você tiver um usuário com o perfil de um _Administrador do Sistema_ como o usuário de sincronização, desmarque a caixa de seleção **[!UICONTROL Somente Leitura]** do perfil de Administrador do Sistema (como mostrado abaixo)
      * Se você criou um _perfil personalizado_ para o usuário de sincronização, desmarque a caixa de seleção **[!UICONTROL Somente Leitura]** desse perfil personalizado

   ![](assets/image2016-6-30-9-3a25-3a4.png)

1. Escolha os layouts de página que devem exibir o campo.

   ![](assets/image2016-5-26-15-3a14-3a45.png)

1. Clique em **[!UICONTROL Salvar e Novo]** para voltar e criar cada um dos outros dois campos personalizados. Clique em **[!UICONTROL Salvar]** ao terminar com todos os três.

   ![](assets/image2016-5-23-15-3a8-3a43.png)

1. No menu Criar, à esquerda, clique em **[!UICONTROL Personalizar]** e selecione Contatos. Clique em Campos.
1. Execute as etapas de 3 a 10 para os campos Pontuação, Data de aquisição e Programa de aquisição no objeto de contato, da mesma forma que fazia para o objeto de lead.
1. Como opção, use o procedimento acima para qualquer campo personalizado adicional desta tabela.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Rótulo do campo 
    </div></th> 
   <th> 
    <div>
      Nome do campo 
    </div></th> 
   <th> 
    <div>
      Tipo de dados 
    </div></th> 
   <th> 
    <div>
      Atributos do campo 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID do programa de aquisição</td> 
   <td>mkto71_Acquisition_Program_Id</td> 
   <td>Número</td> 
   <td>Comprimento 18<br>Casas decimais 0 </td> 
  </tr> 
  <tr> 
   <td>Responsável pela indicação original</td> 
   <td>mkto71_Original_Referrer</td> 
   <td>Texto</td> 
   <td>Comprimento 255</td> 
  </tr> 
  <tr> 
   <td>Mecanismo de pesquisa original</td> 
   <td>mkto71_Original_Search_Engine</td> 
   <td>Texto</td> 
   <td>Comprimento 255</td> 
  </tr> 
  <tr> 
   <td>Frase de pesquisa original</td> 
   <td>mkto71_Original_Search_Phrase</td> 
   <td>Texto</td> 
   <td>Comprimento 255</td> 
  </tr> 
  <tr> 
   <td>Informações da fonte original</td> 
   <td>mkto71_Original_Source_Info</td> 
   <td>Texto</td> 
   <td>Comprimento 255</td> 
  </tr> 
  <tr> 
   <td>Tipo de fonte original</td> 
   <td>mkto71_Original_Source_Type</td> 
   <td>Texto</td> 
   <td>Comprimento 255</td> 
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
>Os valores nos campos atribuídos automaticamente pelo Marketo não estarão imediatamente disponíveis no Salesforce quando o novo campo for criado. O Marketo sincronizará os dados com o Salesforce na próxima atualização do registro em qualquer sistema (ou seja, uma atualização para qualquer um dos campos sincronizados entre o Marketo e o Salesforce).

## Mapear campos personalizados para conversões {#map-custom-fields-for-conversions}

Um campo personalizado no objeto de cliente potencial no Salesforce deve ser mapeado para um campo de contato no objeto de contato para que os dados sejam transportados quando ocorrer uma conversão.

1. No canto superior direito, clique em **[!UICONTROL Instalação]**.

   ![](assets/image2016-5-26-16-3a34-3a0.png)

1. Digite &quot;Campos&quot; na Pesquisa de navegação sem pressionar Enter. Os campos aparecem em objetos diferentes; clique em **[!UICONTROL Campos]** em Clientes potenciais.

   ![](assets/image2016-5-26-16-3a36-3a32.png)

1. Vá para a seção Campos Personalizados de Cliente Potencial e Relações e clique em **[!UICONTROL Mapear Campos de Cliente Potencial]**.

   ![](assets/image2016-5-26-16-3a39-3a29.png)

1. Clique na lista suspensa ao lado do campo que deseja mapear.

   ![](assets/image2016-5-26-16-3a49-3a53.png)

1. Selecione o campo personalizado de contato correspondente.

   ![](assets/image2016-5-26-16-3a56-3a23.png)

1. Repita as etapas acima para qualquer outro campo criado.

1. Clique em **[!UICONTROL Salvar]** quando terminar.

>[!MORELIKETHIS]
>
>[Etapa 2 de 3: Criar um Usuário do Salesforce para Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
