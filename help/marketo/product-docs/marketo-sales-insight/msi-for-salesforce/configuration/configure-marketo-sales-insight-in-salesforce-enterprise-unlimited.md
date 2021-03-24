---
unique-page-id: 2360368
description: Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited - Documentos do Marketo - Documentação do produto
title: Configurar informações sobre vendas do Marketo no Salesforce Enterprise/Unlimited
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---


# Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Estas são as etapas que você precisa seguir para configurar o Marketing to Sales Insight no Salesforce Enterprise/Unlimited Editions. Vamos começar.

>[!PREREQUISITES]
>
>* [Configurar a sincronização de campo do Marketo em seu Salesforce Enterprise/Unlimited Edition](https://docs.marketo.com/pages/viewpage.action?pageid=2360372)
>* [Instale o Pacote de informações de vendas do Marketo no Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
>
>**Permissões de administrador necessárias**

## Configurar o Insight de vendas no Marketo {#configure-sales-insight-in-marketo}

1. Abra uma nova janela do navegador para obter as credenciais do Marketo Sales Insight de sua conta do Marketo.

1. Vá para a área Admin e selecione **Sales Insight**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Clique em **Editar configuração da API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Insira uma chave secreta da API de sua escolha e clique em **Save**. NÃO use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >Sua chave secreta da API é como uma senha para sua organização e deve ser segura.

1. Clique em **Exibir** no painel Restante configuração da API para preencher as credenciais.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Você verá um pop-up de confirmação. Clique em **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

## Configurar o Sales Insight no Salesforce {#configure-sales-insight-in-salesforce}

1. No Salesforce, clique em **Setup**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Procure por &quot;site remoto&quot; e selecione **Configurações de site remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Clique em **Novo Site Remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoSoapAPI&quot;). Insira o URL do site remoto, que é o URL do seu Marketo Host no painel Configuração da API Soap no Marketo. Clique em **Salvar**. Agora você criou configurações do site remoto para a API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Clique em **Novo Site Remoto** novamente.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoRestAPI&quot;). Insira o URL do site remoto, que é o URL da sua API do painel Configuração da API restante no Marketo. Clique em **Salvar**. Agora você criou configurações de site remoto para a API Rest.

## Configurar o Marketo Sales Insight {#set-up-marketo-sales-insight}

1. Faça logon na instância do Marketo e clique em **Admin**.

   ![](assets/login-admin.png)

1. Clique em **Sales Insight**.

   ![](assets/image2015-5-22-15-3a12-3a33.png)

1. Clique em **Editar configuração da API**.

   ![](assets/image2015-5-22-15-3a15-3a0.png)

1. Insira uma **Chave secreta da API** e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/image2015-5-27-16-3a36-3a56.png)

   >[!TIP]
   >
   >Mantenha essa janela aberta. Você precisará dessas informações posteriormente no Salesforce.

1. Volte para Salesforce e clique em **Setup**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Procure por &quot;local remoto&quot; e clique em **Configuração remota de site** em **Controles de segurança**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Clique em **Novo Site Remoto**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Insira **Nome do Site Remoto** e **URL do Site Remoto**, em seguida clique em **Guardar**.

   ![](assets/remote-site.png)

   >[!NOTE]
   >
   >Você escolhe seu **Nome do site remoto** (a API do Marketo é usada aqui). O **URL do site remoto** pode ser encontrado no campo Host do Marketo da caixa de diálogo Editar configuração da API na Etapa 4.

## Personalizar layouts de página {#customize-page-layouts}

1. Clique em **Configurar**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Procure por &quot;layout de página&quot; e selecione o **Layout de página** em **Leads**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Clique em **Visualforce Pages** à esquerda. Arraste **Section** para o layout abaixo da seção Links personalizados .

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Insira &quot;Marketing to Sales Insight&quot; como o **Nome da seção**. Selecione **1-Column** e clique em **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arraste e solte **Lead** na nova seção.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >O nome dessa caixa será alterado com base no tipo de objeto. Por exemplo, se você estiver modificando o layout da página para Contatos, isso dirá Contato.

1. Clique duas vezes no bloco **Lead** que acabou de adicionar.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Edite a altura para **450** pixels e clique em **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >Recomendamos uma altura de 410 pixels para os objetos Contas e Oportunidades.

1. Clique em **Fields** à esquerda. Em seguida, pesquise e arraste o rótulo **Envolvimento** para o layout **Insight de vendas do Marketo**.

   ![](assets/image2015-5-22-16-3a32-3a46.png)

1. Repita a etapa acima também para esses campos.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Envolvimento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor relativo da pontuação</p></td> 
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
   <td colspan="1" rowspan="1"><p>Fonte do Último Momento Interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Tipo de Último Momento Interessante</p></td> 
  </tr> 
 </tbody> 
</table>

1. Clique em **Salvar** quando terminar.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita esse processo para adicionar seções de página da Força de Vencimento e campos de Insight de Vendas para **Contato**, **Conta** e **Oportunidade**.

1. Repita as etapas 5 a 7 para adicionar seções de página de Força de Vencimento para Contato, Conta e Oportunidade. Em seguida, repita as etapas de 8 a 10 para adicionar campos de Informações de Vendas para **Contato**. Certifique-se de salvar após qualquer alteração.

## Mapear campos de pessoa personalizados {#map-custom-person-fields}

Os campos de pessoa do Marketo precisam ser mapeados para os campos de contato do Salesforce para garantir que a conversão funcione corretamente. Veja como.

1. Clique em **Configurar**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Procure por &quot;campos&quot; na barra de pesquisa e clique em **Fields** em **Leads**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Clique em **Mapear campos de lead**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Clique na lista suspensa à direita para **Engagement**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Selecione **Contact.Engagement** na lista.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Repita e mapeie esses campos também.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1" rowspan="1">Campo Personalizado de Pessoa do Marketo</th> 
   <th colspan="1" rowspan="1">Campo Personalizado do Contato do Salesforce</th> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Envolvimento</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor relativo da pontuação</p></td> 
   <td colspan="1" rowspan="1"><p>Valor da Pontuação Relativa ao Contact.Relative</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de urgência</p></td> 
   <td colspan="1" rowspan="1"><p>Valor de Contact.Urgency</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Data do Último Momento Interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Data do Último Momento Interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Desc do último momento interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interesting Momento Desc</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Fonte do Último Momento Interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Contact.Last Interesting Moment Source</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Tipo de Último Momento Interessante</p></td> 
   <td colspan="1" rowspan="1"><p>Tipo de Momento de Contato.Último Interessante</p></td> 
  </tr> 
 </tbody> 
</table>

1. Clique em **Salvar** quando terminar.

## Configuração do Marketing to Sales Insight {#marketo-sales-insight-config}

1. Clique em **+** e selecione **Marketo Sales Insight Config**.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Marque **Ativar a API do Marketo**. Em seguida, preencha as [informações de Configuração da API no Marketo Admin](#set-up-marketo-sales-insight). Clique em **Salvar alterações** quando terminar.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >Se o teste de diagnósticos falhar, talvez seja necessário [adicionar mais campos ao layout da página](https://nation.marketo.com/docs/DOC-1115).

E é isso! Você deve conseguir ver os campos de Informações de Vendas do Marketo para Clientes Potenciais, Contatos, Contas e Oportunidades.

![](assets/twenty-six.png)

>[!NOTE]
>
>Para contas, o Sales Insight incluirá todos os emails, mas somente os momentos interessantes mais recentes, a atividade da Web e as alterações de pontuação.

## Acessar informações de vendas do Marketo {#access-marketo-sales-insight}

1. No Salesforce, clique em **+** no final da barra de guias e clique em **Marketo Sales Insight Config**.

1. Marque a caixa de seleção **Ativar API do Marketo** .

1. Copie as credenciais do painel da API Soap na página Admin do Insight de vendas do Marketo e cole-as na seção API Soap da página Configuração do Insight de vendas do Salesforce .

1. Copie as credenciais do painel da Rest API na página Admin do Insight de vendas do Marketo e cole-as na seção Rest API da página Configuração do Insight de vendas do Salesforce .

   ![](assets/access-msi.png)

>[!MORELIKETHIS]
>
>* [Prioridade, urgência, pontuação relativa e melhores propostas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Adicionar guia e botões do Marketo Sales Insight ao Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/bulk-actions/add-marketo-sales-insight-tab-and-buttons-to-salesforce.md)
>* [Configuração do insight de vendas para sua equipe](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)

