---
unique-page-id: 7504736
description: Instale o Marketo para Microsoft Dynamics 2015 no local Etapa 1 de 3 - Documentos do Marketo - Documentação do produto
title: Instale o Marketo para Microsoft Dynamics 2015 no local Etapa 1 de 3
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
source-git-commit: 1e20fdd1d3c6bba265ceabe499e0d7a4babf4ef1
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Etapa 1 de 3: Configurar usuário de sincronização para Marketo (2015 no local) {#step-of-configure-sync-user-for-marketo-on-premises-2015}

Antes de sincronizar o Microsoft Dynamics 2015 no local com o Marketo, é necessário primeiro instalar a solução Marketo no Dynamics.

>[!NOTE]
>
>Depois de sincronizar o Marketo com um CRM, não é possível sincronizar um novo CRM com a instância existente do Marketo.

>[!PREREQUISITES]
>
>Se estiver usando o Microsoft Dynamics no local, você deve ter [Implantação virada para a Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) com [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) configurado. Observação: O documento IFD é baixado automaticamente ao clicar no link.
>
>[Baixe a solução de gerenciamento de clientes potenciais da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) antes de começar.

>[!NOTE]
>
>**Permissões de administrador do Dynamics são necessárias.**
>
>Você precisa de privilégios de administrador do CRM para executar essa sincronização.

1. Faça logon em **Dinâmica.** Clique no botão **Microsoft Dynamics CRM** e selecione **Configurações**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Em **Configurações**, selecione **Soluções**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Clique em **Importar**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Clique em **Procurar** e selecione a solução [baixado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Próximo**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Veja as Informações da solução e clique em **Exibir detalhes do pacote da solução**.

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

1. O Gerenciamento de clientes potenciais da Marketo será exibido no **Todas as soluções** página.

   ![](assets/image2015-3-19-8-40-38.png)

1. Selecione a solução Marketo e clique em **Publicar todas as personalizações**.

   ![](assets/image2015-3-19-8-41-21.png)

   Alto cinco! A instalação foi concluída.

   >[!CAUTION]
   >
   >Desativar qualquer um dos processos de mensagens do SDK do Marketo resultará em uma instalação interrompida!

   >[!MORELIKETHIS]
   >
   >[Instale o Marketo para Microsoft Dynamics 2015 no local Etapa 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md)
