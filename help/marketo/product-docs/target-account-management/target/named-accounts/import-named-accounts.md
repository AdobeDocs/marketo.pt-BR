---
unique-page-id: 12615800
description: Importar contas nomeadas - Documentos do Marketo - Documentação do produto
title: Importar contas nomeadas
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---


# Importar contas nomeadas {#import-named-accounts}

Já tem um CSV cheio de possíveis contas do target? Importe-os diretamente para o TAM!

1. Clique no menu suspenso **New** e selecione **Import Named Accounts**.

   ![](assets/inaone.png)

1. Uma nova janela será aberta. Clique em **Procurar** e selecione o arquivo de contas nomeadas que deseja importar.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >No arquivo , forneça [a maior quantidade de informações](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) possível. Você só pode adicionar informações firmmográficas; nada que o Marketo calcule (ou seja, pipeline). Para criar contas nomeadas com base em contas CRM, basta exportar o nome da conta e a ID do CRM de seu CRM para um arquivo CSV, usar a opção Nome da conta e mapear a ID do CRM durante o processo de importação. Para vincular adequadamente uma conta CRM a uma conta nomeada, você deve fornecer o nome exato da conta CRM.

1. Escolha entre dois modos de dedupe: Nome da conta ou Nome do domínio. Neste exemplo, vamos escolher Conta. Clique no menu suspenso **Modos** e selecione **Por nome de conta**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Se você escolher **By Domain Mode**, a conta nomeada e os campos de domínio deverão ser incluídos.

1. Para escolher a lista de contas à qual sua conta nomeada é adicionada, clique no menu suspenso **Lista de Contas** e faça sua seleção.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Você também pode criar uma Lista de contas totalmente nova digitando seu nome na caixa suspensa.

1. Para enviar uma notificação da importação, clique no menu suspenso **Enviar alerta para** e selecione um usuário do Marketo. Você _não pode_ inserir manualmente um endereço de email.

   ![](assets/inafive-2.png)

1. Clique em **Next**.

   ![](assets/inasix-2.png)

1. Mapeie cada campo clicando duas vezes no menu suspenso **Marketo Field** e selecionando o campo apropriado. Clique em **Next** quando terminar.

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
>Quando o Marketo anexa uma conta nomeada, estamos atualizando uma regra (nos bastidores) que nos permite identificar pessoas que devem fazer parte da conta nomeada. Exemplo: se você atualizar &quot;IBM&quot; para &quot;IBM, EUA&quot;, as pessoas com qualquer nome de empresa serão associadas à Conta Nomeada.

Se o Marketo encontrar registros que vemos como duplicatas, processaremos apenas o primeiro.
