---
description: Encaminhar um segmento do Adobe Experience Platform para uma lista estática do Marketo - Documentos do Marketo - Documentação do produto
title: Encaminhar um segmento do Adobe Experience Platform para uma lista estática do Marketo
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
source-git-commit: 0dd8059a43bfb37cdcb6b36cc73d82538263245e
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Encaminhar um segmento do Adobe Experience Platform para uma lista estática do Marketo {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

Esse recurso permite que você envie segmentos localizados no Adobe Experience Platform para o Marketo no formato de uma lista estática.

>[!PREREQUISITES]
>
>* [Editar a função da API](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role) para garantir que tenha o **Pessoa de Leitura-Escrita** permissão (encontrada no menu suspenso API de acesso ).
>* [Criar um usuário de API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) no Marketo.
>* Ir para **Administrador** > **Launchpoint**. Encontre o nome da função que acabou de criar e clique em **Exibir detalhes**. Copie e salve as informações em **ID do cliente** e **Segredo do cliente**, pois pode ser necessário para a Etapa 7.
>* No Marketo, crie uma lista estática ou localize e selecione uma que já tenha criado. Você precisará da ID dele.


1. Faça logon em [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. Clique no ícone de grade e selecione **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. Na navegação à esquerda, clique em **Destinos**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. Clique em **Catálogo**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. Encontre o Marketo Engage e clique em **Ativar**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. Clique em **Configurar novo destino**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. Em Tipo de conta, selecione o botão de opção Conta existente ou nova (neste exemplo, estamos escolhendo **Conta existente**). Clique no ícone Selecionar conta .

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >Se você estiver escolhendo Nova conta, poderá encontrar sua ID do Munchkin acessando **Administrador** > **Munchkin** (também faz parte do URL do Marketo depois de conectado). ID do cliente/Segredo é necessário seguir os pré-requisitos na parte superior deste artigo.

1. Escolha a conta de destino e clique em **Selecionar**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. Inserir um destino **Nome** e uma Descrição opcional. Clique no menu suspenso Criação de pessoa e escolha &quot;Corresponder pessoas existentes do Marketo e Criar pessoas ausentes no Marketo&quot; _ou_ &quot;Corresponder Apenas Às Pessoas Existentes Do Marketo.&quot; Neste exemplo, estamos escolhendo o primeiro.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >Se você escolher &quot;Corresponder somente pessoas existentes do Marketo&quot;, será necessário mapear o Email e/ou a ECID para que seja possível ignorar as Etapas 13 a 16.

1. Esta seção é opcional. Clique em **Criar** para ignorar.

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. Selecione o destino criado e clique em **Próximo**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Escolha o segmento que deseja enviar para o Marketo e clique em **Próximo**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >Se você escolher vários segmentos, será necessário mapear cada segmento para uma lista estática especificada na guia Agendamento de segmento.

   >[!IMPORTANT]
   >
   >Depois que um segmento é ativado para o destino do Marketo pela primeira vez, os perfis de preenchimento retroativo que já existiam no segmento antes da ativação do destino do Marketo podem receber **até 24 horas**. A partir de agora, sempre que perfis forem adicionados ao segmento, eles serão adicionados ao Marketo imediatamente.

1. Clique em **Adicionar novo mapeamento**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. Clique no ícone de mapeamento.

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. Mapear o nome pela seleção **firstName** e clicando em **Selecionar**.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

1. Mapeie o sobrenome e o nome da empresa clicando em **Adicionar novo mapeamento** novamente e repetindo a Etapa 15 duas vezes, escolhendo **lastName** e depois **companyName**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. Agora é hora de mapear o endereço de email. Clique em **Adicionar novo mapeamento** novamente.

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. Clique no ícone de mapeamento.

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. Clique no botão de opção Selecionar namespace de identidade e escolha  **Email**, depois clique em **Selecionar**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >Mapeamento de email e/ou ECID do **Namespace de identidade** A guia é a coisa mais importante a se fazer para garantir que a pessoa seja comparada no Marketo. Mapear email garantirá a maior taxa de correspondência.

1. Agora é hora de escolher os campos de origem. Para email, clique no ícone do cursor.

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. Clique no botão de opção Selecionar namespace de identidade , localize e selecione **Email**, depois clique em **Selecionar**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. Para escolher o campo de origem Nome da empresa , clique no ícone do cursor na linha.

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. Deixe o botão de opção Selecionar atributos marcado. Procure por &quot;empresa&quot; e selecione **companyName**, depois clique em **Selecionar**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. Mapeie os campos de origem para Sobrenome e Nome clicando no ícone de cursor para cada um e repetindo a Etapa 23 duas vezes, escolhendo **lastName** e depois **firstName**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. Clique em **Próximo**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. Agora, será necessário a ID da lista. Clique na guia no navegador que tem a lista estática do Marketo aberta (ou abra uma nova guia e selecione a lista estática desejada).

   ![](assets/push-an-adobe-experience-platform-segment-26.png)

   >[!NOTE]
   >
   >Para obter melhores resultados, use uma lista Marketo Engage vazia.

1. Realce e copie a ID da lista no final do URL.

   ![](assets/push-an-adobe-experience-platform-segment-27.png)

1. Cole a ID que acabou de copiar em ID de mapeamento e clique em **Próximo**.

   ![](assets/push-an-adobe-experience-platform-segment-28.png)

1. Clique em **Concluir**.

   ![](assets/push-an-adobe-experience-platform-segment-29.png)
