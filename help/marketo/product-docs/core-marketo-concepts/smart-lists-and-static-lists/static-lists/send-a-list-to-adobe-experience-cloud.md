---
unique-page-id: 37356194
description: Enviar uma lista para o Adobe Experience Cloud - Documentação do Marketo - Documentação do produto
title: Enviar uma lista para o Adobe Experience Cloud
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
feature: Static Lists
source-git-commit: 8bc619b9b9a75c3b20a8f30ebf902ab4b881e627
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 1%

---

# Enviar uma lista para o Adobe Experience Cloud {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Uma implantação pronta para HIPAA de uma instância do Marketo Engage não pode usar esse recurso.

>[!PREREQUISITES]
>
>[Configurar o Adobe Organization Mapping](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Aplicativos de destino suportados {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (_somente_ se você tiver uma licença do Adobe Audience Manager)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-Time Customer Data Platform
* Adobe Target

## Como enviar uma lista estática {#how-to-send-a-static-list}

Uma lista estática é exatamente isso, estática. Nenhuma alteração ocorrerá na lista no Adobe Experience Cloud, a menos que você as faça manualmente.

1. No Marketo, encontre a lista que deseja exportar. Clique com o botão direito do mouse nele e selecione **[!UICONTROL Enviar para o Experience Cloud]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. Clique na lista suspensa **[!UICONTROL Pasta do Audience Manager]** e selecione a pasta de destino desejada na Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. Escolha se deseja criar um novo público ou substituir um já existente (neste exemplo, estamos criando um novo). Insira o novo nome de público e clique em **[!UICONTROL Enviar]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. Clique em **[!UICONTROL OK]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >Pode levar de 6 a 8 horas para que a associação de público-alvo seja totalmente preenchida no Adobe.

## Como enviar uma lista sincronizada {#how-to-send-a-synced-list}

Sincronizar uma lista significa que, sempre que você atualiza uma lista no Marketo, essa alteração é sincronizada automaticamente com o público-alvo no Adobe Experience Cloud.

1. No Marketo, encontre a lista que deseja exportar. Clique com o botão direito do mouse nele e selecione **[!UICONTROL Enviar para o Experience Cloud]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. Clique no menu suspenso **[!UICONTROL Pasta da biblioteca de público-alvo]** e selecione a pasta de destino desejada na Experience Cloud.

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. Escolha se deseja criar um novo público ou substituir um já existente (neste exemplo, estamos criando um novo). Insira o novo nome de público, marque a caixa **[!UICONTROL Manter associação de público-alvo em sincronização]** e clique em **[!UICONTROL Enviar]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. Clique em **[!UICONTROL OK]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## Como Interromper uma Sincronização de Lista {#how-to-stop-a-list-sync}

Você pode interromper a sincronização da sua lista a qualquer momento.

1. No Marketo, localize e clique com o botão direito do mouse na lista que deseja interromper a sincronização. Clique em **[!UICONTROL Interromper Sincronização de Lista]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. Selecione o(s) público(s) que deseja interromper a sincronização e clique em **[!UICONTROL Parar]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. Clique em **[!UICONTROL Parar]** para confirmar.

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## Itens a Observar {#things-to-note}

### Compartilhamento no Adobe Analytics {#sharing-to-adobe-analytics}

* Para usuários que possuem o Adobe Audience Manager e o Adobe Analytics, essa integração permitirá que os públicos-alvo sejam compartilhados do Marketo com seus Conjuntos de relatórios do Adobe Analytics. No entanto, há algumas etapas de configurações adicionais que precisam ser executadas no Adobe Audience Manager para habilitar isso. Consulte a [documentação da Adobe Audience Manager](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html?lang=pt-BR){target="_blank"} para obter mais informações sobre como configurar esta página.

* Depois que uma lista é carregada do Marketo para o Adobe Audience Manager, ela também pode ser acessada pelo Adobe Target. Esta configuração [precisa ser habilitada no Adobe Target](https://experienceleague.adobe.com/pt-br/docs/target/using/integrate/audience-manager-target-integration){target="_blank"}.

* Se uma lista estiver vazia ou não tiver pessoas com valores ECID, o nome da lista não será enviado para ser referenciado fora do Marketo.

### Uso de características para clientes do Adobe Audience Manager {#trait-usage-aam}

Ao iniciar uma exportação de lista no Marketo, você observará as seguintes alterações refletidas na instância do Adobe Audience Manager:

* Para todas as Pessoas na Lista exportada, o Marketo gravará uma característica usando seus emails com hash como um Identificador entre dispositivos. O nome da característica corresponderá ao Nome do público-alvo de destino especificado durante a exportação.
* Para todos os ECIDs que o Marketo conseguiu corresponder às Pessoas na Lista exportada, o Marketo gravará uma característica usando o Identificador de dispositivo ECID. O nome da característica corresponderá ao Nome do público-alvo de destino especificado durante a exportação.
* O Marketo também criará um segmento na sua instância do Audience Manager usando a característica da ECID como o único critério de segmentação. O nome do segmento corresponderá ao Nome do público-alvo de destino especificado durante a exportação.

## Perguntas frequentes {#faq}

**Por que o tamanho da lista no Marketo é diferente do tamanho da lista no Adobe?**

Por baixo dos panos, a integração do público-alvo funciona sincronizando os cookies do Marketo Munchkin com o cookie correspondente do Adobe ECID. O Marketo só pode compartilhar dados de associação de pessoas para as quais a Marketo sincronizou uma ECID. Para obter os melhores resultados possíveis, é recomendável carregar o script de rastreamento munchkin.js do Marketo em paralelo com o código de rastreamento visitor.js do Adobe em todas as páginas nas quais você está interessado em rastrear para fins de marketing.

**Como funciona a sincronização de cookies?**

Quando a sincronização de cookies estiver ativada para sua assinatura do Marketo, o munchkin.js da Marketo tentará capturar e armazenar ECIDs do Adobe para a Organização IMS da Adobe especificada durante a configuração de integração e corresponder essas ECIDs ao identificador de cookie do Marketo correspondente. Isso permite que perfis de usuários anônimos da Marketo sejam enriquecidos com ECIDs do Adobe.

Uma outra etapa é necessária para associar o perfil de usuário anônimo a um Perfil de pessoa, que é identificado usando um email de texto sem formatação. [está descrito aqui](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"} como isto funciona exatamente.

**Que informações são compartilhadas?**

Essa integração compartilha somente informações de associação de lista do Marketo para a Adobe (por exemplo, o conhecimento de que a Pessoa X é membro da Lista Y). Nenhum atributo de pessoa adicional é compartilhado para a Adobe por meio dessa integração.
