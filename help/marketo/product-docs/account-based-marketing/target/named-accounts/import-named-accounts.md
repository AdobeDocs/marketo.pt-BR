---
unique-page-id: 12615800
description: Importar contas nomeadas - Documentos do Marketing - Documentação do produto
title: Importar contas nomeadas
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---


# Importar contas nomeadas {#import-named-accounts}

Já tem um CSV cheio de possíveis contas de públicos alvos? Importe-os diretamente para o ABM!

1. Clique na lista suspensa **Novo** e selecione **Importar contas nomeadas**.

   ![](assets/inaone.png)

1. Uma nova janela será aberta. Clique em **Procurar** e selecione o arquivo de contas nomeadas que deseja importar.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >No arquivo, forneça [o máximo de informações](/help/marketo/product-docs/account-based-marketing/target/named-accounts/named-account-overview.md#named-account-attributes) possível. Você só pode adicionar informações firmmográficas; nada que o Marketo calcule (isto é, Pipeline). Para criar contas nomeadas com base em contas CRM, basta exportar o nome da conta e a ID do CRM de seu CRM para um arquivo CSV, usar a opção Nome da conta e mapear a ID do CRM durante o processo de importação. Para vincular adequadamente uma conta CRM a uma conta nomeada, é necessário fornecer o nome exato da conta CRM.

1. Escolha entre dois modos de desduplicação: Nome da conta ou Nome do domínio. Neste exemplo, escolheremos Conta. Clique no menu suspenso **Modos** e selecione **Por nome de conta**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Se você escolher **Por modo de domínio**, a conta nomeada e os campos de domínio devem ser incluídos.

1. Para escolher a lista de conta à qual sua conta nomeada será adicionada, clique no menu suspenso **Lista de conta** e faça sua seleção.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Você também pode criar uma nova Lista Conta digitando seu nome na caixa suspensa.

1. Para enviar uma notificação da importação, clique no menu suspenso **Enviar alerta para** e selecione um usuário de marketing para. Você _não pode_ inserir manualmente um endereço de email.

   ![](assets/inafive-2.png)

1. Clique em **Próximo**.

   ![](assets/inasix-2.png)

1. Mapeie cada campo clicando com o duplo no menu suspenso **Campo de marketing** e selecionando o campo apropriado. Clique em **Próximo** quando terminar.

   ![](assets/inaseven.png)

   Sucesso!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Verificar status de importação&quot; mostra apenas os últimos três dias de atividade.

Cenários quando você faz dedupe por Nome de Conta:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importando registro com nome de conta nomeado existente</strong></td> 
   <td><p>Atualizaremos o registro existente</p></td> 
  </tr> 
  <tr> 
   <td><strong>Importando registro com o novo nome de Conta Nomeada</strong></td> 
   <td>Criaremos um novo registro</td> 
  </tr> 
 </tbody> 
</table>

Cenários quando você faz dedupe por Nome de Domínio:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importar registro com um novo nome de conta e novo nome de domínio</strong></td> 
   <td>Criaremos uma nova conta nomeada com as informações fornecidas</td> 
  </tr> 
  <tr> 
   <td><strong>Importar registro com um nome de conta existente e nome de domínio existente</strong></td> 
   <td>Atualizaremos a conta nomeada existente</td> 
  </tr> 
   <tr> 
   <td><strong>Importar registro com um novo nome de conta e nome de domínio existente</strong></td> 
   <td>Acrescentaremos o novo nome de conta à Conta Nomeada existente que corresponde ao nome do domínio e atualizará outras informações (por exemplo, Setor, Estado etc)</td> 
  </tr> 
  <tr> 
   <td><strong>Importando registro com nome de conta nomeado existente e novo nome de domínio</strong></td> 
   <td>Acrescentaremos o novo nome de domínio à Conta Nomeada existente que corresponde ao nome da conta e atualizará outras informações (por exemplo, Setor, Estado etc)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando o Marketo anexa uma conta nomeada, estamos atualizando uma regra (nos bastidores) que nos permite identificar pessoas que devem fazer parte da conta nomeada. Exemplo: se você atualizar &quot;IBM&quot; para &quot;IBM, EUA&quot;, as pessoas com qualquer nome de empresa serão associadas à Conta Nomeada.

Se o Marketo encontrar registros que vemos como duplicados, processaremos apenas o primeiro.
