---
unique-page-id: 2360368
description: Configuração do Marketing to Sales Insight no Salesforce Enterprise/Unlimited - Documentos do Marketing - Documentação do produto
title: Configurar o Marketing to Sales Insight no Salesforce Enterprise/Unlimited
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---


# Configurar o Marketing to Sales Insight no Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Estas são as etapas necessárias para configurar o Marketing to Sales Insight no Salesforce Enterprise/Unlimited Editions. Vamos começar.

>[!PREREQUISITES]
>
>* [Configurar a sincronização de campos do Marketing em seu Salesforce Enterprise/Unlimited Edition](http://docs.marketo.com/pages/viewpage.action?pageid=2360372)
>* [Instalar o pacote de insight de vendas do Marketing Cloud na AppExchange do Salesforce](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>



>[!NOTE]
>
>**Permissões de administrador necessárias**

## Configurar insight de vendas no Marketing {#configure-sales-insight-in-marketo}

1. Abra uma nova janela do navegador para obter as credenciais do Marketing Insight de vendas da sua conta de Marketing.
1. Vá para a área Admin e selecione **Sales Insight**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Clique em **Editar configuração da API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Digite uma chave secreta da API de sua escolha e clique em **Salvar**. NÃO use um E comercial (&amp;) em sua chave secreta da API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >Sua chave secreta da API é como uma senha para sua organização e deve ser segura.

1. Clique em **Visualização** no painel Restaurar configuração da API para preencher as credenciais.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Você verá um pop-up de confirmação. Clique em **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

## Configurar insight de vendas no Salesforce {#configure-sales-insight-in-salesforce}

1. No Salesforce, clique em **Setup**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Procure &quot;site remoto&quot; e selecione **Configurações de site remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Clique em **Novo Site Remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Digite o Nome do site remoto (pode ser algo como &quot;MarketoSoapAPI&quot;). Insira o URL do site remoto, que é o URL do host do Marketo no painel Configuração da API Soap no Marketo. Clique em **Salvar**. Agora você criou configurações de site remoto para a API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Clique novamente em **Novo Site Remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Digite o Nome do site remoto (pode ser algo como &quot;MarketoRestAPI&quot;). Insira o URL do site remoto, que é o URL da sua API no painel Restaurar configuração da API no Marketo. Clique em **Salvar**. Agora você criou configurações de site remoto para a Rest API.

## Configurar o Marketing to Sales Insight {#set-up-marketo-sales-insight}

1. Faça logon na sua instância do Marketo e clique em **Admin**.

   ![](assets/login-admin.png)

1. Clique em** Sales Insight**.

   ![](assets/image2015-5-22-15-3a12-3a33.png)

1. Clique em **Editar configuração da API**.

   ![](assets/image2015-5-22-15-3a15-3a0.png)

1. Digite uma **chave secreta da API** e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/image2015-5-27-16-3a36-3a56.png)

   >[!TIP]
   >
   >Mantenha esta janela aberta. Você precisará dessas informações mais tarde no Salesforce.

1. Volte para Salesforce e clique em **Setup**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Procure &quot;site remoto&quot; e clique em **Configuração remota de site** em **Controles de segurança**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Clique em **Novo Site Remoto**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Digite **Nome do site remoto** e **URL do site remoto**, em seguida, clique em **Salvar**.

   ![](assets/remote-site.png)

   >[!NOTE]
   >
   >Escolha seu **Nome do site remoto** (a API de marketing é usada aqui). O **URL do site remoto** pode ser encontrado no campo Host de marketing da caixa de diálogo Editar configuração da API na Etapa 4.

## Personalizar layouts de página {#customize-page-layouts}

1. Clique em **Configuração**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Procure por &quot;layout de página&quot; e selecione **Layout de página** em **Leads**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Clique em **Páginas de força de visita **à esquerda. Arraste **Seção** para o layout abaixo da seção Links personalizados.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Digite &quot;Marketing to Sales Insight&quot; como o **Nome da Seção**. Selecione **1-Column** e clique em **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arraste e solte **Lead** na nova seção.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >O nome dessa caixa será alterado com base no tipo de objeto. Por exemplo, se você estiver modificando o layout da página para Contatos, isso indicará Contato.

1. Clique com o duplo no bloco **Lead** que acabou de adicionar.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Edite a altura para **450** pixels e clique em **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >Recomendamos uma altura de 410 pixels para os objetos Contas e Oportunidades.

1. Clique em **Campos **à esquerda. Em seguida, pesquise e arraste o rótulo **Envolvimento** para o layout **Marketing to Sales Insight**.

   ![](assets/image2015-5-22-16-3a32-3a46.png)

1. Repita a etapa acima também para esses campos.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Envolvimento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor da pontuação relativa</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de urgência</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Data do Último Momento Interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Desc do último momento interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Origem do Último Momento Interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Último Tipo de Momento Interessante</p></td> 
  </tr> 
 </tbody> 
</table>

1. Clique em **Salvar** quando terminar.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita esse processo para adicionar seções de página do Visualforce e campos do Sales Insight para **Contact**, **Account** e **Oportunity**.
1. Repita as etapas de 5 a 7 para adicionar seções de página de Força de visita para Contato, Conta e Oportunidade. Em seguida, repita as etapas de 8 a 10 para adicionar campos de insight de vendas para **Contact**. Certifique-se de salvar após qualquer alteração.

## Mapear campos de pessoa personalizada {#map-custom-person-fields}

Campos de pessoa de marketing precisam ser mapeados para campos de contato do Salesforce para garantir que a conversão funcione corretamente. Veja como.

1. Clique em **Configuração**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Procure &quot;fields&quot; na barra de pesquisa e clique em **Campos** em **Clientes potenciais**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Clique em **Mapear campos de cliente potencial**.

   ** ![](assets/image2015-6-1-9-3a58-3a48.png)

   **

1. Clique na lista suspensa à direita para **Envolvimento**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Selecione **Contact.Engagement **na lista.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Repita e mapeie esses campos também.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">Campo personalizado de pessoa do Marketo</th> 
   <th colspan="1" rowspan="1">Campo Personalizado do Contato do Salesforce</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Envolvimento</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor da pontuação relativa</p></td> 
   <td colspan="1" rowspan="1"><p>Valor de Pontuação Relativa do Contact.Relative</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de urgência</p></td> 
   <td colspan="1" rowspan="1"><p>Valor Contact.Urgency</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Data do Último Momento Interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Data do último momento interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Desc do último momento interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interesting Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Origem do Último Momento Interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Fonte do Último Momento Interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Último Tipo de Momento Interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interesting Tipo de momento</p></td> 
  </tr> 
 </tbody> 
</table>

1. Clique em **Salvar **quando terminar.

## Configuração do Marketing Insight de Vendas {#marketo-sales-insight-config}

1. Clique em **+ **e selecione **Configuração do Marketing Insight**.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Marque **Ativar a API de marketing**. Em seguida, preencha as [informações de Configuração da API em Admin do Marketing ](http://docs.marketo.com/display/DOCS/Configure+Marketo+Sales+Insight+in+Salesforce+Professional+Edition#ConfigureMarketoSalesInsightinSalesforceProfessionalEdition-SetupMarketoSalesInsight). Clique em **Salvar alterações **quando terminar.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >Se o teste de diagnóstico falhar, talvez seja necessário [adicionar mais campos ao layout da página](http://nation.marketo.com/docs/DOC-1115).

E é isso! Você deve ser capaz de ver os campos do Marketing to Sales Insight para Clientes potenciais, Contatos, Contas e Oportunidades.

![](assets/twenty-six.png)

>[!NOTE]
>
>Para contas, o Sales Insight incluirá todos os emails, mas somente os momentos interessantes mais recentes, a atividade na Web e as alterações na pontuação.

## Acessar o Marketing to Sales Insight {#access-marketo-sales-insight}

1. No Salesforce, clique em **+** no final da barra de guias e clique em **Marketing Insight Config**.
1. Marque a caixa de seleção **Ativar API de marketing**.
1. Copie as credenciais do painel da API Soap na página Admin do Marketing Insight de Vendas e cole-as na seção API Soap da página Configuração do Salesforce Sales Insight.
1. Copie as credenciais do painel da Rest API na página Admin do Marketing Insight de Vendas e cole-as na seção Rest API da página Configuração do Salesforce Sales Insight.

   ![](assets/access-msi.png)

>[!MORELIKETHIS]
>
>* [Prioridade, urgência, pontuação relativa e melhores propostas](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Adicionar a guia de insight de vendas e botões do Marketing Cloud ao Salesforce](../../../../product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)

>



