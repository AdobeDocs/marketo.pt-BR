---
unique-page-id: 3571805
description: Etapa 1 de 3 - Instalar a solução Marketo (nas instalações 2011) - Documentação do produto - Documentação do produto
title: Etapa 1 de 3 - Instalar a solução Marketo (2011 no local)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# Etapa 1 de 3: Instale a solução Marketo (2011 On-Premise) {#step-of-install-the-marketo-solution-on-premises}

Antes de poder sincronizar o Microsoft Dynamics On-Premise e o Marketing, é necessário instalar primeiro a solução Marketo no Dynamics.

>[!NOTE]
>
>Depois de sincronizar o Marketo com um CRM, não é possível executar uma nova sincronização sem substituir a instância.

>[!PREREQUISITES]
>
>Você deve ter [Implantação para Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) com [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 ou 3.0 (ADFS) configurados. **Observação**: O documento IFD é baixado automaticamente quando você clica no link.
>
>[Baixe a ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) solução de gerenciamento líder de marketing antes do start.

>[!NOTE]
>
>**Permissões do administrador dinâmico necessárias.**
>
>Você precisa de privilégios de administrador do CRM para executar essa sincronização.

1. Faça logon em **Dinâmicas**, selecione **Configurações** no menu inferior esquerdo.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Selecione **Soluções** na árvore.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Clique em **Importar**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Clique em **Procurar**. Selecione a solução de Gerenciamento líder de marketing [baixada](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Próximo**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Visualização as Informações da solução e clique em **Detalhes do pacote da solução de Visualização**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Quando terminar de verificar todos os detalhes, clique em **Fechar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Na página Informações da solução, clique em **Próximo**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Verifique se a caixa de seleção da opção de mensagem do SDK está marcada. Clique em **Próximo**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Será necessário ativar pop-ups no seu navegador para concluir o processo de instalação.

1. Agora espere a importação terminar. Levante-se e faça alguns trechos.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Clique em **Fechar**.

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;Gerenciamento de cliente potencial concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. O Gerenciamento líder de marketing agora será exibido na página **Todas as soluções**.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Selecione Gerenciamento de cliente em potencial e clique em **Publicar todas as personalizações.**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

Não era tão ruim, certo? Vamos, eu continuarei te guiando pelo resto.

>[!CAUTION]
>
>A desativação de qualquer um dos processos de mensagens do SDK do Marketo resultará em uma instalação interrompida!

>[!MORELIKETHIS]
>
>[Etapa 2 de 3: Configurar usuário de sincronização de marketing no Dynamics (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)
