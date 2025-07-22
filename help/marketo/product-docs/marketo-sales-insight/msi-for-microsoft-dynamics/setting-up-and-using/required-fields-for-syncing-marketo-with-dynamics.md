---
unique-page-id: 11375827
description: Campos obrigatórios para sincronização do Marketo com o Dynamics - Documentação do Marketo - Documentação do produto
title: Campos obrigatórios para sincronização do Marketo com o Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 3%

---

# Campos Obrigatórios para Sincronização do Marketo com [!DNL Dynamics] {#required-fields-for-syncing-marketo-with-dynamics}

Estes campos *devem* ser sincronizados com a Marketo para que o [!UICONTROL Lead] e o [!UICONTROL Contato] para [!DNL Sales Insight] funcionem:

* Prioridade
* Urgência
* Pontuação relativa

Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, verifique sua instância para ter certeza de que os campos estão sincronizados para **[!UICONTROL Lead]** e **[!UICONTROL Contato]**. Caso contrário, adicione-os.

Veja como verificar e adicionar campos de sincronização.

1. Vá para [!UICONTROL Admin] e clique em **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **[!UICONTROL Editar]** em [!UICONTROL Detalhes da sincronização de campo].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Em [!UICONTROL Lead], marque a caixa de seleção [!UICONTROL Prioridade].

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Agora, role para baixo e marque a caixa de seleção [!UICONTROL Urgência]...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...e a caixa de seleção [!UICONTROL Pontuação relativa].

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Em seguida, marque as caixas de seleção para [!UICONTROL Prioridade], [!UICONTROL Urgência] e [!UICONTROL Pontuação Relativa] para [!UICONTROL Contato].

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Aguarde pelo menos 10 minutos para que uma sincronização seja executada antes de verificar se você corrigiu o problema.

>[!MORELIKETHIS]
>
>[Configurando Estrelas e Chamas para Registros de Cliente Potencial/Contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
