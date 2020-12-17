---
title: priority-override-for-trigger-campanha
description: Substituição de prioridade para Campanhas de acionador
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Substituição de prioridade para Campanhas de acionador

<br> 

Os administradores podem sobrepor a prioridade determinada do Marketo para disparar campanhas para definir prioridades que se alinham melhor com os objetivos de negócios.

>[!NOTE]
>
>Este recurso está disponível somente para campanhas de disparo e para usuários aos quais foi concedida a permissão &quot;Editar prioridade de Campanha de disparador&quot;.

>[!CAUTION]
>
>É altamente recomendável que você use esse recurso em um conjunto limitado de campanhas essenciais para os negócios (25 é o máximo recomendado). Usar o recurso livremente em um conjunto grande pode afetar negativamente a execução geral da campanha.

## Prioridade de substituição

1. Na campanha do acionador, clique na guia **[!UICONTROL Agendar]** e, em seguida, clique em **[!UICONTROL Sobrepor prioridade]**.

   ![Imagem Um](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. Escolha um novo nível de prioridade no menu suspenso. Clique em **[!UICONTROL Confirmar]**.

   ![Imagem dois](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![Imagem Três](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* Você pode visualização sua prioridade padrão de campanha na [!UICONTROL Fila de Campanhas] em [!UICONTROL Atividades de marketing]. Para aumentar a taxa de execução, recomendamos definir sua prioridade de campanha para um nível superior ao padrão.
>* A prioridade definida pelo usuário se aplica somente a novas pessoas que se qualificam para a campanha; as pessoas que já estão em fila não serão afetadas.


## Redefinir prioridade

1. Para redefinir a prioridade da campanha de volta ao padrão do sistema, vá para a guia **[!UICONTROL Schedule]** na campanha do acionador e clique em **[!UICONTROL Reset Priority]**.

   ![Imagem quatro](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. Clique em **[!UICONTROL Redefinir]** para confirmar.

   ![Imagem cinco](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>As substituições e redefinições de prioridade são capturadas na Trilha de auditoria. Você pode visualização a [Trilha de auditoria](https://docs.marketo.com/x/GZ2t) pela área [!UICONTROL Admin] na experiência Clássica.

## Conceder Acesso de Substituição de Prioridade

>[!CAUTION]
>
>Somente Administradores ou usuários com responsabilidades administrativas devem ter acesso de substituição de prioridade campanha.

1. Na área [!UICONTROL Admin], clique em **[!UICONTROL Usuários e funções]**.

   ![Imagem seis](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. Clique na guia **[!UICONTROL Funções]**, selecione o usuário ao qual deseja conceder acesso e clique em **[!UICONTROL Editar Função]**.

   ![Imagem sete](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. Em [!UICONTROL Acessar Atividades de marketing], marque **[!UICONTROL Editar prioridade de Campanha do acionador]**. Clique em **[!UICONTROL Salvar]**.

   ![Imagem Oito](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Prioridade de Campanha de visualização no Marketing Clássico

Você pode visualização a prioridade da campanha na experiência [!DNL Classic] clicando na guia **[!UICONTROL Agendamento]** em uma campanha de disparo.

![Imagem Nove](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>A prioridade na experiência [!DNL Classic] é somente visualização. A alteração ou redefinição da prioridade da campanha só está disponível através do Marketo Sky.
