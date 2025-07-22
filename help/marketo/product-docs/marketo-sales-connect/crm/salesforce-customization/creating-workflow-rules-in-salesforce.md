---
unique-page-id: 14745823
description: Criação de regras de fluxo de trabalho no Salesforce - Documentação do Marketo - Documentação do produto
title: Criação de regras de fluxo de trabalho no Salesforce
exl-id: 0cfce178-453b-4949-96aa-c327278a267d
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 1%

---

# Criação de regras de fluxo de trabalho no Salesforce {#creating-workflow-rules-in-salesforce}

Ao usar o Marketo Sales Insight (MSI) e o Marketo Sales Connect (MSC) em paralelo, o recurso Melhores Opções de MSI no [!DNL Salesforce] não será atualizado. Todos os outros recursos do MSI funcionam como de costume (visualizar momentos interessantes no iFrame, enviar email, adicionar a campanhas etc.). Este artigo oferece uma solução alternativa para fazer com que as Melhores Opções funcionem novamente.

>[!NOTE]
>
>Isso afeta apenas os clientes que estão usando o **MSI** e o MSE e que desejam usar o recurso Melhores Opções no MSI. Se não precisar/usar as Melhores Opções, você poderá desconsiderá-las.

## Introdução {#getting-started}

A solução alternativa inclui a criação de novas regras de fluxo de trabalho para copiar valores de novos campos do MSE para os campos do MSI antigos. Você precisará criar quatro regras de fluxo de trabalho para o objeto de Contato e as mesmas quatro regras de fluxo de trabalho para o objeto de Cliente potencial na sua própria instância [!DNL Salesforce]. Isso pode exigir que você tenha direitos de Administrador do CRM (dependendo de sua função e configuração no CRM).

Abaixo estão os nomes recomendados das regras de workflow e a descrição de cada uma. Estes se aplicam aos objetos [!UICONTROL Contato] e [!UICONTROL Lead]:

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

1. Depois de clicar em **[!UICONTROL Configuração]**, procure por **Fluxo de Trabalho** e selecione **[!UICONTROL Regras de Fluxo de Trabalho]**.

   ![](assets/one-1.png)

1. Selecione **[!UICONTROL Nova regra]**.

   ![](assets/two-1.png)

1. Clique no menu suspenso [!UICONTROL Objeto], selecione **[!UICONTROL Cliente em potencial]** e clique em **[!UICONTROL Avançar]**.

   ![](assets/three-1.png)

1. Insira &quot;Atualizar campo Desc. Momento Interessante&quot; como o [!UICONTROL Nome da Regra]. Selecione o botão de opção **[!UICONTROL criado e sempre que for editado]**. No menu suspenso [!UICONTROL Critérios da Regra], selecione **[!UICONTROL fórmula que é avaliada como verdadeira]**. Procure e selecione a função ISCHANGED. Em seguida, destaque o valor do campo padrão e clique em **[!UICONTROL Inserir Campo]**.

   ![](assets/four-1.png)

1. Na janela pop-up &quot;[!UICONTROL Inserir campo]&quot;, escolha **[!UICONTROL Última descrição do compromisso do Marketo]** e clique em **[!UICONTROL Inserir]**.

   ![](assets/five-1.png)

1. Clique em **[!UICONTROL Salvar e Avançar]**.

   ![](assets/6.png)

1. No menu suspenso [!UICONTROL Adicionar ação de fluxo de trabalho], selecione **[!UICONTROL Nova atualização de campo]**.

   ![](assets/seven.png)

1. No campo [!UICONTROL Nome], digite &quot;Atualizar Campo Desc. Momento Interessante&quot; ([!UICONTROL Nome Exclusivo] será gerado automaticamente). No menu suspenso [!UICONTROL Campo a Atualizar], escolha **[!UICONTROL Última Descrição de Momento Interessante]**. Selecione o botão de opção **[!UICONTROL Usar uma fórmula para definir o novo valor]** e clique em **[!UICONTROL Mostrar Editor de Fórmulas]**.

   ![](assets/eight.png)

1. Clique no botão **[!UICONTROL Inserir Campo]**.

   ![](assets/9a.png)

1. Selecione **[!UICONTROL Última Descrição do Envolvimento do Marketo]** e clique em **[!UICONTROL Inserir]**. Na próxima página, clique em **[!UICONTROL Salvar]**.

   ![](assets/nine.png)

1. Clique em **[!UICONTROL Concluído]**.

   ![](assets/twelve.png)

1. Clique em **[!UICONTROL Ativar]** para ativar a regra de fluxo de trabalho.

   ![](assets/thirteen.png)

   Após a última etapa, você pode optar por clonar a regra de fluxo de trabalho para os outros campos listados na seção [!UICONTROL Introdução]: Descrição, Tipo, Source, Data. Após concluir as quatro regras de fluxo de trabalho no objeto [!UICONTROL Contato], repita o mesmo procedimento para o objeto [!UICONTROL Lead].
