---
solution: Marketo Engage
product: marketo
title: Spam Assassin
description: O TEXTO É INSERIDO AQUI
level: Beginner, Intermediate
feature: Email Editor
hide: true
hidefromtoc: true
source-git-commit: 0157bc64444151a43bf464158d508e84d75b3427
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Spam Assassin {#spam-assassin}

Usando o SpamAssassin no Marketo Engage, você pode testar seu conteúdo de e-mail e ver a probabilidade de ISPs/provedores de caixa de correio marcá-lo como spam.

O SpamAssassin analisa seu conteúdo e atribui uma pontuação com base em vários critérios. Quanto menor a pontuação, melhor. É importante manter uma pontuação baixa, pois o envio de emails com uma pontuação alta pode afetar negativamente a capacidade geral de entrega.

## Acessar o relatório de spam {#access-the-spam-report}

1. Na tela Simular, clique no botão **Relatório de spam**.

CAPTURA DE TELA

1. Um relatório de spam é gerado.

CAPTURA DE TELA

1. Verifique as pontuações e descrições de cada item.

>[!IMPORTANT]
>
>Se a pontuação geral for superior a 5, seu email poderá ser bloqueado ou marcado como spam no momento do delivery.

1. Se você considerar a pontuação muito alta, edite o conteúdo no Designer de email e execute novamente o relatório de spam até que a pontuação esteja onde deseja que ele esteja.

CAPTURA DE TELA

>[!NOTE]
>
>A pontuação de spam é derivada do SpamAssassin e as regras não são de propriedade da Adobe. Mais detalhes sobre essas regras podem ser encontrados na [documentação do SpamAssassin](https://spamassassin.apache.org/#_blank). Uma lista completa de erros [pode ser vista aqui](https://spamassassin.apache.org/old/tests_3_0_x.html?utm_source=chatgpt.com).
