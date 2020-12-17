---
unique-page-id: 4719297
description: Ativar/Desativar sincronização de objetos personalizados - Documentos de marketing - Documentação do produto
title: Ativar/desativar sincronização de objetos personalizados
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Ativar/Desativar Sincronização de Objeto Personalizado {#enable-disable-custom-object-sync}

Os objetos personalizados criados na instância do Salesforce também podem fazer parte do Marketing. Veja como configurar.

## Ativar/Desativar Sincronização de Objeto Personalizado {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>Direitos de administrador necessários.

1. Clique em **Admin**.

   ** ![](assets/one.png)

   **

1. No menu Gerenciamento de banco de dados, clique em **Salesforce** **Sincronização de objetos**.

   ![](assets/two-2.png)

1. Se este for seu primeiro Objeto personalizado, clique em **Sincronizar schema.** Caso contrário, clique em  **Atualizar** Schemato para garantir que você tenha a versão mais recente.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Se a sincronização global estiver em execução, será necessário desativá-la clicando em **Desativar sincronização global.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >Uma sincronização do schema de objeto personalizado do Salesforce pode levar alguns minutos.

1. Clique em **Atualizar Schema**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Selecione o objeto que deseja sincronizar e clique em **Ativar sincronização**.

   >[!TIP]
   >
   >O Marketo só pode sincronizar um objeto personalizado se ele tiver um relacionamento direto com o objeto Cliente potencial, Contato ou Conta no Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Clique novamente em **Ativar Sincronização**.

   ** ![](assets/image2014-12-10-10-3a15-3a40.png)

   **

1. Volte para a guia **Salesforce** e clique em **Ativar sincronização**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Usando seus objetos personalizados {#using-your-custom-objects}

>[!NOTE]
>
>Não é possível usar objetos personalizados em campanhas inteligentes com acionadores.

1. Na sua lista inteligente, arraste sobre o filtro **Tem oportunidade** e defina como **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Em seguida, use as restrições de filtro para restringir o foco.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Excelente! Agora você pode usar os dados desse objeto personalizado em campanhas inteligentes e listas inteligentes.

>[!MORELIKETHIS]
>
>* [Adicionar/remover campo de objeto personalizado como restrições de Lista inteligente/acionador](add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

>



