---
unique-page-id: 11375827
description: Campos obrigatórios para sincronização de marketing com dinâmicas - Documentos do marketing - Documentação do produto
title: Campos necessários para sincronizar o marketing com o Dynamics
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---


# Campos necessários para sincronizar o marketing com o Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Esses campos *devem* ser sincronizados com o Marketo para clientes potenciais e para que o Contact for Sales Insight funcione:

* Prioridade
* Urgência
* Pontuação relativa

Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, verifique sua instância para ter certeza de que os campos estão sincronizados para **Lead** e **Contact**. Caso contrário, adicione-os.

Veja como verificar e adicionar campos de sincronização.

1. Vá para Admin e clique em Microsoft Dynamics.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em Editar em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Em Lead, marque a caixa de seleção Prioridade.

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Agora, role para baixo e marque a caixa de seleção Urgência...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...e a caixa de seleção Pontuação relativa.

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Em seguida, marque as caixas de seleção Prioridade, Urgência e Pontuação relativa para contato.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Clique em Salvar.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Aguarde pelo menos 10 minutos para que uma sincronização seja executada antes de verificar se você corrigiu o problema.

>[!MORELIKETHIS]
>
>[Configuração de estrelas e chamas para registros de cliente potencial/contato](http://docs.marketo.com/x/BICMAg)

