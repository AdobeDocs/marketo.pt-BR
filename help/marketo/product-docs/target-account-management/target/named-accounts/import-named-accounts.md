---
unique-page-id: 12615800
description: Importar contas nomeadas - Documentos do Marketo - Documentação do produto
title: Importar contas nomeadas
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---

# Importar contas nomeadas {#import-named-accounts}

Já tem um CSV cheio de possíveis contas do target? Importe-os diretamente para o TAM!

1. Clique no botão **Novo** e selecione **Importar contas nomeadas**.

   ![](assets/inaone.png)

1. Uma nova janela será aberta. Clique em **Procurar** e selecione o arquivo de contas nomeadas que deseja importar.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >No arquivo , forneça [quanta informação](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) o mais possível. Você só pode adicionar informações firmmográficas; nada que o Marketo calcule (ou seja, pipeline). Para criar contas nomeadas com base em contas CRM, basta exportar o nome da conta e a ID do CRM de seu CRM para um arquivo CSV, usar a opção Nome da conta e mapear a ID do CRM durante o processo de importação. Para vincular adequadamente uma conta CRM a uma conta nomeada, você deve fornecer o nome exato da conta CRM.

1. Escolha entre dois modos de dedupe: Nome da conta ou Nome do domínio. Neste exemplo, vamos escolher Conta. Clique no botão **Modos** e selecione **Por nome de conta**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Se você escolher **Por Modo de Domínio**, a conta nomeada e os campos de domínio devem ser incluídos.

1. Para escolher em qual lista de contas sua conta nomeada é adicionada, clique no botão **Lista de contas** e faça sua seleção.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Você também pode criar uma Lista de contas totalmente nova digitando seu nome na caixa suspensa.

1. Para enviar uma notificação da importação, clique no link **Enviar Alerta para** e selecione um usuário do Marketo. Você _cannot_ insira manualmente um endereço de email.

   ![](assets/inafive-2.png)

1. Clique em **Próximo**.

   ![](assets/inasix-2.png)

1. Mapeie cada campo clicando duas vezes na variável **Campo Marketo** e selecionando o campo apropriado. Clique em **Próximo** quando concluído.

   ![](assets/inaseven.png)

   Sucesso!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Verificar status de importação&quot; mostra apenas os últimos três dias de atividade.

Cenários quando você faz deduplicação por Nome da Conta:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importando registro com o nome de Conta Nomeada existente</strong></td> 
   <td><p>Atualizaremos o registro existente</p></td> 
  </tr> 
  <tr> 
   <td><strong>Importando registro com o novo nome de Conta Nomeada</strong></td> 
   <td>Criaremos um novo registro</td> 
  </tr> 
 </tbody> 
</table>

Cenários quando você faz deduplicação por Nome de Domínio:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importando registro com um novo nome de conta e novo nome de domínio</strong></td> 
   <td>Criaremos uma nova Conta nomeada com as informações fornecidas</td> 
  </tr> 
  <tr> 
   <td><strong>Importando registro com um nome de conta existente e nome de domínio existente</strong></td> 
   <td>Atualizaremos a Conta Nomeada existente</td> 
  </tr> 
   <tr> 
   <td><strong>Importando registro com um novo nome de conta e nome de domínio existente</strong></td> 
   <td>Acrescentaremos o novo nome da conta à Conta Nomeada existente que corresponde ao nome do domínio e atualizará outras informações (ou seja, Setor, Estado etc)</td> 
  </tr> 
  <tr> 
   <td><strong>Importando registro com o nome de conta nomeado existente e o novo nome de domínio</strong></td> 
   <td>Acrescentaremos o novo nome de domínio à Conta Nomeada existente que corresponde ao nome da conta e atualizará outras informações (ou seja, Setor, Estado etc)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando o Marketo anexa uma conta nomeada, estamos atualizando uma regra (em segundo plano) que nos permite identificar pessoas que devem fazer parte da conta nomeada. Exemplo: se você atualizar &quot;IBM&quot; para &quot;IBM, EUA&quot;, as pessoas com qualquer nome de empresa serão associadas à conta nomeada.

Se o Marketo encontrar registros que vemos como duplicatas, processaremos apenas o primeiro.
