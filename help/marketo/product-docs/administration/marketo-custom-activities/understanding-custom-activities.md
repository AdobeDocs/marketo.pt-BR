---
unique-page-id: 10100266
description: Visão geral das atividades personalizadas para rastrear ações de pessoas específicas de negócios, como elas diferem de objetos personalizados e a configuração de duas etapas da criação da atividade e da implementação da API.
title: Noções básicas de atividades personalizadas
exl-id: 0bb74d9d-3a9d-4ef7-8c8c-2de36cd6190b
feature: Custom Activities
source-git-commit: 7fe6ed8b9fcb1aacf0e651a11ab90eaf0ae07937
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 8%

---

# Noções básicas de atividades personalizadas {#understanding-custom-activities}

Monitore, com atividades personalizadas, uma ação específica de sua empresa empreendida por uma pessoa.

## O que são atividades {#what-are-activities}

Há várias maneiras de uma pessoa interagir com sua organização. Eles podem visitar o site da empresa, participar de uma de suas feiras comerciais ou clicar em um link em um email enviado a eles. Essas ações são atividades e, qualquer que seja a ação executada, a Marketo as captura para que sua equipe de marketing possa entender melhor como enviá-las em tempo hábil e com comunicação relevante.

## Atividades personalizadas {#custom-activities}

As atividades personalizadas ajudam você a rastrear uma atividade que não está relacionada a um formulário, email ou página de aterrissagem do Marketo. Para rastrear quando alguém deposita um cheque, use uma atividade personalizada. Para monitorar quando alguém participa de um webinário, use uma atividade personalizada.

>[!NOTE]
>
>As atividades personalizadas diferem dos objetos personalizados. Use objetos personalizados quando o valor puder mudar (ou seja, a &quot;cor do carro&quot; muda de azul para vermelho). Use atividades personalizadas ao rastrear momentos que ocorreram e seus detalhes não podem ser alterados (ou seja, &quot;carro comprado&quot;).

## Campos {#fields}

Você pode adicionar [campos adicionais](/help/marketo/product-docs/administration/marketo-custom-activities/add-edit-delete-marketo-custom-activity-fields.md) que deseja associar à atividade. Assim como o campo principal, eles podem ser usados como critérios de filtragem em uma lista inteligente.

## Introdução {#getting-started}

As atividades personalizadas funcionam da mesma forma que as atividades padrão. No entanto, a configuração deles é um processo de duas etapas.

Etapa 1: [Criar uma atividade personalizada](/help/marketo/product-docs/administration/marketo-custom-activities/create-a-custom-activity.md) em sua conta da Marketo

Etapa 2: o funcionário em sua organização que trabalha com a API do Marketo pode iniciar a implementação. Mais informações podem ser encontradas aqui: [API de atividade personalizada](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/addCustomActivityUsingPOST)
