---
unique-page-id: 10096681
description: Noções básicas sobre os status do programa do webinar - Documentação da Marketo - Documentação do produto
title: Noções básicas sobre os status do programa do webinar
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Noções básicas sobre os status do programa do webinar {#understanding-webinar-program-statuses}

Os status do programa representam os diferentes status de evento que uma pessoa avança como membro do evento. Eles estão associados a um tipo de canal. O Marketo tem um tipo de canal integrado chamado **Webinar**. Os status podem ser usados em campanhas de lote e de acionador.

As pessoas se movem pelos status do programa de maneira linear e não retornam ao status. Por exemplo, uma pessoa com status de **Participante** não é possível voltar para **Registrado**.

Esta é uma breve descrição dos status do programa associados ao canal Webinar.

>[!TIP]
>
>Para atualizar os status manualmente, clique em  **Atualizar do provedor de webinar** no **Ações do evento** lista suspensa.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Não está no programa** - Use esse status para remover pessoas do evento.

**Convidado** - Use esse status para adicionar pessoas ao evento.

**Aprovação pendente** - Use esse status para não enviar ao seu pessoal um email de confirmação. Consulte &quot;Aprovar registrantes manualmente&quot; em [Atualizações do registro de eventos ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target=&quot;_blank&quot;} para obter mais informações.

**Aguardar Lista** - Utilizar este estatuto para manter algumas pessoas à espera até que estejam disponíveis lugares adicionais.

**Rejeitada** - Use esse status para rejeitar o registro de uma pessoa em seu Evento.

**Registrado** - Esse status empurra as pessoas para ON24 quando você está usando a integração ON24. O status da pessoa é atualizado quando ON24 responde que a pessoa foi registrada com sucesso.

**Erro de Registro** - Esse status reflete que o usuário encontrou um erro ao tentar se registrar no Evento.

>[!NOTE]
>
>Se ocorrer um erro de registro, você poderá obter informações adicionais para essa pessoa, observando a coluna Motivo do Status na guia Membros do seu programa. Depois que o erro for corrigido, é possível alterar manualmente o status do programa do usuário para Registered in Marketo.

**Participante** - Na conclusão do webinário, ON24 retorna uma lista de pessoas que participaram. Esse status é enviado automaticamente para o Marketo.

**Atendido sob demanda** - As pessoas que participaram da versão arquivada do webinário recebem esse status.

**Sem programa** - Na conclusão do webinário e após a retirada dos dados de presença da ON24, o status das pessoas que se registraram mas não participaram é atualizado para Sem programa. Pode levar de 30 minutos a 3 horas para que a ON24 prepare as informações finais de presença e as disponibilize no Marketo.

>[!NOTE]
>
>Para que o Marketo obtenha o status No Show , as pessoas devem ter sido registradas *no Marketo*. Não é possível capturar Nenhuma exibição proveniente do feed de dados On24.

>[!MORELIKETHIS]
>
>[Noções básicas sobre os eventos do adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target=&quot;_blank&quot;}
