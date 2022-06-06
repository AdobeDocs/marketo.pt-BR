---
unique-page-id: 3571743
description: Configurar o Marketo Sales Insight no Salesforce Professional Edition - Documentos da Marketo - Documentação do produto
title: Configurar o Marketo Sales Insight no Salesforce Professional Edition
exl-id: fae63560-0bb3-46a9-94a3-cc27c1aa363e
source-git-commit: bb172e59e96cca3e8997615a2f1367ecccf700ed
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 5%

---

# Configurar o Marketo Sales Insight no Salesforce Professional Edition {#configure-marketo-sales-insight-in-salesforce-professional-edition}

Estas são as etapas necessárias para configurar o Marketo Sales Insight no Salesforce Professional Edition. Vamos começar.

>[!PREREQUISITES]
>
>* Instale o Marketo no Salesforce Professional Edition.
>
>* [Instalar o pacote de informações de vendas da Marketo no Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)


>[!NOTE]
>
>**Permissões de administrador necessárias**

## Configurar o Sales Insight no Marketo {#configure-sales-insight-in-marketo}

1. Abra uma nova janela do navegador para obter as credenciais do Marketo Sales Insight de sua conta do Marketo.
1. Acesse a área Admin e selecione **Insight de vendas**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1-1.png)

1. Clique em **Editar configuração da API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2-1.png)

1. Insira uma chave secreta de API de sua escolha e clique em **Salvar**. NÃO use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3-1.png)

   >[!NOTE]
   >
   >Sua chave secreta da API é como uma senha para sua organização e deve ser segura.

1. Clique em **Exibir** no painel Configuração da Rest API para preencher as credenciais.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4-1.png)

1. Você verá um pop-up de confirmação. Clique em **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5-1.png)

## Configurar o Sales Insight no Salesforce {#configure-sales-insight-in-salesforce}

1. No Salesforce, clique em **Configuração**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6-1.png)

1. Procure por &quot;site remoto&quot; e selecione **Configurações de local remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7-1.png)

1. Clique em **Novo local remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8-1.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoSoapAPI&quot;). Insira o URL do site remoto, que é o URL do host do Marketo no painel Configuração da API Soap no Marketo. Clique em **Salvar**. Agora você criou configurações do site remoto para a API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9-1.png)

1. Clique em **Novo local remoto** novamente.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10-1.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoRestAPI&quot;). Insira o URL do site remoto, que é o URL da sua API do painel Configuração da API restante no Marketo. Clique em **Salvar**. Agora você criou configurações de site remoto para a API Rest.

## Configurar o Marketo Sales Insight {#set-up-marketo-sales-insight}

1. Faça logon na instância do Marketo e clique em **Administrador**.

   ![](assets/login-admin-1.png)

1. Clique em **Insight de vendas**.

   ![](assets/image2015-5-22-15-3a12-3a33-1.png)

1. Clique em **Editar configuração da API**.

   ![](assets/image2015-5-22-15-3a15-3a0-1.png)

1. Insira um **Chave secreta da API** e clique em **Salvar**.

   >[!CAUTION]
   >
   >Não use um E comercial (&amp;) em sua Chave secreta da API.

   ![](assets/image2015-5-27-16-3a36-3a56-1.png)

   >[!TIP]
   >
   >Mantenha essa janela aberta. Você precisará dessas informações posteriormente no Salesforce.

1. Volte para o Salesforce e clique em **Configuração**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Procure por &quot;site remoto&quot; e clique em **Configuração de local remoto** under **Controles de segurança**.

   ![](assets/image2014-9-24-17-3a25-3a52.png)

1. Clique em **Novo local remoto**.

   ![](assets/image2014-9-24-17-3a26-3a6.png)

1. Enter **Nome do local remoto** e **URL de local remoto**, depois clique em **Salvar**.

   ![](assets/remote-site-1.png)

   >[!NOTE]
   >
   >Você escolhe o seu **Nome do local remoto** (A API do Marketo é usada aqui). O **URL de local remoto** O pode ser encontrado no campo Host do Marketo da caixa de diálogo Editar configuração da API da etapa 4.

## Personalizar layouts de página {#customize-page-layouts}

1. Clique em **Configuração**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Procure por &quot;layout de página&quot; e selecione o **Layout da página** under **Clientes potenciais**.

   ![](assets/image2015-5-28-14-3a58-3a39-1.png)

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

   >[!NOTE]
   >
   >Verificar **Mostrar barras de rolagem** se você precisar acessar atividades de rolagem.

   >[!TIP]
   >
   >Recomendamos uma altura de 410 pixels para os objetos Contas e Oportunidades.

1. Clique em **Campos** à esquerda. Em seguida, pesquise e arraste a **Envolvimento** no **Insight sobre vendas da Marketo** layout.

   ![](assets/image2015-5-22-16-3a32-3a46-1.png)

1. Repita a etapa acima também para esses campos.

<table> 
 <tbody> 
  <tr> 
   <td colspan="1">Envolvimento</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de pontuação relativa</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Valor de urgência</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Data do último momento interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Desc. do último momento interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Fonte do último momento interessante</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p>Tipo do último momento interessante</p></td> 
  </tr> 
 </tbody> 
</table>

1. lamber **Salvar** quando terminar.

   ![](assets/image2014-9-24-17-3a35-3a6.png)

1. Repita esse processo para adicionar seções de página de Força de Visita e campos de Insight de Vendas para **Contato**, **Conta** e **Oportunidade**.
1. Repita as etapas 5 a 7 para adicionar seções de página de Força de Vencimento para Contato, Conta e Oportunidade. Em seguida, repita as etapas de 8 a 10 para adicionar campos de Insight de vendas para **Contato**. Certifique-se de salvar após qualquer alteração.

## Mapear campos de pessoa personalizados {#map-custom-person-fields}

Os campos de pessoa do Marketo precisam ser mapeados para campos de contato do Salesforce para garantir que a conversão funcione corretamente. Veja como.

1. Clique em **Configuração**.

   ![](assets/image2015-5-22-14-3a40-3a39-1.png)

1. Procure por &quot;campos&quot; na barra de pesquisa e clique em **Campos** under **Clientes potenciais**.

   ![](assets/image2015-6-1-9-3a54-3a50-1.png)

1. Clique em **Mapear campos de lead**.

   ![](assets/image2015-6-1-9-3a58-3a48-1.png)

1. Clique na lista suspensa à direita para **Envolvimento**.

   ![](assets/image2015-6-1-10-3a9-3a53-1.png)

1. Selecionar **Contact.Engagement** na lista.

   ![](assets/image2015-6-1-10-3a12-3a11-1.png)

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

   ![](assets/image2014-9-24-17-3a37-3a17.png)

## Config. do Marketo Sales Insight {#marketo-sales-insight-config}

1. Clique em **+** e depois selecione **Configuração do Marketo Sales Insight**.

   ![](assets/image2014-9-24-17-3a37-3a45.png)

1. Verificar **Habilitar a API do Marketo**. Em seguida, preencha o [Informações de configuração da API no Marketo Admin](#set-up-marketo-sales-insight). Clique em **Salvar alterações** quando terminar.

   ![](assets/image2014-9-24-17-3a38-3a0.png)

   >[!NOTE]
   >
   >Se o teste de diagnóstico falhar, talvez seja necessário [adicionar mais campos ao layout da página](https://nation.marketo.com/docs/DOC-1115).

E é isso! Você deve conseguir ver os campos Marketo Sales Insight para Clientes potenciais, Contatos, Contas e Oportunidades.

![](assets/twenty-six-1.png)

>[!NOTE]
>
>Para contas, o Sales Insight incluirá todos os emails, mas somente os momentos interessantes mais recentes, a atividade da Web e as alterações de pontuação.

## Acessar Marketo Sales Insight {#access-marketo-sales-insight}

1. No Salesforce, clique no botão **+** no final da barra de guias e clique em **Configuração do Marketo Sales Insight**.

1. Selecione o **Habilitar a API do Marketo** caixa de seleção.

1. Copie as credenciais do painel da API Soap na página de administração do Insight de vendas da Marketo e cole-as na seção API Soap da página Configuração do Insight de vendas do Salesforce .

1. Copie as credenciais do painel da Rest API na página do Administrador do Insight de vendas da Marketo e cole-as na seção Rest API da página Configuração do Insight de vendas do Salesforce .

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-27.png)

>[!MORELIKETHIS]
>
>* [Prioridade, urgência, pontuação relativa e melhores propostas](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Adicionar a guia Marketo ao Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Adicionar acesso ao insight de vendas a perfis](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;}

