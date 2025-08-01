---
unique-page-id: 12615800
description: Importar [!UICONTROL Contas Nomeadas] - Documentação Do Marketo - Documentação Do Produto
title: Importar [!UICONTROL Contas Nomeadas]
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# Importar [!UICONTROL Contas Nomeadas] {#import-named-accounts}

Já tem um CSV cheio de contas de destino em potencial? Importe-os diretamente para o TAM!

1. Clique no menu suspenso **[!UICONTROL Novo]** e selecione **[!UICONTROL Importar contas nomeadas]**.

   ![](assets/inaone.png)

1. Uma nova janela será aberta. Clique em **[!UICONTROL Procurar]** e selecione o arquivo de contas nomeadas que deseja importar.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Em seu arquivo, forneça [o máximo de informações](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) possível. Você só pode adicionar informações firmográficas; nada que o Marketo calcule (ou seja, Pipeline). Para criar contas nomeadas com base em contas do CRM, basta exportar o nome da conta e a ID do CRM do seu CRM para um arquivo CSV, usar a opção Nome da conta e mapear a ID do CRM durante o processo de importação. Para vincular corretamente uma conta do CRM a uma conta nomeada, você deve fornecer o nome exato da conta do CRM.

1. Escolha entre dois modos de desduplicação: Nome da conta ou Nome do domínio. Neste exemplo, vamos escolher Conta. Clique no menu suspenso **[!UICONTROL Modos]** e selecione **[!UICONTROL Por nome de conta]**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Se você escolher **[!UICONTROL Por Nome de Domínio]**, os campos de conta nomeada e de domínio deverão ser incluídos.

1. Para escolher a qual lista de contas sua conta nomeada será adicionada, clique no menu suspenso **[!UICONTROL Lista de Contas]** e faça sua seleção.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Você também pode criar uma nova [!UICONTROL Lista de contas] simplesmente digitando seu nome na caixa suspensa.

1. Para enviar uma notificação sobre a importação, clique no menu suspenso **[!UICONTROL Enviar Alerta para]** e selecione um usuário do Marketo. Você _não pode_ inserir um endereço de email manualmente.

   ![](assets/inafive-2.png)

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/inasix-2.png)

1. Mapeie cada campo clicando duas vezes no menu suspenso **[!UICONTROL Campo do Marketo]** e selecionando o campo apropriado. Clique em **[!UICONTROL Avançar]** quando terminar.

   ![](assets/inaseven.png)

   Sucesso!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Verificar status da importação&quot; mostra apenas os últimos três dias de atividade.

Cenários em que você elimina a duplicação de [!UICONTROL por Nome de Conta]:

<table>
 <tbody>
  <tr>
   <td><strong>Importando registro com o nome da <span class="uicontrol">Conta Nomeada</span> existente</strong></td>
   <td><p>Atualizaremos o registro existente</p></td>
  </tr>
  <tr>
   <td><strong>Importando registro com o novo nome de <span class="uicontrol">Conta Nomeada</span></strong></td>
   <td>Criaremos um novo registro</td>
  </tr>
 </tbody>
</table>

Cenários em que você elimina a duplicação de [!UICONTROL por Nome de Domínio]:

<table>
 <tbody>
  <tr>
   <td><strong>Importando registro com um novo nome de conta e um novo nome de domínio</strong></td>
   <td>Criaremos uma nova <span class="uicontrol">Conta nomeada</span> com as informações fornecidas</td>
  </tr>
  <tr>
   <td><strong>Importação de registro com um nome de conta existente e um nome de domínio existente</strong></td>
   <td>Atualizaremos a <span class="uicontrol">Conta nomeada</span> existente</td>
  </tr>
   <tr>
   <td><strong>Importação de registro com um novo nome de conta e nome de domínio existente</strong></td>
   <td>Vamos anexar o novo nome de conta à <span class="uicontrol">Conta Nomeada</span> existente que corresponde ao nome de domínio e atualizar outras informações (por exemplo, Setor, Estado etc)</td>
  </tr>
  <tr>
   <td><strong>Importando registro com nome e novo nome de domínio da <span class="uicontrol">Conta Nomeada</span> existente</strong></td>
   <td>Vamos anexar o novo nome de domínio à <span class="uicontrol">Conta Nomeada</span> existente que corresponde ao nome da conta e atualizar outras informações (por exemplo, Setor, Estado etc)</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>Quando o Marketo anexa uma conta nomeada, estamos atualizando uma regra (em segundo plano) que nos permite identificar as pessoas que devem fazer parte da [!UICONTROL Conta Nomeada]. Exemplo: se você atualizar &quot;IBM&quot; para &quot;IBM, EUA&quot;, as pessoas com qualquer nome de empresa serão associadas à [!UICONTROL Conta nomeada].

Se o Marketo encontrar registros que vemos como duplicatas, processaremos apenas o primeiro.
