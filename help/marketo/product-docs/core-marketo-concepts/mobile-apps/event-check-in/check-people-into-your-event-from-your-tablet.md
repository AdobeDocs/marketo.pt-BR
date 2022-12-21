---
unique-page-id: 2949839
description: Verifique as pessoas no seu evento do tablet - Documentos do Marketo - Documentação do produto
title: Verifique as pessoas no seu evento do seu tablet
exl-id: b48f5f95-8e36-441f-a785-1651f42f9f60
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Verifique as pessoas no seu evento do seu tablet {#check-people-into-your-event-from-your-tablet}

Quando as pessoas aparecem no seu evento, você pode encontrar suas informações no aplicativo. Após o check-in, eles são promovidos para o status de Participante quando você sincroniza com o Marketo.

O aplicativo funciona da mesma forma no iPad e no Android, exceto pequenas diferenças de layout e design.

>[!PREREQUISITES]
>
>* Crie um evento no Marketo e preencha-o com Pessoas convidadas e registradas.
>* Baixe o aplicativo para tablet para [Android](https://play.google.com/store/apps/details?id=com.marketo.eventcheckin&amp;hl=en) ou [iOS](https://itunes.apple.com/us/app/marketo-events/id522766637?mt=8)


## Verificar Convidados Registrados {#check-in-registered-guests}

1. Toque no ícone do aplicativo no tablet iPad ou Android.

1. Toque **Logon** para iniciar o aplicativo Marketo Event.

   ![](assets/1.jpg)

1. Digite seu nome de usuário e senha do Marketo e clique em **Logon**.

   >[!NOTE]
   >
   >Você deve ter uma função com acesso ao Banco de Dados para ver as pessoas no aplicativo.

1. Selecione um **Evento**.

   ![](assets/2.jpg)

   >[!TIP]
   >
   >Somente os programas de eventos (com exceção dos webinars) agendados uma semana antes e uma semana depois da data de hoje são exibidos.

1. Na tela inicial, navegue para encontrar convidados registrados. Para localizar uma pessoa na lista, você pode:

   * Rolar para localizar um nome
   * Insira um nome no campo de pesquisa
   * Pule para uma letra inicial específica do sobrenome tocando-a no lado direito da lista

   >[!NOTE]
   >
   >O processo é o mesmo no iPad e no Android, mas as telas são diferentes e os itens podem estar em locais diferentes. Este artigo apresenta a interface do iPad. Compare a tela Android nesta seção para referência.

   **iPad**

   ![](assets/image2016-4-15-11-3a55-3a11.png)

   **Android**

   ![](assets/image2016-4-15-14-3a50-3a19.png)

1. Toque no nome selecionado e, no registro de pessoa, toque em **Check-in**.

   ![](assets/img-0068-35-hands.png)

O convidado agora tem um status de Participante e recebe uma marca de seleção. O registro de pessoa é atualizado ao sincronizar com o Marketo. O contador vermelho no botão Sincronizar é incrementado para mostrar o número de check-ins desde a última sincronização com o Marketo. O botão Sincronizar é diferente e está em um local diferente para iPad e Android:

**iPad**

![](assets/image2016-4-12-14-3a25-3a13.png)

**Android**

![](assets/image2016-4-15-14-3a58-3a6.png)

>[!TIP]
>
>Se uma pessoa for convidada mas não tiver registrado, você poderá pesquisá-la clicando em **Pesquisar no servidor**, logo abaixo da caixa Pesquisar . O status do Convite é alterado para **Participante** para o evento .

## Criar uma nova pessoa no tablet {#create-a-new-person-on-the-tablet}

Você pode adicionar convidados manualmente que não são pessoas existentes no banco de dados do Marketo. Eles serão automaticamente marcados e adicionados ao seu banco de dados ao sincronizar com o Marketo.

1. Clique em **Adicionar**.

   **iPad**

   ![](assets/image2016-4-15-11-3a58-3a51.png)

   **Android**

   ![](assets/image2016-4-15-15-3a2-3a38.png)

1. Preencha quantos campos de informações básicas puder e toque em **Concluído**.

   ![](assets/image2016-4-15-11-3a33-3a59.png)

   >[!NOTE]
   >
   >Você só pode usar os campos existentes. Não é possível criar personalizados.

   >[!CAUTION]
   >
   >Verifique novamente o endereço de email. Outros campos podem ser corrigidos posteriormente, mas o endereço de email é o método principal para entrar em contato com o convidado.

A nova pessoa é registrada como check-in no seu evento e será adicionada ao banco de dados do Marketo com status de Participante ao sincronizar com o Marketo.

## Inverter uma Check-in {#reverse-a-check-in}

Se você fez check-in em uma pessoa por engano, _antes de sincronizar com o Marketo_, você pode reverter o status Attended .

1. Toque no nome na lista e, no registro da pessoa, toque em **Desfazer**.

   ![](assets/image2016-4-15-11-3a38-3a31.png)

   Tudo corrigido!

## Editar um registro de pessoa no check-in {#edit-a-person-record-at-check-in}

Você pode adicionar e modificar informações do convidado, diretamente no evento!

1. Toque no nome na lista de pessoas e toque em **Editar**.

   ![](assets/image2016-4-15-11-3a43-3a46.png)

1. Edite e adicione informações aos campos e toque em **Concluído**.

   ![](assets/image2016-4-15-11-3a50-3a18.png)

   >[!NOTE]
   >
   >No Android, a variável **Concluído** pode estar oculto. Role para baixo para encontrá-lo.

As informações serão atualizadas quando você sincronizar o aplicativo com o Marketo.

## Sincronizar o aplicativo com o Marketo {#sync-the-app-with-marketo}

O aplicativo Marketo Events funciona independentemente até que você sincronize sua atividade de volta ao banco de dados do Marketo. É melhor sincronizar o mais rápido possível após o último check-in. O seu comprimido tem de estar ligado à Internet.

>[!CAUTION]
>
>Depois de sincronizar, não é possível reverter um check-in do aplicativo.

1. No tablet, abra o aplicativo e navegue até o evento .

1. Toque **Sincronizar**.

   Seu evento é atualizado com novos check-ins no banco de dados do Marketo. O contador vermelho no botão Sincronizar apaga, até que você verifique outra pessoa no.

   Por motivos de segurança, você deve sair do aplicativo Marketo Events depois de concluir a sincronização.

## Trabalhando com acesso limitado à Internet {#working-with-limited-internet-access}

Alguns locais têm péssimo acesso à Internet. Você precisa de uma boa conexão para:

* Baixe e instale o aplicativo
* Login
* Selecionar um evento
* Sincronizar o aplicativo com o Marketo

Se estiver preocupado com o acesso à Internet no local, talvez você queira fazer logon no aplicativo Marketo Events e selecionar seu evento antecipadamente, em um local com acesso intenso à Internet. Dessa forma, você ainda pode usar o aplicativo offline. Em seguida, ao recuperar uma conexão com a Internet, sincronize imediatamente com o banco de dados do Marketo.

>[!TIP]
>
>Se você não tiver uma conexão com a Internet, ainda poderá criar uma nova pessoa para uma pessoa fazendo check-in. Ele será reconciliado com a pessoa existente ao sincronizar o aplicativo.

>[!NOTE]
>
>O aplicativo encerra a sessão automaticamente após oito horas de inatividade.
