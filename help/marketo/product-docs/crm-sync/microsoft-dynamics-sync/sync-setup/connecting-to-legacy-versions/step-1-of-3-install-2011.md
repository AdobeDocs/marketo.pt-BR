---
unique-page-id: 3571805
description: Etapa 1 de 3 - Instalar a solução da Marketo (2011 no local) - Documentação da Marketo - Documentação do produto
title: Etapa 1 de 3 - Instalar a solução da Marketo (2011 no local)
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Etapa 1 de 3: instalar a solução da Marketo (2011 no local) {#step-of-install-the-marketo-solution-on-premises}

Antes de sincronizar o Microsoft Dynamics no local e o Marketo, é necessário instalar a solução Marketo no Dynamics.

>[!NOTE]
>
>Após sincronizar o Marketo com um CRM, não é possível executar uma nova sincronização sem substituir a instância.

>[!PREREQUISITES]
>
>Você deve ter [Implantação voltada para a Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) com [Serviços de Federação do Ative Diretory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 ou 3.0 (ADFS) configurado. **Nota**: o documento IFD é baixado automaticamente quando você clica no link.
>
>[Baixe a solução de gerenciamento líder da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) antes de começar.

>[!NOTE]
>
>**Permissões de administrador do Dynamics necessárias.**
>
>Você precisa de privilégios de administrador do CRM para executar esta sincronização.

1. Efetue logon no **Dynamics**, selecione **Configurações** no menu inferior esquerdo.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Selecionar **Soluções** na árvore.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Clique em **Importar**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Clique em **Procurar**. Selecione a solução de gerenciamento líder da Marketo que você [baixado](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clique em **Próxima**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Exiba as Informações da Solução e clique em **Exibir detalhes do pacote de soluções**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Quando terminar de verificar todos os detalhes, clique em **Fechar**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Na página Informações da solução, clique em **Próxima**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Verifique se a caixa de seleção da opção de mensagem do SDK está marcada. Clique em **Próxima**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Você precisará ativar os pop-ups no seu navegador para concluir o processo de instalação.

1. Agora aguarde a conclusão da importação. Levante-se e faça alguns alongamentos.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Clique em **Fechar**.

   >[!NOTE]
   >
   >Você pode ver uma mensagem dizendo &quot;O Gerenciamento de clientes potenciais da Marketo foi concluído com aviso&quot;. Isso é totalmente esperado.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. O Gerenciamento de clientes potenciais da Marketo agora aparecerá no **Todas as soluções** página.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Selecione Marketo Lead Management e clique em **Publicar Todas As Personalizações.**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

Não foi muito ruim, certo? Vamos, vou continuar te guiando pelo resto.

>[!CAUTION]
>
>Desativar qualquer um dos processos de mensagens do SDK do Marketo resultará em uma instalação corrompida!

>[!MORELIKETHIS]
>
>[Etapa 2 de 3: Configurar o usuário do Marketo Sync no Dynamics (2011 no local)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)
