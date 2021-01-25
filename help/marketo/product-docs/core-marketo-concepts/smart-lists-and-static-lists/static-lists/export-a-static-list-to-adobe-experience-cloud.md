---
unique-page-id: 37356194
description: Exportar uma Lista estática para Adobe Experience Cloud - Documentos do Marketing - Documentação do produto
title: Exportar uma Lista estática para Adobe Experience Cloud
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---


# Exportar uma Lista estática para Adobe Experience Cloud {#export-a-static-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Uma implantação pronta para HIPAA de uma instância de Marketo não pode usar esse recurso.

>[!PREREQUISITES]
>
>[Configurar o compartilhamento de Audiências da Adobe Experience Cloud](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## Aplicativos de destino suportados {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (**somente** se você possuir uma licença da Adobe Audience Manager)
* Adobe Audience Manager
* Adobe Experience Manager
* Plataforma de dados do cliente em tempo real do Adobe
* Adobe Target

## Como exportar uma Lista {#how-to-export-a-list}

1. Em Marketo, localize e selecione a lista que deseja exportar.

   ![](assets/one.png)

1. Clique no menu suspenso **Ações de Lista** e selecione **Enviar para Experience Cloud**.

   ![](assets/two-1.png)

1. Clique na lista suspensa **Pasta de Audience Manager** e selecione a pasta de destino desejada no Experience Cloud.

   ![](assets/three-1.png)

1. Escolha se deseja criar uma nova audiência ou substituir uma existente (neste exemplo, estamos criando uma nova). Digite o novo nome da audiência e clique em **Enviar**.

   ![](assets/four.png)

1. Clique em **OK**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Pode levar de 6 a 8 horas para que a associação à audiência seja totalmente preenchida no Adobe.

## Observação {#things-to-note}

**Compartilhamento no Adobe Analytics**

Para os clientes que possuem Adobe Audience Manager e Adobe Analytics, essa integração permitirá que as audiências sejam compartilhadas do Marketing para seus Conjuntos de relatórios da Adobe Analytics, no entanto, há algumas etapas adicionais de configuração que precisam ser seguidas no Adobe Audience Manager para habilitar essa ação. Consulte a documentação da Adobe Audience Manager para obter mais informações sobre como configurar: [https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html](https://docs.adobe.com/content/help/en/analytics/integration/audience-analytics/mc-audiences-aam.html).

**Uso de características para clientes Adobe Audience Manager**

Ao iniciar uma exportação de lista no Marketo, você observará as seguintes alterações refletidas em sua instância do Adobe Audience Manager:

* Para todos os clientes potenciais na Lista exportada, o Marketo gravará uma característica usando os emails com hash dos clientes potenciais como um identificador entre dispositivos. O nome da característica corresponderá ao Nome da Audiência de Destino especificado durante a exportação.
* Para todos os ECIDs que o Marketo conseguiu corresponder aos clientes potenciais na Lista exportada, o Marketo gravará uma característica usando o identificador de dispositivo ECID. O nome da característica corresponderá ao Nome da Audiência de Destino especificado durante a exportação.
* O Marketo também criará um segmento em sua instância do Audience Manager usando a característica ECID como único critério de segmentação. O nome do segmento corresponderá ao Nome da Audiência de Destino especificado durante a exportação.

## Perguntas frequentes {#faq}

**Por que o tamanho da lista em Marketo é diferente do tamanho em Adobe?**

Sob o capô, a integração da audiência funciona sincronizando os cookies do Marketo Munchkin com o cookie Adobe ECID correspondente. O Marketo só pode compartilhar dados de associação para clientes potenciais para os quais o Marketo sincronizou um ECID. Para obter os melhores resultados possíveis, é recomendável carregar o script de rastreamento munchkin.js do Marketo em paralelo ao código de rastreamento visitante.js do Adobe em todas as páginas que você está interessado em rastrear para fins de marketing.

**Como a sincronização de cookies funciona?**

Quando a sincronização de cookies estiver ativada para sua Subscrição do Marketo, o munchkin.js do Marketo tentará capturar e armazenar Adobe ECIDs para a Organização Adobe IMS especificada durante a configuração da integração e combinar esses ECIDs com o identificador de cookie do Marketo correspondente. Isso permite que os perfis de usuário anônimos do Marketo se tornem enriquecidos com ECIDs de Adobe.

Uma outra etapa é necessária para associar o perfil de usuário anônimo a um Perfil principal, que é identificado usando um email de texto simples. Exatamente como isso funciona está descrito aqui: [https://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People](https://docs.marketo.com/display/public/DOCS/Tracking+Anonymous+Activity+and+People).
