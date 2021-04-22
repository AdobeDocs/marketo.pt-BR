---
unique-page-id: 3571813
description: Etapa 1 de 3 - Instalar a solução Marketo no Dynamics (2013 no local) - Documentos da Marketo - Documentação do produto
title: Etapa 1 de 3 - Instalar a solução Marketo no Dynamics (2013 no local)
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Etapa 1 de 3: Instalar a solução Marketo no Dynamics (2013 no local) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Antes de sincronizar o Microsoft Dynamics no local e o Marketo, é necessário primeiro instalar a solução da Marketo no Dynamics.

>[!NOTE]
>
>Depois de sincronizar o Marketo com um CRM, não é possível executar uma nova sincronização sem substituir a instância.

>[!PREREQUISITES]
>
>Você deve ter [Implantação Virada para a Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) com [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 ou 3.0 (ADFS) configurados. Observação: O documento IFD é baixado automaticamente ao clicar no link.
>
>[Baixe a ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) solução da Marketo antes de começar.

>[!NOTE]
>
>**Permissões de administrador do Dynamics são necessárias.**
>
>Você precisa de privilégios de administrador do CRM para executar essa sincronização.

1. Faça logon em **Dynamics**. Clique no menu suspenso **Microsoft Dynamics CRM** e selecione **Settings**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Em **Configurações**, selecione **Soluções**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Clique em **Importar**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Clique em **Procurar** e selecione a [solução baixada](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Next**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Exiba as Informações da solução e clique em **Exibir detalhes do pacote da solução**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Quando terminar de verificar todos os detalhes, clique em **Fechar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. De volta à página Informações da solução , clique em **Próximo**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Verifique se a opção SDK está marcada. Clique em **Importar**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Aguarde até que a importação seja concluída.

   >[!TIP]
   >
   >Você precisará ativar pop-ups no seu navegador para concluir o processo de instalação.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Baixe um arquivo de log (se desejar) e clique em **Fechar**.

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;Marketo Lead Management concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. O Gerenciamento de clientes potenciais da Marketo será exibido na página **Todas as soluções**.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Selecione a solução Marketo e clique em **Publish all Customizations**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

Não foi tão ruim, certo? Vamos, eu vou continuar te conduzindo pelo resto.

>[!CAUTION]
>
>Desativar qualquer um dos processos de mensagens do SDK do Marketo resultará em uma instalação interrompida!

>[!MORELIKETHIS]
>
>[Etapa 2 de 3: Configurar usuário de sincronização para Marketo (2013 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)
