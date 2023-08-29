---
unique-page-id: 2360368
description: Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited - Documentação do Marketo - Documentação do produto
title: Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited
exl-id: a33ed396-8d26-403f-b6d8-fe7c55ce76ba
feature: Marketo Sales Insights
source-git-commit: c85f544f2c06a2f5bb92d6e7cad5f801e73fdaed
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 10%

---

# Configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited {#configure-marketo-sales-insight-in-salesforce-enterprise-unlimited}

Estas são as etapas necessárias para configurar o Marketo Sales Insight no Salesforce Enterprise/Unlimited Editions. Vamos começar.

>[!PREREQUISITES]
>
>[Instalar o pacote Marketo Sales Insight no Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)

>[!NOTE]
>
>**Permissões de administrador necessárias**

## Configurar o Sales Insight no Marketo {#configure-sales-insight-in-marketo}

1. Obtenha suas credenciais de MSI no Marketo. Acesse a área Admin e selecione **Sales Insight**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-1.png)

1. Clique em **Editar configuração da API**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-2.png)

1. Insira uma chave secreta de API de sua escolha e clique em **Salvar**. NÃO use um E comercial (&amp;) na chave secreta da API.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-3.png)

   >[!NOTE]
   >
   >Sua chave secreta de API é como uma senha para sua organização e deve ser segura.

1. Clique em **Exibir** no painel Configuração da API Rest para preencher as credenciais.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-4.png)

1. Você verá uma janela pop-up de confirmação. Clique em **OK**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-5.png)

   >[!TIP]
   >
   >Mantenha essa janela aberta. Você precisará dessas informações posteriormente no Salesforce.

## Configurar o Sales Insight no Salesforce {#configure-sales-insight-in-salesforce}

1. No Salesforce, clique em **Configuração**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-6.png)

1. Procure por &quot;local remoto&quot; e selecione **Configurações do site remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-7.png)

1. Clique em **Novo local remoto**.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-8.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoSoapAPI&quot;). Insira o URL do site remoto, que é o URL do host do Marketo no painel Configuração da API Soap no Marketo. Clique em **Salvar**. Agora você criou configurações de site remoto para a API Soap.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-9.png)

1. Clique em **Novo local remoto** novamente.

   ![](assets/configure-marketo-sales-insight-in-salesforce-professional-edition-10.png)

1. Insira o Nome do site remoto (pode ser algo como &quot;MarketoAPI&quot;). Insira o URL do site remoto, que é o URL da API no painel Configuração da API Rest no Marketo. Clique em **Salvar**. Agora você criou configurações de site remoto para a API Rest.

   >[!NOTE]
   >
   >_Você_ escolha o seu **Nome do local remoto** (MarketoAPI é usada aqui). A variável **URL do local remoto** Você pode ser encontrado no campo Host do Marketo da caixa de diálogo Editar configuração da API na Etapa 3 da seção &quot;Configurar o Sales Insight no Marketo&quot;.

## Conceder aos usuários do Sales Insight acesso aos objetos padrão do Salesforce {#grant-sales-insight-users-profile-access}

Devido aos aprimoramentos de segurança do Salesforce, os pacotes do App Exchange não podem mais conceder permissão a objetos padrão, e o acesso precisará ser concedido aos objetos relevantes do Salesforce no perfil do usuário do Salesforce.  Siga as etapas abaixo para conceder as permissões necessárias.

1. Clique em **Configuração**.

1. Pesquise &quot;Perfis&quot; em Localização rápida.

1. Clique em **Editar** ao lado do perfil que seus usuários do Salesforce estão usando.

1. Na seção Permissão de objeto padrão, habilite o acesso de leitura para os seguintes objetos: cliente em potencial, contato, conta e oportunidade.

1. Clique em **Salvar**.

## Personalizar Layouts de Página {#customize-page-layouts}

1. Clique em **Configuração**.

   ![](assets/image2015-5-22-14-3a40-3a39.png)

1. Procure por &quot;layout da página&quot; e selecione o **Layout da página** em **Clientes potenciais**.

   ![](assets/image2015-5-28-14-3a58-3a39.png)

1. Clique em **Visualforce Páginas** à esquerda. Arrastar **Seção** para o layout abaixo da seção Links personalizados.

   ![](assets/image2014-9-24-17-3a32-3a53.png)

1. Insira &quot;Marketo Sales Insight&quot; como o **Nome da seção**. Selecionar **1-coluna** e clique em **OK**.

   ![](assets/image2014-9-24-17-3a33-3a23.png)

1. Arrastar e soltar **Lead** na nova seção.

   ![](assets/image2014-9-24-17-3a33-3a45.png)

   >[!TIP]
   >
   >O nome desta caixa será alterado com base no tipo de objeto. Por exemplo, se você estiver modificando o layout de página para Contatos, ele indicará Contato.

1. Clique duas vezes na guia **Lead** bloco que você acabou de adicionar.

   ![](assets/image2014-9-24-17-3a34-3a0.png)

1. Editar altura para **450** pixels e clique **OK**.

   ![](assets/image2014-9-24-17-3a34-3a26.png)

   >[!NOTE]
   >
   >Marcar **Mostrar barras de rolagem** se você precisar de acesso para rolar pelas atividades.

   >[!TIP]
   >
   >Recomendamos uma altura de 410 pixels para os objetos Contas e Oportunidades.

1. Clique em **Campos** à esquerda. Em seguida, pesquise e arraste o **Urgente** rótulo na caixa **Marketo Sales Insight** layout.

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
      <td>Última atividade do por Vendas</td> 
     </tr> 
     <tr> 
      <td>Último envolvimento do por Vendas</td> 
     </tr> 
     <tr> 
      <td>ID de contato MSI</td> 
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

1. Repita as etapas de 5 a 7 para adicionar seções de página do Visualforce e campos do Sales Insight para **Contato**, **Conta** e **Oportunidade**.

1. Repita as etapas 8 a 10 para adicionar campos do Sales Insight da lista abaixo para **Contato**. Certifique-se de salvar as alterações.

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
      <td>Pontuação de lead MKTO</td> 
     </tr> 
     <tr> 
      <td>Pontuação relativa</td> 
     </tr> 
     <tr> 
      <td>Valor de pontuação relativa</td> 
     </tr> 
     <tr> 
      <td>Sales Insight - abre a página de lista completa de contatos</td> 
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

1. Pesquise por &quot;campos&quot; na barra de pesquisa e clique em **Campos** em **Clientes potenciais**.

   ![](assets/image2015-6-1-9-3a54-3a50.png)

1. Clique em **Mapear campos de lead**.

   ![](assets/image2015-6-1-9-3a58-3a48.png)

1. Clique na lista suspensa à direita de **Envolvimento**.

   ![](assets/image2015-6-1-10-3a9-3a53.png)

1. Selecionar **Contact.Engagement** na lista.

   ![](assets/image2015-6-1-10-3a12-3a11.png)

1. Repita e mapeie esses campos também.

   <table> 
    <tbody> 
     <tr> 
      <th colspan="1" rowspan="1">Campo personalizado da pessoa do Marketo</th> 
      <th colspan="1" rowspan="1">Campo personalizado do contato do Salesforce</th> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Envolvimento</p></td> 
      <td colspan="1" rowspan="1"><p>Contact.Engagement</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valor de pontuação relativa</p></td> 
      <td colspan="1" rowspan="1"><p>Valor da Pontuação de Contact.Relative</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Valor de urgência</p></td> 
      <td colspan="1" rowspan="1"><p>Valor Contact.Urgency</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Data do último momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Data do último momento interessante Contact.Last</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Desc. do último momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Descrição do último momento interessante do Contact.Last</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Fonte do último momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Fonte de momento interessante Contact.Last</p></td> 
     </tr> 
     <tr> 
      <td colspan="1" rowspan="1"><p>Tipo do último momento interessante</p></td> 
      <td colspan="1" rowspan="1"><p>Tipo de momento interessante Contact.Last</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** quando terminar.

## Guia Configuração do Marketo Sales Insight {#marketo-sales-insight-configuration-tab}

1. No Salesforce, clique na guia **+** no final da barra de guias e clique em **Configuração do Marketo Sales Insight**.

1. Copie as credenciais do painel API Soap em [Página do administrador do Sales Insight da Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e cole-os na seção API SOAP da página Configuração do Salesforce Sales Insight.

1. Copie as credenciais do painel API REST em [Página do administrador do Sales Insight da Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md#set-up-marketo-sales-insight){target="_blank"} e cole-os na seção API Rest da página Configuração do Salesforce Sales Insight.

   ![](assets/configure-marketo-sales-insight-in-salesforce-enterprise-edition-25.png)

E é isso! Você poderá ver os campos Marketo Sales Insight para clientes potenciais, contatos, contas e oportunidades.

>[!NOTE]
>
>Se o teste de diagnóstico falhar, talvez seja necessário [adicionar mais campos ao layout da página](https://nation.marketo.com/docs/DOC-1115){target="_blank"}.

>[!NOTE]
>
>Para contas do, o Sales Insight incluirá todos os emails, mas somente os momentos interessantes mais recentes, a atividade da Web e as alterações de pontuação.

>[!MORELIKETHIS]
>
>* [Prioridade, Urgência, Pontuação Relativa e Melhores Opções](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.md)
>* [Adicionar a guia Marketo ao Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-marketo-tab-to-salesforce.md)
>* [Adicionar acesso ao Sales Insight aos perfis](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
