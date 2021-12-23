---
unique-page-id: 3571805
description: Etapa 1 de 3 - Instalar a solução Marketo (2011 no local) - Documentos da Marketo - Documentação do produto
title: Etapa 1 de 3 - Instalar a solução Marketo (2011 no local)
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Etapa 1 de 3: Instalar a solução Marketo (2011 no local) {#step-of-install-the-marketo-solution-on-premises}

Antes de sincronizar o Microsoft Dynamics no local e o Marketo, é necessário primeiro instalar a solução Marketo no Dynamics.

>[!NOTE]
>
>Depois de sincronizar o Marketo com um CRM, não é possível executar uma nova sincronização sem substituir a instância.

>[!PREREQUISITES]
>
>Você deve ter [Implantação virada para a Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) com [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 ou 3.0 (ADFS) configuradas. **Observação**: O documento IFD é baixado automaticamente ao clicar no link.
>
>[Baixe a solução de gerenciamento de clientes potenciais da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) antes de começar.

>[!NOTE]
>
>**Permissões de administrador do Dynamics são necessárias.**
>
>Você precisa de privilégios de administrador do CRM para executar essa sincronização.

1. Faça logon em **Dynamics**, selecione **Configurações** no menu inferior esquerdo.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Selecionar **Soluções** na árvore.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Clique em **Importar**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Clique em **Procurar**. Selecione a solução de Gerenciamento de clientes potenciais da Marketo que você [baixado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Próximo**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Veja as Informações da solução e clique em **Exibir detalhes do pacote da solução**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Quando terminar de verificar todos os detalhes, clique em **Fechar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. De volta à página Informações da solução , clique em **Próximo**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Verifique se a caixa de seleção da opção SDK message está marcada. Clique em **Próximo**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Você precisará ativar pop-ups no seu navegador para concluir o processo de instalação.

1. Agora aguarde a conclusão da importação. Levante-se e faça alguns trechos.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Clique em **Fechar**.

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;Marketo Lead Management concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. O Gerenciamento de clientes potenciais da Marketo será exibido no **Todas as soluções** página.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Selecione Marketo Lead Management e clique em **Publicar todas as personalizações.**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

Não foi tão ruim, certo? Vamos, eu vou continuar te conduzindo pelo resto.

>[!CAUTION]
>
>Desativar qualquer um dos processos de mensagens do SDK do Marketo resultará em uma instalação interrompida!

>[!MORELIKETHIS]
>
>[Etapa 2 de 3: Configurar o usuário do Marketo Sync no Dynamics (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)
