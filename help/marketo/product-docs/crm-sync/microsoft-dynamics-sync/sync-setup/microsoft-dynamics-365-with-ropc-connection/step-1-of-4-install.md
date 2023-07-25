---
description: Etapa 1 de 4 - Instalar a solução da Marketo com a conexão de controle de senha de proprietário de recurso - Documentação da Marketo - Documentação do produto
title: Etapa 1 de 4 - Instalar a Solução da Marketo com a Conexão de Controle de Senha do Proprietário do Recurso
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Etapa 1 de 4: instalar a solução Marketo com a conexão de controle de senha de proprietário de recurso {#step-1-of-4-install-the-marketo-solution-ropc}

Antes de sincronizar o Microsoft Dynamics 365 e o Marketo, é necessário instalar a solução Marketo no Dynamics. **As permissões de administrador do Dynamics são necessárias.**

>[!CAUTION]
>
>* Não habilite a sincronização de entidade personalizada antes que a sincronização inicial seja concluída. Você será notificado por email quando a sincronização inicial for concluída.
>* Se a Autenticação Multifator (MFA) estiver habilitada para o Dynamics Sync, desabilite-a para que o Dynamics seja sincronizado corretamente com o Marketo. Para obter mais informações, entre em contato com [Suporte ao Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!NOTE]
>
>Após sincronizar o Marketo com um CRM, não é possível executar uma nova sincronização sem substituir a instância.

>[!PREREQUISITES]
>
>[Baixe a solução de gerenciamento líder da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Efetue logon no **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Clique em ![](assets/image2015-3-16-16-3a1-3a13.png) e selecione **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Clique em ![](assets/image2015-5-13-10-3a5-3a8.png) menu. No menu suspenso, selecione **Configurações** e selecione **Soluções**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Clique em **Importar.**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Clique em **Escolha Arquivo.** Selecione a solução de gerenciamento líder da Marketo que você [baixado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Próxima**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Exiba as Informações da Solução e clique em **Exibir detalhes do pacote de soluções**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Quando terminar de verificar todos os detalhes, clique em **Fechar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Agora, na página Informações da solução, clique em **Próxima**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Verifique se a caixa de seleção da opção SDK está marcada. Clique em **Importar**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Você precisará ativar os pop-ups no seu navegador para concluir o processo de instalação.

1. Agora aguarde a conclusão da importação. Levante-se e faça alguns alongamentos.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Clique em **Fechar.**

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;O Gerenciamento de clientes potenciais da Marketo foi concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. O gerenciamento líder da Marketo agora será exibido na lista de soluções.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Selecionar **Gerenciamento de clientes em potencial da Marketo** e clique em **Publicar Todas As Personalizações.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Toque cinco! A instalação foi concluída.

   >[!MORELIKETHIS]
   >
   >[Etapa 2 de 4: Configurar a Solução da Marketo com a Conexão de Controle de Senha do Proprietário do Recurso](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
