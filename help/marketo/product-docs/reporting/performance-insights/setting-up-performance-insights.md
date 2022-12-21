---
unique-page-id: 12981145
description: Configuração de insights de desempenho - Documentos do Marketo - Documentação do produto
title: Configuração de insights de desempenho
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 3%

---

# Configuração de insights de desempenho {#setting-up-performance-insights}

Siga as etapas abaixo para configurar a MPI.

## Configuração da Oportunidade {#opportunity-setup}

1. Clique em **Administrador**.

   ![](assets/admin.png)

1. Clique em **Análise do ciclo de receita**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Se você não tiver RCA, precisará selecionar **Análise de programa** para a Etapa 2.

1. Em Atribuição, clique em **Editar**.

   ![](assets/three-1.png)

1. Configurações de atribuição são exibidas.

   ![](assets/four-2.png)

   Se a Atribuição for explícita, verifique se a Função de Contato da Oportunidade foi preenchida (por meio do endpoint Função da Oportunidade ou por meio da integração CRM).

   Se a Atribuição estiver implícita, verifique se o campo da empresa no cliente potencial/contato é o mesmo que o Nome da conta da oportunidade.

   >[!NOTE]
   >
   >Verifique se todas as oportunidades têm os campos apropriados preenchidos:
   >
   >* Valor da oportunidade
   >* É fechado
   >* É obtido
   >* Data de criação (talvez não seja definida em seu caso)
   >* Data de fechamento (talvez não seja definida no seu caso)
   >* Tipo de oportunidade


## Configuração de programa {#program-setup}

Atualize os custos do programa por pelo menos 12 meses. Você pode fazer isso manualmente ou usando a API do programa. Neste exemplo, fazemos isso manualmente.

1. Clique em **Atividades de marketing**.

   ![](assets/ma.png)

1. Localize e selecione seu programa.

   ![](assets/select-program.png)

1. Clique no botão **Configuração** guia .

   ![](assets/setup-tab.png)

1. Arrastar **Custo do Período** na tela.

   ![](assets/period-cost.png)

1. Configure o Mês do Programa para pelo menos 12 meses atrás e clique em **Ok**.

   ![](assets/set-period.png)

1. Defina o custo do período e clique em **Salvar**.

   ![](assets/set-cost.png)

Em seguida, analise o comportamento do analytics para indicar se um canal específico deve ser incluído no analytics. Defina o comportamento do Analytics (Normal, Inclusivo, Operacional).

1. Clique em **Administrador**.

   ![](assets/admin.png)

1. Clique em **Tags**.

   ![](assets/tags.png)

1. Clique no botão **+** para expandir a lista Canal.

   ![](assets/channel.png)

1. Clique duas vezes no canal desejado.

   ![](assets/channel-click.png)

1. Clique no botão **Comportamento do Analytics** e selecione o comportamento desejado.

   ![](assets/edit-channel.png)

1. Defina os critérios de sucesso.

   ![](assets/success.png)

1. Clique em **Salvar**.

   ![](assets/save.png)

## Vincular o programa à pessoa {#tie-the-program-to-the-person}

1. Verifique se o Programa de aquisição e a Data de aquisição foram definidos para cada pessoa no banco de dados para que a Atribuição de primeiro contato funcione.
1. Certifique-se de que os seus programas estejam a definir estados de sucesso para o seu pessoal.

>[!NOTE]
>
>As alterações efetuadas não são instantâneas. É necessário um período overnight antes de as alterações entrarem em vigor.
