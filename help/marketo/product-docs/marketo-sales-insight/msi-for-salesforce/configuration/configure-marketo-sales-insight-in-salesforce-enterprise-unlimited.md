---
unique-page-id: 2360368
description: Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited - Documentos da Marketo - Documentação do produto
title: Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 12%

---

# Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Estas são as etapas que você precisa seguir para configurar o Marketo Sales Insight nas Edições Enterprise/Unlimited do Salesforce. Vamos começar.

>[!PREREQUISITES]
>
>[Instalar o pacote de informações de vendas da Marketo no Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Configurar o Sales Insight no Marketo {#configure-sales-insight-in-marketo}

1. Obtenha suas credenciais do MSI no Marketo. Acesse a área Admin e selecione **Insight de vendas**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Clique em **Editar configuração da API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Insira uma chave secreta de API de sua escolha e clique em **Salvar**. NÃO use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >Sua chave secreta da API é como uma senha para sua organização e deve ser segura.

1. Clique em **Exibir** no painel Configuração da Rest API para preencher as credenciais.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Você verá um pop-up de confirmação. Clique em **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Mantenha essa janela aberta. Você precisará dessas informações mais tarde no Salesforce.

## Configurar o Sales Insight no Salesforce {#configure-sales-insight-in-salesforce}

1. No Salesforce, clique em **Configuração**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Procure por &quot;site remoto&quot; e selecione **Configurações de local remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Clique em **Novo local remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoSoapAPI&quot;). Insira o URL do site remoto, que é o URL do host do Marketo no painel Configuração da API Soap no Marketo. Clique em **Salvar**. Agora você criou configurações do site remoto para a API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Clique em **Novo local remoto** novamente.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoAPI&quot;). Insira o URL do site remoto, que é o URL da sua API do painel Configuração da API restante no Marketo. Clique em **Salvar**. Agora você criou configurações de site remoto para a API Rest.

   >[!NOTE]
   >
   >_Você_ escolha sua **Nome do local remoto** (A API do Marketo é usada aqui). O **URL de local remoto** O pode ser encontrado no campo Host do Marketo da caixa de diálogo Editar configuração da API da etapa 3 da seção &quot;Configurar insight de vendas no Marketo&quot;.

## Personalizar layouts de página {#customize-page-layouts}

1. Clique em **Configuração**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Procure por &quot;layout de página&quot; e selecione o **Layout da página** under **Clientes potenciais**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Clique em **Páginas da força de visita** à esquerda. Arrastar **Seção** para o layout na seção Links personalizados .

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Digite &quot;Marketo Sales Insight&quot; como o **Nome da seção**. Selecionar **1-Coluna** e clique em **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arrastar e soltar **Líder** na nova seção.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >O nome dessa caixa será alterado com base no tipo de objeto. Por exemplo, se você estiver modificando o layout da página para Contatos, isso dirá Contato.

1. Clique duas vezes no **Líder** bloco que acabou de adicionar.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Editar altura para **450** pixels e clique **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!TIP]
   >
   >Recomendamos uma altura de 410 pixels para os objetos Contas e Oportunidades.

1. Clique em **Campos** à esquerda. Em seguida, pesquise e arraste a **Urgência** no **Insight sobre vendas da Marketo** layout.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-18.png)

1. Repita a etapa acima também para esses campos.

   <table> 
    <tbody> 
     <tr> 
      <td>Último momento interessante</td> 
     </tr> 
     <tr> 
      <td>Data do último momento interessante</td> 
     </tr> 
     <tr> 
      <td>Desc. do último momento interessante</td> 
     </tr> 
     <tr> 
      <td>Fonte do último momento interessante</td> 
     </tr> 
     <tr> 
      <td>Tipo do último momento interessante</td> 
     </tr> 
     <tr> 
      <td>Última atividade do Marketo no Sales</td> 
     </tr> 
     <tr> 
      <td>Último envolvimento do Marketo no Sales</td> 
     </tr> 
     <tr> 
      <td>Id de Contato MSI</td> 
     </tr> 
     <tr> 
      <td>Pontuação relativa</td> 
     </tr> 
     <tr> 
      <td>Valor de pontuação relativa</td> 
     </tr> 
     <tr> 
      <td>Urgência</td> 
     </tr> 
     <tr> 
      <td>Valor de urgência</td> 
     </tr> 
     <tr> 
      <td>Exibir no Marketo</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** quando terminar.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita as etapas de 5 a 7 para adicionar seções de página de Força Visual e campos de Insight de Vendas para **Contato**, **Conta** e **Oportunidade**.

1. Repita as etapas de 8 a 10 para adicionar campos de informações de vendas da lista abaixo para **Contato**. Certifique-se de salvar as alterações.

<table> 
    <tbody> 
     <tr> 
      <td>Último momento interessante</td> 
     </tr> 
     <tr> 
      <td>Data do último momento interessante</td> 
     </tr> 
     <tr> 
      <td>Desc. do último momento interessante</td> 
     </tr> 
     <tr> 
      <td>Fonte do último momento interessante</td> 
     </tr> 
     <tr> 
      <td>Tipo do último momento interessante</td> 
     </tr> 
     <tr> 
      <td>Última atividade do Marketo no Sales</td> 
     </tr> 
     <tr> 
      <td>Último envolvimento do Marketo no Sales</td> 
     </tr> 
     <tr> 
      <td>Pontuação de lead da MKTO</td> 
     </tr> 
     <tr> 
      <td>Pontuação relativa</td> 
     </tr> 
     <tr> 
      <td>Valor de pontuação relativa</td> 
     </tr> 
     <tr> 
      <td>Insight de vendas - abre a página da lista completa do contato</td> 
     </tr> 
     <tr> 
      <td>Urgência</td> 
     </tr> 
     <tr> 
      <td>Valor de urgência</td> 
     </tr> 
    </tbody> 
   </table>

## Mapear campos de pessoa personalizados {#map-custom-person-fields}

Os campos de pessoa do Marketo precisam ser mapeados para campos de contato do Salesforce para garantir que a conversão funcione corretamente. Veja como.

1. Clique em **Configuração**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Procure por &quot;campos&quot; na barra de pesquisa e clique em **Campos** under **Clientes potenciais**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Clique em **Mapear campos de lead**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Clique na lista suspensa à direita para **Envolvimento**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Selecionar **Contact.Engagement** na lista.

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
      <td colspan="1" rowspan="1"><p>Valor de pontuação relativa</p></td> 
      <td colspan="1" rowspan="1"><p>Valor da Pontuação Relativa ao Contact.Relative</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valor de urgência</p></td> 
      <td colspan="1" rowspan="1"><p>Valor de Contact.Urgency</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Data do último momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Data do Último Momento Interessante</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Desc. do último momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interesting Momento Desc</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Fonte do último momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Last Interesting Moment Source</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Tipo do último momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Tipo de Momento de Contato.Último Interessante</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** quando terminar.

## Config. do Marketo Sales Insight {#marketo-sales-insight-config}

1. Clique em **+** e depois selecione **Configuração do Marketo Sales Insight**.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Verificar **Habilitar a API do Marketo**. Em seguida, preencha o [Informações de configuração da API no Marketo Admin](#set-up-marketo-sales-insight). Clique em **Salvar alterações** quando terminar.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >Se o teste de diagnóstico falhar, talvez seja necessário [adicionar mais campos ao layout da página](https://nation.marketo.com/docs/DOC-1115).

E é isso! Você deve conseguir ver os campos Marketo Sales Insight para Clientes potenciais, Contatos, Contas e Oportunidades.

![](assets/twenty-six.png)

>[!NOTE]
>
>Para contas, o Sales Insight incluirá todos os emails, mas somente os momentos interessantes mais recentes, a atividade da Web e as alterações de pontuação.

## Acessar Marketo Sales Insight {#access-marketo-sales-insight}

1. No Salesforce, clique no botão **+** no final da barra de guias e clique em **Configuração do Marketo Sales Insight**.

1. Selecione o **Habilitar a API do Marketo** caixa de seleção.

1. Copie as credenciais do painel da API Soap na página de administração do Insight de vendas da Marketo e cole-as na seção API Soap da página Configuração do Insight de vendas do Salesforce .

1. Copie as credenciais do painel da Rest API na página do Administrador do Insight de vendas da Marketo e cole-as na seção Rest API da página Configuração do Insight de vendas do Salesforce .

   ![](assets/access-msi.png)

>[!MORELIKETHIS]
>
>* [Prioridade, urgência, pontuação relativa e melhores propostas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Adicionar a guia Marketo ao Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Adicionar acesso ao insight de vendas a perfis](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}

