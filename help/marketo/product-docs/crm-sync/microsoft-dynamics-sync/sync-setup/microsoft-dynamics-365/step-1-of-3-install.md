---
unique-page-id: 3571822
description: Etapa 1 de 3 - Instalar a solução Marketo (Online) - Documentos Marketo - Documentação do produto
title: Etapa 1 de 3 - Instalar a solução Marketo (Online)
exl-id: 593fc014-db38-42cc-8f9f-0dd8307751e8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Etapa 1 de 3: Instalar a solução Marketo (Online) {#step-of-install-the-marketo-solution-online}

Antes de sincronizar o Microsoft Dynamics 365 e o Marketo, é necessário primeiro instalar a solução da Marketo no Dynamics. **As Permissões de administrador do Dynamics são necessárias.**

>[!CAUTION]
>
>* Não ative a sincronização de entidade personalizada antes de concluir a sincronização inicial. Você será notificado por email quando a sincronização inicial for concluída.
>* Se a Autenticação de vários fatores (MFA) estiver ativada para a Sincronização dinâmica, é necessário desativá-la para que o Dynamics sincronize corretamente com a Marketo. Para obter mais informações, entre em contato com o [Suporte da Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).


>[!NOTE]
>
>Depois de sincronizar o Marketo com um CRM, não é possível executar uma nova sincronização sem substituir a instância.

>[!PREREQUISITES]
>
>[Baixe a solução de gerenciamento de clientes potenciais da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Faça logon em **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Clique no menu ![](assets/image2015-3-16-16-3a1-3a13.png) e selecione **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Clique no menu ![](assets/image2015-5-13-10-3a5-3a8.png). No menu suspenso, selecione **Settings** e selecione **Solutions**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Clique em **Importar.**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Clique em **Escolher arquivo.** Selecione a solução de Gerenciamento de clientes potenciais da Marketo que você  [baixou](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Next**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Exiba as Informações da solução e clique em **Exibir detalhes do pacote da solução**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Quando terminar de verificar todos os detalhes, clique em **Fechar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Agora, de volta à página Informações da solução , clique em **Próximo**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Certifique-se de que a caixa de seleção da opção SDK esteja marcada. Clique em **Importar**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Você precisará ativar pop-ups no seu navegador para concluir o processo de instalação.

1. Agora aguarde a conclusão da importação. Levante-se e faça alguns trechos.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Clique em **Fechar.**

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;Marketo Lead Management concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. O Gerenciamento de clientes potenciais da Marketo será exibido na lista de soluções.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Selecione **Marketo Lead Management** e clique em **Publicar todas as personalizações.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Alto cinco! A instalação foi concluída.

   >[!MORELIKETHIS]
   >
   >[Etapa 2 de 3: Configurar o usuário do Marketo Sync no Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)
