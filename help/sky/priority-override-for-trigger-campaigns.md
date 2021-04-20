---
title: priority-override-for-trigger-campanhas
description: Substituição de prioridade para campanhas do acionador
exl-id: 4468868c-33d7-4b5e-b524-bfcc2785c8ce
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---

# Substituição de prioridade para campanhas do acionador

<br> 

Os administradores podem substituir a prioridade determinada do Marketo para acionar campanhas a fim de definir prioridades que estejam mais alinhadas aos objetivos de negócios.

>[!NOTE]
>
>Esse recurso está disponível somente para campanhas do acionador e para usuários que receberam a permissão &quot;Editar prioridade de campanha do acionador&quot;.

>[!CAUTION]
>
>É altamente recomendável usar esse recurso em um conjunto limitado de campanhas críticas para os negócios (25 é o máximo recomendado). O uso do recurso vagamente em um conjunto grande pode afetar negativamente a execução geral da campanha.

## Prioridade de Substituição

1. Na campanha do acionador, clique na guia **[!UICONTROL Schedule]** e, em seguida, clique em **[!UICONTROL Override Priority]**.

   ![Imagem Um](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. Escolha um novo nível de prioridade no menu suspenso . Clique em **[!UICONTROL Confirmar]**.

   ![Imagem dois](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![Imagem Três](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* Você pode visualizar a prioridade padrão da campanha no [!UICONTROL Fila da campanha] em [!UICONTROL Atividades de marketing]. Para aumentar a taxa de execução, recomendamos configurar a prioridade da campanha para um nível superior ao padrão.
>* A prioridade do conjunto de usuários se aplica somente a novas pessoas que se qualificam para a campanha; as pessoas que já estão na fila não serão afetadas.


## Redefinir prioridade

1. Para redefinir a prioridade da campanha de volta ao padrão do sistema, vá para a guia **[!UICONTROL Schedule]** na campanha do acionador e clique em **[!UICONTROL Reset Priority]**.

   ![Imagem quatro](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. Clique em **[!UICONTROL Redefinir]** para confirmar.

   ![Imagem cinco](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>As substituições e redefinições de prioridade são capturadas na Trilha de auditoria. Você pode visualizar a [Trilha de Auditoria](https://docs.marketo.com/x/GZ2t) através da área [!UICONTROL Admin] na experiência Clássica.

## Conceder Acesso de Substituição de Prioridade

>[!CAUTION]
>
>Somente administradores ou usuários com responsabilidades de administrador devem ter acesso de substituição de prioridade de campanha.

1. Na área [!UICONTROL Admin], clique em **[!UICONTROL Usuários e funções]**.

   ![Imagem 6](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. Clique na guia **[!UICONTROL Funções]**, selecione o usuário ao qual deseja conceder acesso e clique em **[!UICONTROL Editar Função]**.

   ![Imagem sete](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. Em [!UICONTROL Acessar atividades de marketing], marque **[!UICONTROL Editar prioridade de campanha do acionador]**. Clique em **[!UICONTROL Salvar]**.

   ![Imagem Oito](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## Exibir a prioridade da campanha no Marketo Classic

Você pode visualizar a prioridade da campanha na experiência [!DNL Classic] clicando na guia **[!UICONTROL Schedule]** em uma campanha de acionamento.

![Imagem nove](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>A prioridade na experiência [!DNL Classic] é somente visualização. Alterar ou redefinir a prioridade da campanha só está disponível através do Marketo Sky.
