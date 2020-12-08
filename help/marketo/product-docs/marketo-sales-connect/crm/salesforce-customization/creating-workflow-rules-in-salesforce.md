---
unique-page-id: 14745823
description: Criação de regras de fluxo de trabalho no Salesforce - Documentos do Marketing - Documentação do produto
title: Criação de regras de fluxo de trabalho no Salesforce
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---


# Criação de regras de fluxo de trabalho no Salesforce {#creating-workflow-rules-in-salesforce}

Ao usar o Marketing Cloud Sales Insight (MSI) e o Markto Sales Connect (MSC) em paralelo, o recurso de Melhores Apostas MSI no Salesforce não será atualizado. Todos os outros recursos MSI funcionam como de costume (exibindo momentos interessantes no iFrame, enviando e-mail, adicionando ao campanha etc.). Este artigo oferta uma solução alternativa para que as Melhores Propostas funcionem novamente.

>[!NOTE]
>
>Isso só afeta os clientes que estão usando **MSI e MSE, e que desejam usar o recurso Melhores** propostas no MSI. Se você não precisar/usar as Melhores Apostas, poderá ignorar.

## Introdução {#getting-started}

A solução alternativa inclui a criação de novas regras de fluxo de trabalho para copiar valores de novos campos MSE para os campos MSI antigos. Você precisará criar quatro regras de fluxo de trabalho para o objeto Contact e as mesmas quatro regras de fluxo de trabalho para o objeto Lead na sua própria instância do Salesforce. Isso pode exigir que você tenha direitos de Administrador do CRM (dependendo de sua função e configuração no CRM).

Abaixo estão os nomes recomendados das regras de fluxo de trabalho e a descrição de cada uma. Eles se aplicam ao objeto Contato e Cliente potencial:

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Atualizar Campo Desc de Momento Interessante</td> 
   <td><p>Copiar de: Último<br>DescCopy de Envolvimento do Marketing para: Desc do último momento interessante</p></td> 
  </tr> 
  <tr> 
   <td>Atualizar campo Tipo de Momento Interessante</td> 
   <td><p>Copiar de: Último<br>Tipo de Envolvimento do Marketing para: Último Tipo de Momento Interessante</p></td> 
  </tr> 
  <tr> 
   <td>Atualizar campo Fonte de Momento Interessante</td> 
   <td><p>Copiar de: Último<br>Cópia de Envolvimento do Marketing para: Origem do Último Momento Interessante</p></td> 
  </tr> 
  <tr> 
   <td>Atualizar campo Data de Momento Interessante</td> 
   <td><p>Copiar de: Última<br>Data de Envolvimento do Marketing para: Data do Último Momento Interessante</p></td> 
  </tr> 
 </tbody> 
</table>

## Instruções {#instructions}

1. Depois de clicar em **Configurar**, procure **Fluxo de trabalho** e selecione Regras **** de fluxo de trabalho.

   ![](assets/one-1.png)

1. Selecione **Nova regra**.

   ![](assets/two-1.png)

1. Clique na lista suspensa Objeto e selecione **Cliente potencial** e clique em **Avançar**.

   ![](assets/three-1.png)

1. Digite &quot;Atualizar campo de descrição de momento interessante&quot; como o nome da regra. Selecione o botão de opção **criado e sempre que ele for editado**. Na lista suspensa Critérios da regra, selecione a **fórmula avaliada como true**. Procure e selecione a função ISCHANGED. Em seguida, realce o valor do campo padrão e clique em **Inserir campo**.

   ![](assets/four-1.png)

1. No pop-up &quot;Inserir campo&quot;, escolha **Último segmento de marketing para a descrição** de envolvimento e clique em **Inserir**.

   ![](assets/five-1.png)

1. Clique em **Salvar e próximo**.

   ![](assets/6.png)

1. Na lista suspensa Adicionar ação do fluxo de trabalho, selecione **Nova atualização** de campo.

   ![](assets/seven.png)

1. No campo Nome, digite &quot;Atualizar campo de descrição de momento interessante&quot; (o nome exclusivo será gerado automaticamente). No menu suspenso Campo para atualizar, escolha Desc. **Último momento interessante**. Selecione o botão de opção **Usar uma fórmula para definir um novo valor** e clique em **Mostrar editor** de fórmulas.

   ![](assets/eight.png)

1. Clique no botão **Inserir campo** .

   ![](assets/9a.png)

1. Selecione **Último segmento de marketing** e clique em **Inserir**. Na próxima página, clique em **Salvar**.

   ![](assets/nine.png)

1. Clique em **Concluído**.

   ![](assets/twelve.png)

1. Clique em **Ativar** para ativar a regra de fluxo de trabalho.

   ![](assets/thirteen.png)

   Após a última etapa, você pode optar por clonar a regra de fluxo de trabalho para os outros campos listados na seção Introdução: Descrição, Tipo, Origem, Data. Depois de concluir as quatro regras de fluxo de trabalho no objeto Contact, repita o mesmo para o objeto Lead.

