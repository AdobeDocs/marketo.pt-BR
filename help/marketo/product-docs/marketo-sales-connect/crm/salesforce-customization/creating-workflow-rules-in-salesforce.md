---
unique-page-id: 14745823
description: Criação de regras de fluxo de trabalho no Salesforce - Documentação do Marketo - Documentação do produto
title: Criação de regras de fluxo de trabalho no Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Criação de regras de fluxo de trabalho no Salesforce {#creating-workflow-rules-in-salesforce}

Ao usar o Marketo Sales Insight (MSI) e o Marketo Sales Connect (MSC) em paralelo, o recurso Melhores opções de MSI no Salesforce não será atualizado. Todos os outros recursos do MSI funcionam como de costume (visualizar momentos interessantes no iFrame, enviar email, adicionar a campanhas etc.). Este artigo oferece uma solução alternativa para fazer com que as Melhores Opções funcionem novamente.

>[!NOTE]
>
>Isso afeta apenas os clientes que estão usando o **MSI** e o MSE e que desejam usar o recurso Melhores Opções no MSI. Se não precisar/usar as Melhores Opções, você poderá desconsiderá-las.

## Introdução {#getting-started}

A solução alternativa inclui a criação de novas regras de fluxo de trabalho para copiar valores de novos campos do MSE para os campos do MSI antigos. Você precisará criar quatro regras de fluxo de trabalho para o objeto Contact e as mesmas quatro regras de fluxo de trabalho para o objeto Lead em sua própria instância do Salesforce. Isso pode exigir que você tenha direitos de Administrador do CRM (dependendo de sua função e configuração no CRM).

Abaixo estão os nomes recomendados das regras de workflow e a descrição de cada uma. Isso se aplica aos objetos Contato e Cliente Potencial:

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td>Atualizar Campo Desc. Momento Interessante</td> 
   <td><p>Copiar de: Última descrição do Marketo Engagement <br>Copiar para: Última descrição do momento interessante</p></td> 
  </tr> 
  <tr> 
   <td>Atualizar campo Tipo de momento interessante</td> 
   <td><p>Copiar de: Último tipo de envolvimento do Marketo<br>Copiar para: Último tipo de momento interessante</p></td> 
  </tr> 
  <tr> 
   <td>Atualizar campo Source de momento interessante</td> 
   <td><p>Copiar de: Último Marketo Engagement Source<br>Copiar para: Último momento interessante Source</p></td> 
  </tr> 
  <tr> 
   <td>Atualizar campo Data de Momento Interessante</td> 
   <td><p>Copiar de: Última data de compromisso do Marketo<br>Copiar para: Última data de momento interessante</p></td> 
  </tr> 
 </tbody> 
</table>

## Instruções {#instructions}

1. Depois de clicar em **Configuração**, procure por **Fluxo de Trabalho** e selecione **Regras de Fluxo de Trabalho**.

   ![](assets/one-1.png)

1. Selecione **Nova regra**.

   ![](assets/two-1.png)

1. Clique na lista suspensa Objeto, selecione **Lead** e clique em **Avançar**.

   ![](assets/three-1.png)

1. Insira &quot;Atualizar campo Desc. Momento Interessante&quot; como o Nome da regra. Selecione o botão de opção **criado e sempre que for editado**. Na lista suspensa Critérios da Regra, selecione **fórmula avaliada como verdadeira**. Procure e selecione a função ISCHANGED. Em seguida, destaque o valor do campo padrão e clique em **Inserir Campo**.

   ![](assets/four-1.png)

1. Na janela pop-up &quot;Inserir campo&quot;, escolha **Última descrição do Marketo Engagement** e clique em **Inserir**.

   ![](assets/five-1.png)

1. Clique em **Salvar e Avançar**.

   ![](assets/6.png)

1. No menu suspenso Adicionar ação de fluxo de trabalho, selecione **Nova atualização de campo**.

   ![](assets/seven.png)

1. No campo Nome, digite &quot;Atualizar campo de descrição do momento interessante&quot; (nome exclusivo será gerado automaticamente). No menu suspenso Campo para Atualização, escolha **Última Descrição de Momento Interessante**. Selecione o botão de opção **Usar uma fórmula para definir o novo valor** e clique em **Mostrar Editor de Fórmulas**.

   ![](assets/eight.png)

1. Clique no botão **Inserir Campo**.

   ![](assets/9a.png)

1. Selecione **Última Descrição do Envolvimento do Marketo** e clique em **Inserir**. Na próxima página, clique em **Salvar**.

   ![](assets/nine.png)

1. Clique em **Concluído**.

   ![](assets/twelve.png)

1. Clique em **Ativar** para ativar a regra de fluxo de trabalho.

   ![](assets/thirteen.png)

   Após a última etapa, você pode optar por clonar a regra de fluxo de trabalho para os outros campos listados na seção Introdução: Desc, Type, Source, Date. Depois de concluir as quatro regras de fluxo de trabalho no objeto Contact, repita o mesmo procedimento para o objeto Lead.
