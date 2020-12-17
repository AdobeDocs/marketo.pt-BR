---
unique-page-id: 3571822
description: Etapa 1 de 3 - Instalar a solução Marketo (Online) - Documentação do produto - Documentação do produto
title: Etapa 1 de 3 - Instalar a solução Marketing (Online)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Etapa 1 de 3: Instale a solução Marketo (Online) {#step-of-install-the-marketo-solution-online}

Antes de sincronizar o Microsoft Dynamics 365 e o Marketo, é necessário instalar primeiro a solução Marketing no Dynamics. **As Permissões de administrador dinâmico são obrigatórias.**

>[!CAUTION]
>
>* `Do not enable custom entity sync before the initial sync is completed. You will be notified via email once the initial sync is completed.`
>* Se a Autenticação Multifator (MFA) estiver ativada para sua Sincronização Dinâmica, você deverá desativá-la para que a Dinâmica seja sincronizada corretamente com o Marketo. Para obter informações adicionais, entre em contato com o [Suporte do Marketing](http://nation.marketo.com/community/support_solutions).

>



>[!NOTE]
>
>Depois de sincronizar o Marketo com um CRM, não é possível executar uma nova sincronização sem substituir a instância.

>[!PREREQUISITES]
>
>[Download da solução de gerenciamento líder de marketing](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Efetue login em ** [Microsoft Office 365](https://login.microsoftonline.com/) **.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Clique no menu ![](assets/image2015-3-16-16-3a1-3a13.png)e selecione **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Clique no menu ![](assets/image2015-5-13-10-3a5-3a8.png). No menu suspenso, selecione **Configurações **e, em seguida, selecione **Soluções**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Clique em **Importar.**

   ** ![](assets/image2015-3-19-8-3a34-3a8.png)

   **

1. Clique em **Escolher arquivo.** Selecione a solução de Gerenciamento líder de mercado que você  [baixou](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Próximo**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Visualização as Informações da solução e clique em **Detalhes do pacote da solução de Visualização**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Quando terminar de verificar todos os detalhes, clique em **Fechar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Agora, na página Informações da solução, clique em **Próximo**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Verifique se a caixa de seleção da opção SDK está selecionada. Clique em **Importar**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Será necessário ativar pop-ups no seu navegador para concluir o processo de instalação.

1. Agora espere a importação terminar. Levante-se e faça alguns trechos.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Clique em **Fechar.**

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;Gerenciamento de cliente potencial concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. O Gerenciamento líder de marketing agora será exibido na lista de soluções.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Selecione **Gerenciamento líder de marketing** e clique em **Publicar todas as personalizações.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Alto cinco! A instalação foi concluída.

   >[!MORELIKETHIS]
   >
   >[Etapa 2 de 3: Configurar usuário de sincronização de marketing no Dynamics](step-2-of-3-set-up.md)
