---
unique-page-id: 7504736
description: Instale o Marketo para Dynamics 2015 no local e 2016 365 no local Etapa 1 de 3 - Documentos da Marketo - Documentação do produto
title: Instale o Marketo para Dynamics 2015 no local e 2016 365 no local Etapa 1 de 3
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Etapa 1 de 3: Configurar o usuário de sincronização para Marketo (2015 no local e 2016 365 no local) {#step-of-configure-sync-user-for-marketo-on-premises-and-365}

Antes de sincronizar o Microsoft Dynamics 2015 no local ou 2016 (Dynamics 365) com o Marketo, é necessário primeiro instalar a solução da Marketo no Dynamics.

>[!NOTE]
>
>Depois de sincronizar o Marketo com um CRM, não é possível sincronizar um novo CRM com a instância existente do Marketo.

>[!PREREQUISITES]
>
>Se você estiver usando o Microsoft Dynamics On-Premise, deverá ter [Implantação Facing da Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) com [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) configurados. Observação: O documento IFD é baixado automaticamente ao clicar no link.
>
>[Baixe a ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) solução de gerenciamento de clientes potenciais da Marketo antes de iniciar.

>[!NOTE]
>
>**Permissões de administrador do Dynamics são necessárias.**
>
>Você precisa de privilégios de administrador do CRM para executar essa sincronização.

1. Faça logon em **Dynamics.** Clique no menu suspenso  **Microsoft Dynamics** CRM e selecione  **Configurações**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Em **Configurações**, selecione **Soluções**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Clique em **Importar**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Clique em **Procurar** e selecione a solução [baixada](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Next**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Exiba as Informações da solução e clique em **Exibir detalhes do pacote da solução**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Quando terminar de verificar todos os detalhes, clique em **Fechar**.

   ![](assets/step6.png)

1. De volta à página Informações da solução , clique em **Próximo**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Certifique-se de que a caixa de seleção da opção SDK esteja marcada. Clique em **Importar**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Aguarde até que a importação seja concluída.

   >[!TIP]
   >
   >Você precisará ativar pop-ups no seu navegador para concluir o processo de instalação.

   ![](assets/image2015-3-11-11-34-9.png)

1. Baixe um arquivo de log (se desejar) e clique em **Fechar**.

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;Marketo Lead Management concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2015-3-13-9-54-39.png)

1. O Gerenciamento de clientes potenciais da Marketo será exibido na página **Todas as soluções**.

   ![](assets/image2015-3-19-8-40-38.png)

1. Selecione a solução Marketo e clique em **Publicar todas as personalizações**.

   ![](assets/image2015-3-19-8-41-21.png)

   Alto cinco! A instalação foi concluída.

   >[!CAUTION]
   >
   >Desativar qualquer um dos processos de mensagens do SDK do Marketo resultará em uma instalação interrompida!

   >[!MORELIKETHIS]
   >
   >[Instale o Marketo para Dynamics 2015 no local e 2016 365 no local Etapa 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
