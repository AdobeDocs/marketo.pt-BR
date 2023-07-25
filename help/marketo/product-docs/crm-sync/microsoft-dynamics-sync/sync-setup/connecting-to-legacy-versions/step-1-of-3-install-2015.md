---
unique-page-id: 7504736
description: Instalar o Marketo para Microsoft Dynamics 2015 no local Etapa 1 de 3 - Documentação do Marketo - Documentação do produto
title: Instalar o Marketo para Microsoft Dynamics 2015 no Local Etapa 1 de 3
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Etapa 1 de 3: Configurar usuário de sincronização para o Marketo (2015 no local) {#step-of-configure-sync-user-for-marketo-on-premises-2015}

Antes de sincronizar o Microsoft Dynamics 2015 no local com o Marketo, é necessário instalar a solução Marketo no Dynamics.

>[!NOTE]
>
>Depois de sincronizar o Marketo com um CRM, você não pode sincronizar um novo CRM com a instância existente do Marketo.

>[!PREREQUISITES]
>
>Se estiver usando o Microsoft Dynamics no local, você deve ter [Implantação voltada para a Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) com [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) configurado. Observação: o documento IFD é baixado automaticamente quando você clica no link.
>
>[Baixe a solução de gerenciamento líder da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) antes de começar.

>[!NOTE]
>
>**Permissões de administrador do Dynamics necessárias.**
>
>Você precisa de privilégios de administrador do CRM para executar esta sincronização.

1. Efetue logon no **Dinâmica.** Clique em **Microsoft Dynamics CRM** e selecione **Configurações**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Em **Configurações**, selecione **Soluções**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Clique em **Importar**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Clique em **Procurar** e selecione a solução que você [baixado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Próxima**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Exiba as Informações da Solução e clique em **Exibir detalhes do pacote de soluções**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Quando terminar de verificar todos os detalhes, clique em **Fechar**.

   ![](assets/step6.png)

1. Na página Informações da solução, clique em **Próxima**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Verifique se a caixa de seleção da opção SDK está marcada. Clique em **Importar**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Aguarde a conclusão da importação.

   >[!TIP]
   >
   >Você precisará ativar os pop-ups no seu navegador para concluir o processo de instalação.

   ![](assets/image2015-3-11-11-34-9.png)

1. Baixe um arquivo de log (se desejar) e clique em **Fechar**.

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;O Gerenciamento de clientes potenciais da Marketo foi concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2015-3-13-9-54-39.png)

1. O Gerenciamento de clientes potenciais da Marketo agora aparecerá no **Todas as soluções** página.

   ![](assets/image2015-3-19-8-40-38.png)

1. Selecione a solução da Marketo e clique em **Publicar todas as personalizações**.

   ![](assets/image2015-3-19-8-41-21.png)

   Toque cinco! A instalação foi concluída.

   >[!CAUTION]
   >
   >Desativar qualquer um dos processos de mensagens do SDK do Marketo resultará em uma instalação corrompida!

   >[!MORELIKETHIS]
   >
   >[Instalar o Marketo para Microsoft Dynamics 2015 no Local Etapa 2 de 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md)
