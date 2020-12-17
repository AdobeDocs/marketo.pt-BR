---
unique-page-id: 1900597
description: Definir uma Audiência importando uma Lista - Documentos do Marketing - Documentação do produto
title: Definir uma Audiência importando uma Lista
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Definir uma Audiência importando uma Lista {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[Criar um email para um Programa de email](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Depois de criar um programa de e-mail, você desejará dizer a ele para quem enviar o e-mail. Você pode fazer isso ao [criar uma lista inteligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) ou importando uma lista. Veja como fazer isso importando uma lista.

>[!NOTE]
>
>A definição da sua audiência só funcionará quando o programa de e-mail não for aprovado.
>
>Todos os campos de data/hora que estão sendo importados são tratados como Hora Central. Se você tiver campos de data/hora em um fuso horário diferente, poderá usar uma fórmula do Excel para transformá-la em Hora Central (América/Chicago).

1. Vá para **Atividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

   Selecione seu programa de e-mail e clique em Importar Lista sob o título Audiência.
   ![](assets/importlist.png)

1. A janela de importação de lista é aberta, clique em **Procurar** e selecione o arquivo que deseja importar. Depois de selecionar sua lista de pessoas, clique em Avançar.
1. ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Verifique se a lista está codificada em UTF-8, UTF-16, Shift-JIS ou EUC-JP e não excede 50 MB no tamanho do arquivo.

   Verifique se os campos no arquivo estão mapeados corretamente e clique em Avançar.
   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo vai lembrar dos mapeamentos para importações futuras!

1. Digite um **Nome** para sua lista e clique em **Importar**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Quando a importação estiver concluída, volte para a guia programa principal. Você verá quantas pessoas se qualificarão.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Definição**
>
>Você notou o número Bloqueado? Este número é um subconjunto de pessoas qualificadas e representa pessoas que não podem receber este email porque são:
>
>* Inscrito
>* Suspenso de marketing
>* incluir na lista de bloqueios
>* Email Inválido
>* Email vazio

>
>
Clique no número para obter uma lista detalhada de pessoas bloqueadas de correspondências.
>
>Use o botão ![—](assets/image2014-10-23-16-3a32-3a36-1.png) no bloco **Audiência** para ver quantas pessoas estão qualificadas para receber o email com base em critérios de lista inteligente. Subtraia o número Bloqueado do número de Pessoas para obter o número total de pessoas que receberão o email.

>[!TIP]
>
>Você não precisa esperar a importação da lista terminar. Você pode continuar trabalhando se quiser.

Fantástico! Agora é hora de escolher um email já existente ou criar um novo email para enviar a essas pessoas.

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Escolher um email existente](../../../../product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [Criar um email para um Programa de email](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

>



