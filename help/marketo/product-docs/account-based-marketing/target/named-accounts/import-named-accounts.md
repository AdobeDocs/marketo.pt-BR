---
unique-page-id: 12615800
description: Importar contas nomeadas - Documentos do Marketing - Documentação do produto
title: Importar contas nomeadas
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---


# Importar contas nomeadas {#import-named-accounts}

Já tem um CSV cheio de possíveis contas de públicos alvos? Importe-os diretamente para o ABM!

1. Clique na lista suspensa **Novo** e selecione **Importar contas** nomeadas.

   ![](assets/inaone.png)

1. Uma nova janela será aberta. Clique em **Procurar** e selecione o arquivo de contas nomeadas que deseja importar.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Em seu arquivo, forneça o [máximo de informações](http://docs.marketo.com/display/DOCS/Named+Account+Overview#NamedAccountOverview-NamedAccountAttributes) possível. Você só pode adicionar informações firmmográficas; nada que o Marketo calcule (isto é, Pipeline). Para criar contas nomeadas com base em contas CRM, basta exportar o nome da conta e a ID do CRM de seu CRM para um arquivo CSV, usar a opção Nome da conta e mapear a ID do CRM durante o processo de importação. Para vincular adequadamente uma conta CRM a uma conta nomeada, é necessário fornecer o nome exato da conta CRM.

1. Escolha entre dois modos de desduplicação: Nome da conta ou Nome do domínio. Neste exemplo, escolheremos Conta. Clique no menu suspenso **Modos** e selecione **Por nome** de conta.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Se você escolher **Por modo** de domínio, a conta nomeada e os campos de domínio devem ser incluídos.

1. Para escolher a lista de conta à qual sua conta nomeada será adicionada, clique no menu suspenso Lista **** Conta e faça sua seleção.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Você também pode criar uma nova Lista Conta digitando seu nome na caixa suspensa.

1. Para enviar uma notificação da importação, clique no menu suspenso **Enviar alerta para** e selecione um usuário do Marketo. Não é *possível* inserir manualmente um endereço de email.

   ![](assets/inafive-2.png)

1. Clique em **Avançar**.

   ![](assets/inasix-2.png)

1. Mapeie cada campo clicando com o duplo no menu suspenso Campo **de** marketing e selecionando o campo apropriado. Clique em **Avançar** quando terminar.

   ![](assets/inaseven.png)

   Sucesso!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Verificar status de importação&quot; mostra apenas os últimos três dias de atividade.

<table> 
 <tbody> 
  <tr> 
   <td>Importando registro com nome de conta nomeado existente</td> 
   <td><p>Atualizaremos o registro existente</p></td> 
  </tr> 
  <tr> 
   <td>Importando registro com o novo nome de Conta Nomeada</td> 
   <td>Criaremos um novo registro</td> 
  </tr> 
 </tbody> 
</table>

Cenários quando você faz dedupe por Nome de Domínio:

| **Importar registro com um novo nome de conta e novo nome de domínio** | Criaremos uma nova conta nomeada com as informações fornecidas |
|---|---|
| **Importar registro com um nome de conta existente e nome de domínio existente** | Atualizaremos a conta nomeada existente |
| **Importar registro com um novo nome de conta e nome de domínio existente** | Acrescentaremos o novo nome de conta à Conta Nomeada existente que corresponde ao nome do domínio e atualizará outras informações (por exemplo, Setor, Estado etc) |
| **Importando registro com nome de conta nomeado existente e novo nome de domínio** | Acrescentaremos o novo nome de domínio à Conta Nomeada existente que corresponde ao nome da conta e atualizará outras informações (por exemplo, Setor, Estado etc) |

>[!NOTE]
>
>Quando o Marketo anexa uma conta nomeada, estamos atualizando uma regra (nos bastidores) que nos permite identificar pessoas que devem fazer parte da conta nomeada. Exemplo: se você atualizar &quot;IBM&quot; para &quot;IBM, EUA&quot;, as pessoas com qualquer nome de empresa serão associadas à Conta Nomeada.

Se o Marketo encontrar registros que vemos como duplicados, processaremos apenas o primeiro.

Cenários quando você faz dedupe por Nome de Conta: