---
unique-page-id: 12981145
description: Configurando insights de desempenho - Documentos do marketing - Documentação do produto
title: Configurando insights de desempenho
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Configurando Insights de Desempenho {#setting-up-performance-insights}

Siga as etapas abaixo para configurar a MPI.

## Configuração da Oportunidade {#opportunity-setup}

1. Clique em **Admin**.

   ![](assets/admin.png)

1. Clique em **Análises do ciclo de receita**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Se você não tiver RCA, será necessário selecionar **Análise do Programa** para a Etapa 2.

1. Em Atribuição, clique em **Editar**.

   ![](assets/three-1.png)

1. Configurações de atribuição são exibidas.

   ![](assets/four-2.png)

   Se a Atribuição for explícita, verifique se a Função de Contato da Oportunidade foi preenchida (por meio do endpoint de Função da Oportunidade ou por meio da integração do CRM).

   Se a Atribuição estiver implícita, verifique se o campo empresa no cliente potencial/contato é igual ao Nome da conta da oportunidade.

   >[!NOTE]
   >
   >Verifique se todas as oportunidades têm os campos apropriados preenchidos:
   >
   >    
   >    
   >    * Valor da Oportunidade
   >    * Está fechado
   >    * É vencido
   >    * Data de criação (isso pode não ser definido no seu caso)
   >    * Data de Fechamento (isso pode não ser definido no seu caso)
   >    * Tipo de oportunidade


## Configuração do programa {#program-setup}

Atualize os custos do programa por pelo menos 12 meses. É possível fazer isso manualmente ou usando a API do programa. Neste exemplo fazemos manualmente.

1. Clique em **Atividades de marketing**.

   ![](assets/ma.png)

1. Localize e selecione seu programa.

   ![](assets/select-program.png)

1. Clique na guia **Configuração**.

   ![](assets/setup-tab.png)

1. Arraste **Custo do Período** para a tela.

   ![](assets/period-cost.png)

1. Defina o Mês do Programa há pelo menos 12 meses e clique em **Ok**.

   ![](assets/set-period.png)

1. Defina o custo do período e clique em **Salvar**.

   ![](assets/set-cost.png)

Em seguida, analise o comportamento do Analytics para indicar se um canal específico deve ser incluído no Analytics. Defina o comportamento do Analytics (Normal, Inclusivo, Operacional).

1. Clique em **Admin**.

   ![](assets/admin.png)

1. Clique em **Tags**.

   ![](assets/tags.png)

1. Clique em **+** para expandir a lista do Canal.

   ![](assets/channel.png)

1. Clique com o duplo no canal desejado.

   ![](assets/channel-click.png)

1. Clique na lista suspensa **Comportamento do Analytics** e selecione o comportamento desejado.

   ![](assets/edit-channel.png)

1. Defina os critérios de sucesso.

   ![](assets/success.png)

1. Clique em **Salvar**.

   ![](assets/save.png)

## Vincule o Programa à Pessoa {#tie-the-program-to-the-person}

1. Verifique se o Programa de aquisição e a Data de aquisição foram definidos para cada pessoa no banco de dados para que a Atribuição de primeiro contato funcione.
1. Certifique-se de que seus programas estejam configurando estados de sucesso para suas pessoas.

>[!NOTE]
>
>As alterações efetuadas não são instantâneas. É necessário um período overnight antes de as alterações entrarem em vigor.

