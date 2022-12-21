---
unique-page-id: 11375827
description: Campos obrigatórios para sincronizar o Marketo com o Dynamics - Marketo Docs - Documentação do produto
title: Campos obrigatórios para sincronizar o Marketo com o Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 2%

---

# Campos obrigatórios para sincronizar o Marketo com o Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Esses campos *must* ser sincronizado com a Marketo para que o Lead e o Contato para o Insight de vendas funcionem:

* Prioridade
* Urgência
* Pontuação relativa

Se algum desses campos estiver ausente, você verá uma mensagem de erro no Marketo com o nome dos campos ausentes. Para corrigir isso, verifique em sua instância para ter certeza de que os campos estão sincronizados para ambos **Líder** e **Contato**. Caso contrário, adicione-os.

Veja como verificar e adicionar campos de sincronização.

1. Acesse Admin e clique em **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clique em **Editar** em Detalhes de sincronização de campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Em Lead, marque a caixa de seleção Prioridade .

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Agora, role para baixo e marque a caixa de seleção Urgência ...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...e a caixa de seleção Pontuação relativa .

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Em seguida, marque as caixas de seleção Prioridade, Urgência e Pontuação relativa para contato.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Clique em **Salvar**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Aguarde pelo menos 10 minutos para que a sincronização seja executada antes de verificar se você corrigiu o problema.

>[!MORELIKETHIS]
>
>[Configuração de estrelas e chamas para registros de lead/contato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
