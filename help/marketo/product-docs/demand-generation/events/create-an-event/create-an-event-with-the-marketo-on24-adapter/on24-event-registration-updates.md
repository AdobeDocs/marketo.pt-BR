---
unique-page-id: 10096683
description: Atualizações de registro do Evento ON24 - Documentos do marketing - Documentação do produto
title: Atualizações de registro do Evento ON24
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# Atualizações de registro de Eventos ON24 {#on-event-registration-updates}

## Aprovação manual de registrantes {#manually-approving-registrants}

Você pode aprovar manualmente seus inscritos antes de enviar um email de confirmação. Para fazer isso, você precisará configurar suas campanhas para lidar com esta etapa adicional:

1. Para a Campanha do acionador de registro:

   * Na Lista inteligente, defina o acionador como **Preenche o formulário**.
   * No Fluxo, defina o Status em Progressão como **Aprovação pendente**.

1. Vá para o Evento e clique na guia **Membros**. Esta guia exibe todas as pessoas que preencheram o formulário. Seu status deve ser definido como **Aprovação pendente**.
1. Use o filtro na parte superior da grade para visualização somente das pessoas com status **Aprovação pendente**.
1. Selecione as pessoas que deseja registrar (clique com a tecla Shift pressionada, clique com a tecla Ctrl pressionada ou selecione todas).
1. No menu, clique em **Alterar status**. Selecione **Registrado**, **Rejeitada** ou qualquer outro status aplicável.

## Tratamento de pessoas com um erro de registro {#handling-people-with-a-registration-error}

Se uma pessoa acabar não sendo registrada, mas sim definida como o status Erro de registro, não é tarde demais para recuperar.

1. Na guia Membros, filtre a lista de pessoas com o status **Erro de registro**.
1. Antes de continuar, verifique se você determinou e corrigiu o problema com a integração (verifique se não há erros em **Parceiros de Evento** em Admin).
1. Depois que o problema for resolvido, selecione todas as pessoas com o status de Erro de registro e altere seu status para **Registrado**. Isso tentará registrá-los novamente com ON24.

## Atualizando o Status do Membro de ON24 {#updating-member-status-from-on}

O Marketo coleta automaticamente as informações de presença às 11h do Pacífico por noite. Para atualizar manualmente as informações de presença, clique em **Atualizar do Provedor de Webinar** em **Ações do Evento**.

>[!MORELIKETHIS]
>
>* [Noções Gerais dos Eventos do adaptador do Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



