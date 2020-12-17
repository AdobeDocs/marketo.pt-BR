---
unique-page-id: 3571813
description: Etapa 1 de 3 - Instalar a solução Marketo no Dynamics (2013 no local) - Documentação do produto - Documentação do produto
title: Etapa 1 de 3 - Instalar a solução Marketo no Dynamics (2013 no local)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Etapa 1 de 3: Instale a solução Marketo no Dynamics (2013 On-Premise) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Antes de poder sincronizar o Microsoft Dynamics On-Premise e o Marketing, é necessário instalar primeiro a solução Marketo no Dynamics.

>[!NOTE]
>
>Depois de sincronizar o Marketo com um CRM, não é possível executar uma nova sincronização sem substituir a instância.

>[!PREREQUISITES]
>
>Você deve ter [Implantação para Internet](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) com [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 ou 3.0 (ADFS) configurados. Observação: O documento IFD é baixado automaticamente quando você clica no link.
>
>[Baixe a ](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) solução Marketo antes do start.

>[!NOTE]
>
>**Permissões do administrador dinâmico necessárias.**
>
>Você precisa de privilégios de administrador do CRM para executar essa sincronização.

1. Faça logon em **Dinâmicas**. Clique no menu suspenso **Microsoft Dynamics CRM** e selecione **CONFIGURAÇÕES**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Em **CONFIGURAÇÕES**, selecione **SOLUÇÕES**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Clique em **Importar**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Clique em **Procurar** e selecione a [solução baixada](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Próximo**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Visualização as Informações da solução e clique em **Detalhes do pacote da solução de Visualização**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Quando terminar de verificar todos os detalhes, clique em **Fechar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Na página Informações da solução, clique em **Próximo**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Verifique se a opção SDK está marcada. Clique em **Importar**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Aguarde a importação terminar.

   >[!TIP]
   >
   >Será necessário ativar pop-ups no seu navegador para concluir o processo de instalação.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Baixe um arquivo de log (se desejar) e clique em **Fechar**.

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;Gerenciamento de cliente potencial concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. O Gerenciamento líder de marketing agora será exibido na página **Todas as soluções**.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Selecione a solução Marketo e clique em **Publicar todas as personalizações**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

Não era tão ruim, certo? Vamos, eu continuarei te guiando pelo resto.

>[!CAUTION]
>
>A desativação de qualquer um dos processos de mensagens do SDK do Marketo resultará em uma instalação interrompida!

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Etapa 2 de 3: Configurar usuário de sincronização para o Marketing (2013 On-Premise)](step-2-of-3-configure.md)

>



