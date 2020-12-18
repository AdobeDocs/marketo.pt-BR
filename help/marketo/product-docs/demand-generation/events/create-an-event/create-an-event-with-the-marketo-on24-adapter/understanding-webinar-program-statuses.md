---
unique-page-id: 10096681
description: Entendendo os status do Programa do Webinar - Documentos do Marketing - Documentação do produto
title: Entendendo os status dos Programas do webinar
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---


# Entendendo os status do Programa do Webinar {#understanding-webinar-program-statuses}

Os status dos programas representam os diferentes status dos eventos pelos quais uma pessoa progride como membro do evento. Eles estão associados a um tipo de canal. O Marketo tem um tipo de canal incorporado chamado **Webinar**. Os status podem ser usados em campanhas de lote e acionador.

As pessoas se movem através dos status dos programas de forma linear e não retornam ao status. Por exemplo, uma pessoa com um status de **Participante** não pode voltar para **Registrado**.

Esta é uma breve descrição dos status dos programas associados ao canal do Webinar.

>[!TIP]
>
>Para atualizar manualmente os status, clique em **Atualizar do Provedor de Webinar** no menu suspenso **Ações do Evento**.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Não está no Programa**  - Use este status para remover pessoas do evento.

** Convidado** - Use este status para adicionar pessoas ao evento.

**Aprovação**  pendente - Use este status para suspender o envio de um email de confirmação para seu pessoal. Consulte &quot;Aprovação manual de inscritos&quot; em [Atualizações de registro de Eventos ON24](on24-event-registration-updates.md) para obter mais informações.

**Lista**  de espera - Use esse status para manter algumas pessoas esperando até que mais lugares fiquem disponíveis.

**Rejeitada**  - Use esse status para rejeitar o registro de uma pessoa em seu Evento.

**Registrado**  - Esse status empurra as pessoas para ON24 quando você está usando a integração ON24. O status da pessoa é atualizado quando a ON24 responde que a pessoa foi registrada com êxito.

**Erro**  de registro - Esse status reflete que o usuário encontrou um erro ao tentar se registrar no Evento.

>[!NOTE]
>
>Se ocorrer um erro de registro, você poderá obter informações adicionais para essa pessoa, observando a coluna Motivo do status na guia Membros do seu programa. Após corrigir o erro, é possível alterar manualmente o status do programa do usuário para Registrado no Marketo.

**Participante** - Na conclusão do webinar, o ON24 retorna uma lista de pessoas que participaram. Esse status é automaticamente direcionado para o Marketo.

**Participou sob demanda**  - as pessoas que participaram da versão arquivada do webinar recebem esse status.

**Não mostrar** - Na conclusão do webinar e depois que os dados de participação forem obtidos a partir do ON24, o status das pessoas que se registraram mas não participaram é atualizado para Sem mostrar. Pode levar de 30 a 3 horas para que o ON24 prepare as informações finais de presença e disponibilize-as no Marketo.

>[!NOTE]
>
>Para que o Marketo obtenha o status No Show, as pessoas devem ter sido registradas *no Marketo*. Não conseguimos capturar Nenhuma Mostra proveniente do feed de dados On24.

>[!MORELIKETHIS]
>
>* [Noções Gerais dos Eventos do adaptador do Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



