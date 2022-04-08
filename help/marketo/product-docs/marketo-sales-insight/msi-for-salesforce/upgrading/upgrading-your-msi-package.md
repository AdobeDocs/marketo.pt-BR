---
unique-page-id: 37357050
description: Atualização do seu pacote MSI - Documentos do Marketo - Documentação do produto
title: Atualizar seu pacote MSI
exl-id: 45004990-8452-4824-a9b2-89cd8302fe43
source-git-commit: 5c4bce6ab6801b861f70722b6782df34f96fed10
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Atualizar seu pacote MSI {#upgrading-your-msi-package}

1. Navegar para [esta página no appexchange](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000001SVZmEAO){target=&quot;_blank&quot;}.

1. Faça logon na instância do Salesforce (aquela conectada à instância do Marketo, pode ser sandbox ou produção) no canto superior direito da página, na Etapa um. Você deve ter privilégios de administrador para instalar/atualizar um pacote gerenciado no Salesforce.

1. Clique no botão **Obtenha agora** botão. Você deverá escolher onde deseja instalar. Você terá a opção de atualizar, pois já tem uma versão anterior do MSI. Escolha uma opção com base na conta na qual você fez logon durante a Etapa Um.

   >[!TIP]
   >
   >Recomendamos que você teste isso na instância da sandbox antes de atualizar a instância de produção.

1. Você pode atualizar o pacote escolhendo &quot;Instalar somente para administradores&quot; (e fornecer acesso MSI a perfis específicos posteriormente), &quot;Instalar para todos os usuários&quot; ou &quot;Instalar para perfis específicos&quot;. Neste exemplo, estamos escolhendo Somente administradores. Quando tiver feito sua seleção, clique em **Atualizar**.

   ![](assets/four.png)

>[!NOTE]
>
>Recomenda-se que você atualize o pacote somente para Administradores e, em seguida, [fornecer acesso a usuários específicos](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target=&quot;_blank&quot;} com base no número de cadeiras MSI compradas. Como alternativa, você pode criar um perfil específico do Salesforce para usuários do MSI e instalar ou atualizar o pacote somente para esses usuários.
