---
description: Limitação Da Conexão De Email - Documentação Do Marketo - Documentação Do Produto
title: Limitação da conexão de email
exl-id: 02450a1e-5b30-4057-b204-19fab1a7d6c9
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Limitação da conexão de email {#email-connection-throttling}

A integração da sua conta [!DNL Sales Connect] para envio por meio do [!DNL Exchange] ou de provedores de email do Gmail oferece uma configuração simplificada e otimiza a capacidade de entrega de emails para 1:1 comunicação de vendas. No entanto, para manter a integridade dos sistemas e a segurança das contas, o Gmail e o [!DNL Exchange] impõem limites de envio de email. Esses limites podem ser aumentados ou diminuídos a critério dos provedores.

## Limitação da conexão de email (Beta) {#email-connection-throttling-beta}

A limitação de conexão de email permite que os administradores do Sales Connect configurem a taxa de envio de emails ao usar o Gmail ou o Exchange como canal de entrega, para que a taxa na qual os emails sejam entregues ao provedor de canal de entrega não exceda os limites impostos.

Quando os limites são constantemente excedidos, isso pode ser visto às vezes como um comportamento suspeito do provedor de canal de entrega, causando falha nos emails e, às vezes, até mesmo uma conta é desativada.

**Notas/Destaques**

* Habilitado automaticamente quando um usuário se conecta ao Gmail ou [!DNL Exchange]
* Pode ser personalizado se você quiser aumentar ou diminuir as configurações da recomendação para atender às suas necessidades
* Apenas acelera emails enviados pelo Gmail ou [!DNL Exchange], não acelera o canal de entrega personalizado
* A limitação da Conexão de email enfileira emails de cada usuário individual separadamente, pois cada usuário tem sua própria conexão com o provedor de email

**Definindo as Configurações de Limitação da Conexão de Email**

1. Clique no ícone de engrenagem e selecione **[!UICONTROL Configurações]**.

   ![](assets/email-connection-throttling-1.png)

1. Em [!UICONTROL Configurações de Administração], clique em **[!UICONTROL Geral]**.

   ![](assets/email-connection-throttling-2.png)

1. No cartão Limitação da conexão de email à direita, clique no controle deslizante **[!UICONTROL Habilitar limitação de email]**.

   ![](assets/email-connection-throttling-3.png)

1. No cartão de Limitação de conexão de email à direita, insira o tamanho de lote desejado de emails que serão enviados para o provedor de canal de email.

   ![](assets/email-connection-throttling-4.png)

1. Defina o tempo de espera antes do envio de cada lote. Neste exemplo, estamos escolhendo 25 emails a cada 45 segundos.

   ![](assets/email-connection-throttling-5.png)

1. Clique em **[!UICONTROL Salvar]**.

   ![](assets/email-connection-throttling-6.png)

Com as alterações salvas, todos os usuários terão seus emails enviados em lotes para a conta do Gmail ou do [!DNL Exchange] conectada para entrega.

## Limites do provedor de email {#email-provider-limits}

**[!DNL Outlook 365]**

Business/Empresa

* 10 mil por dia
* 30 por minuto
* 500 recipients por email

Mais informações [podem ser encontradas aqui](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 2000 por dia (500 para contas de avaliação e sinalizadas)
* 2 emails por segundo (limite de API)
* 2.000 recipients por mensagem (máximo de 500 para recipients externos)

Mais informações [podem ser encontradas aqui](https://support.google.com/a/answer/166852?hl=en).

**[!DNL Microsoft Exchange Server (2010, 2013)]**

Os limites são definidos pelo departamento de TI da organização, pois o servidor é hospedado por ela. Entre em contato com o administrador da rede ou do sistema, conforme aplicável, para obter mais informações.

>[!MORELIKETHIS]
>
>* [Visão Geral Do Canal De Entrega](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Conexão de email para usuários do Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Conexão de Email para Usuários do Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
