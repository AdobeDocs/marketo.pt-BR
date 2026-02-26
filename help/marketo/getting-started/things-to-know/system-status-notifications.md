---
description: Assinar notificações de status do sistema - Documentação do Marketo Engage - Documentação do produto
title: Assinar Notificações de Status do Sistema
feature: Getting Started
hide: true
hidefromtoc: true
exl-id: f4404a26-3b86-4dc7-8ecb-52a24fdb09b4
source-git-commit: 700e1c62e00ce8d8f510637233de42636e5b90cb
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 1%

---

# Assinar notificações de status do sistema {#subscribe-to-system-status-notifications}

Saiba como assinar notificações de status diferentes para se manter atualizado sobre problemas atuais.

>[!PREREQUISITES]
>
>Antes de criar uma assinatura, primeiro identifique em qual data center e pod/servidor sua assinatura está localizada.

## Identificar o data center {#identify}

+++Identifique seu data center e pod/servidor

1. Na seção **Admin** do Marketo Engage, clique em **Minha conta**.

   ![](assets/subscribe-to-system-status-notifications-1.png)

1. Role para baixo até _Informações de suporte_.

   ![](assets/subscribe-to-system-status-notifications-2.png)

No campo _Data center_, as letras são o data center e os números são o pod. No exemplo acima, o usuário está em nosso data center Ashburn no pod 49.

Na etapa 7 de [criando uma assinatura](#create-a-subscription), esse usuário selecionaria a localização regional **Marketo Ashburn** e o pod **ab49**.

<table style="width:300px;">
  <tr>
    <th colspan="2">Abreviações do data center</th>
  </tr>
  <tr>
    <td style="width:25%;">ab</td>
    <td>Ashburn</td>
  </tr>
  <tr>
    <td style="width:25%;">sj</td>
    <td>San Jose</td>
  </tr>
  <tr>
    <td style="width:25%;">sn</td>
    <td>Sydney</td>
  </tr>
  <tr>
    <td style="width:25%;">lon</td>
    <td>Londres</td>
  </tr>
  <tr>
    <td style="width:25%;">nld</td>
    <td>Amsterdam</td>
  </tr>
</table>

>[!TIP]
>
>Esse método também pode ser usado para identificar em qual pod/servidor do Real Time Personalization (RTP) sua assinatura está.

+++

## Criar uma assinatura {#create-a-subscription}

Depois de [identificar seu data center e pod/servidor](#identify), siga as etapas abaixo para criar uma assinatura.

1. Em [status.adobe.com](https://status.adobe.com/pt-BR), clique em **Gerenciar assinaturas**.

   ![](assets/subscribe-to-system-status-notifications-3.png)

1. Entre (se ainda não estiver usando) com suas credenciais da Adobe ou clique em **Criar uma conta**, se ainda não tiver uma.

   ![](assets/subscribe-to-system-status-notifications-4.png)

1. Fique na guia _Descrições do produto_ e clique em **Criar assinaturas**.

   ![](assets/subscribe-to-system-status-notifications-5.png)

1. Clique no ícone do ![sinal de adição](assets/icon-plus-sign.png) ao lado de _Experience Cloud_ para expandir o menu. Faça o mesmo para _Adobe Marketo Engage_.

   ![](assets/subscribe-to-system-status-notifications-6.png){width="800"}

1. Selecione as ofertas/serviços de produtos sobre os quais você deseja receber notificações e clique em **Continuar**.

   >[!TIP]
   >
   >Marque _Adobe Marketo Engage_ para selecionar tudo.

   ![](assets/subscribe-to-system-status-notifications-7.png){width="800"}

1. Selecione os tipos de evento desejados.

   ![](assets/subscribe-to-system-status-notifications-8.png)

   <table style="width:500px;">
   <tr>
   <td style="width:35%;"><b>Problema grave de serviço</b></td>
   <td>Indisponibilidade de serviço ou grave degradação de desempenho para vários usuários em sistemas de produção.</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>Problema pequeno de serviço</b></td>
   <td>Indisponibilidade parcial do serviço ou degradação moderada do desempenho para vários usuários em sistemas de produção.</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>Manutenção do serviço</b></td>
   <td>Janelas programadas para executar a manutenção do produto que pode afetar a disponibilidade ou o desempenho do produto.</td>
   </tr>
   <tr>
   <td style="width:35%;"><b>Anúncios</b></td>
   <td>Mensagens globais, da família de produtos ou relacionadas ao produto com amplo impacto.</td>
   </tr>
   </table>

1. Selecione o local regional e o ambiente. Clique em **Continuar**.

   ![](assets/subscribe-to-system-status-notifications-9.png){width="900"}

   >[!NOTE]
   >
   >Se você perdeu o local para encontrar isso, consulte [Identificar seu data center](#identify).

1. Escolha sua preferência de assinatura, **Email** ou **Slack**, e clique em **Continuar**.

   ![](assets/subscribe-to-system-status-notifications-10.png)

1. Revise suas seleções e clique em **Confirmar preferências**.

   ![](assets/subscribe-to-system-status-notifications-11.png)
