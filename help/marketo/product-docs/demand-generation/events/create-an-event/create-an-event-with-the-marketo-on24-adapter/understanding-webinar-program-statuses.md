---
unique-page-id: 10096681
description: Noções básicas sobre os status do programa de webinário - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre os status do programa de webinário
exl-id: ef0b1b94-a612-4aa8-9b4a-aa7ef0e2abaa
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 1%

---

# Noções básicas sobre os status do programa de webinário {#understanding-webinar-program-statuses}

Os status do programa representam os diferentes status de evento pelos quais uma pessoa avança como membro do evento. Eles são associados a um tipo de canal. O Marketo tem um tipo de canal interno chamado **Webinar**. Os status podem ser usados em campanhas em lote e de acionador.

As pessoas passam pelos status do programa de forma linear e não voltam ao status. Por exemplo, uma pessoa com o status **Participou** não pode voltar para **Registrado**.

Aqui está uma breve descrição dos status do programa associados ao canal do webinário.

>[!TIP]
>
>Para atualizar os status manualmente, clique em **Atualizar do Provedor de Webinar** na lista suspensa **Ações de Evento**.

![](assets/image2015-12-17-13-3a52-3a39.png)

**Não está no Programa** - Use este status para remover pessoas do evento.

**Convidado** - Use este status para adicionar pessoas ao evento.

**Aprovação pendente** - use esse status para não enviar um email de confirmação para sua equipe. Consulte &quot;Aprovando Manualmente Inscritos&quot; em [ON24 Atualizações de Registro de Eventos](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"} para obter mais informações.

**Em Lista de Espera** - Use este status para manter algumas pessoas esperando até que vagas adicionais sejam disponibilizadas.

**Rejeitado** - Use este status para rejeitar o registro de uma pessoa no seu Evento.

**Registrado** - Este status envia as pessoas para ON24 quando você está usando a integração ON24. O status da pessoa é atualizado quando ON24 responde que a pessoa foi registrada com êxito.

**Erro de Registro** - Esse status reflete que o usuário encontrou um erro ao tentar se registrar no Evento.

>[!NOTE]
>
>Se ocorrer um erro de registro, você poderá obter informações adicionais sobre essa pessoa observando a coluna Motivo do Status na guia Membros do seu programa. Depois que o erro for corrigido, você poderá alterar manualmente o status do programa do usuário para Registrado no Marketo.

**Participou** - Na conclusão do webinário, ON24 retorna uma lista de pessoas que participaram. Esse status é enviado automaticamente para o Marketo.

**Participou sob demanda** - As pessoas que participaram da versão arquivada do webinário recebem esse status.

**Sem programa** - Na conclusão do webinário e após os dados de participação serem obtidos do ON24, o status das pessoas que se registraram, mas não participaram, é atualizado para Sem programa. Pode levar de 30 minutos a 3 horas para que o ON24 prepare as informações finais de participação e as disponibilize no Marketo.

>[!NOTE]
>
>Para que o Marketo obtenha o status Não Mostrar, as pessoas devem ter sido registradas *no Marketo*. Não é possível capturar Nenhum programa que vem do feed de dados On24.

>[!MORELIKETHIS]
>
>[Noções Básicas sobre os Eventos do Adaptador Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
