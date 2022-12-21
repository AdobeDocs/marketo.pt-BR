---
unique-page-id: 14745823
description: Criação de regras de fluxo de trabalho no Salesforce - Documentos do Marketo - Documentação do produto
title: Criação de regras de fluxo de trabalho no Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Criação de regras de fluxo de trabalho no Salesforce {#creating-workflow-rules-in-salesforce}

Ao usar o Marketo Sales Insight (MSI) e a Marketo Sales Connect (MSC) em paralelo, o recurso MSI Best Bets (Melhores Melhores Ocorrências) no Salesforce não será atualizado. Todos os outros recursos MSI funcionam como de costume (visualizando momentos interessantes no iFrame, enviando email, adicionando a campanhas etc.). Este artigo oferece uma solução alternativa para que as Melhores Propostas funcionem novamente.

>[!NOTE]
>
>Isso afeta apenas os clientes que usam **both** MSI e MSE, e que desejam usar o recurso Melhores Propostas no MSI. Se você não precisar/usar as Melhores Práticas, poderá ignorar.

## Introdução {#getting-started}

A solução alternativa inclui a criação de novas regras de fluxo de trabalho para copiar valores de novos campos MSE para campos MSI antigos. Você precisará criar quatro regras de workflow para o objeto Contact e as mesmas quatro regras de workflow para o objeto Lead na sua própria instância do Salesforce. Isso pode exigir que você tenha direitos de administrador do CRM (dependendo de sua função e configuração no CRM).

Abaixo estão os nomes recomendados das regras de fluxo de trabalho e a descrição de cada uma. Isso se aplica ao objeto Contato e Cliente Potencial:

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Atualizar Campo Desc de Momento Interessante</td> 
   <td><p>Copiar de: Último Desc de Envolvimento do Marketo<br>Copiar para: Desc do último momento interessante</p></td> 
  </tr> 
  <tr> 
   <td>Campo Atualizar Tipo de Momento Interessante</td> 
   <td><p>Copiar de: Último tipo de envolvimento do Marketo<br>Copiar para: Tipo de Último Momento Interessante</p></td> 
  </tr> 
  <tr> 
   <td>Atualizar campo Origem de Momento Interessante</td> 
   <td><p>Copiar de: Última origem de envolvimento do Marketo<br>Copiar para: Fonte do Último Momento Interessante</p></td> 
  </tr> 
  <tr> 
   <td>Atualizar campo Data de Momento Interessante</td> 
   <td><p>Copiar de: Última data de envolvimento do Marketo<br>Copiar para: Data do Último Momento Interessante</p></td> 
  </tr> 
 </tbody> 
</table>

## Instruções {#instructions}

1. Depois de clicar **Configuração**, pesquisar por **Fluxo de trabalho** e selecione **Regras de fluxo de trabalho**.

   ![](assets/one-1.png)

1. Selecionar **Nova regra**.

   ![](assets/two-1.png)

1. Clique no menu suspenso Objeto e selecione **Líder**, depois clique em **Próximo**.

   ![](assets/three-1.png)

1. Insira &quot;Update Interesting Moment Desc Field&quot; como o Nome da regra. Selecione o botão de opção **criado e sempre que for editado**. Na lista suspensa Critérios da regra , selecione **fórmula resulta em verdadeiro**. Procure e selecione a função ISCHANGED . Em seguida, realce o valor padrão do campo e clique em **Inserir campo**.

   ![](assets/four-1.png)

1. Na janela pop-up &quot;Inserir campo&quot;, escolha **Último Desc de Envolvimento do Marketo** e clique em **Inserir**.

   ![](assets/five-1.png)

1. Clique em **Salvar e Próximo**.

   ![](assets/6.png)

1. Na lista suspensa Adicionar ação do fluxo de trabalho , selecione **Nova atualização de campo**.

   ![](assets/seven.png)

1. No campo Nome , digite &quot;Atualizar campo de descrição do momento interessante&quot; (o nome exclusivo será gerado automaticamente). No menu suspenso Field to Update (Campo a ser atualizado), escolha **Desc do último momento interessante**. Selecione o **Usar uma fórmula para definir um novo valor** botão de opção, em seguida, clique em **Mostrar Editor de Fórmulas**.

   ![](assets/eight.png)

1. Clique no botão **Inserir campo** botão.

   ![](assets/9a.png)

1. Selecionar **Último Desc de Envolvimento do Marketo** e clique em **Inserir**. Na próxima página, clique em **Salvar**.

   ![](assets/nine.png)

1. Clique em **Concluído**.

   ![](assets/twelve.png)

1. Clique em **Ativar** para ativar a regra de fluxo de trabalho.

   ![](assets/thirteen.png)

   Após a última etapa, você pode optar por clonar a regra de fluxo de trabalho para os outros campos listados na seção Introdução : Desc, Tipo, Fonte, Data. Depois de concluir as quatro regras de fluxo de trabalho no objeto Contato, repita o mesmo para o objeto Lead.
