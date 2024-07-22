---
unique-page-id: 1900597
description: Definir um público-alvo importando uma lista - Documentação do Marketo - Documentação do produto
title: Definir um público-alvo importando uma lista
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# Definir um público-alvo importando uma lista {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[Criar um Email para um Programa de Email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Depois de criar um programa de email, você deverá informar para quem enviar o email. Você pode fazer isso [criando uma lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) ou importando uma lista. Veja como fazer isso importando uma lista.

>[!NOTE]
>
>A definição do público só funcionará quando o programa de email não for aprovado.
>
>Qualquer campo de data/hora que for importado será tratado como Hora central. Se você tiver campos de data/hora em um fuso horário diferente, poderá usar uma fórmula do Excel para transformá-la na Hora Central (América/Chicago).

1. Vá para **Atividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Selecione seu programa de email e clique em Importar lista no bloco Público-alvo.

   ![](assets/importlist.png)

1. A janela de importação de lista é aberta. Clique em **Procurar** e selecione o arquivo que deseja importar. Depois de selecionar sua lista de pessoas, clique em **Avançar**.

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Verifique se a lista está codificada em UTF-8, UTF-16, Shift-JIS ou EUC-JP e se não excede 50 MB no tamanho do arquivo.

1. Verifique se os campos no arquivo estão mapeados corretamente e clique em **Avançar**.

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >O Marketo se lembrará dos mapeamentos para importações futuras!

1. Insira um **Nome** para a lista e clique em **Importar**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Quando a importação for concluída, volte para a guia principal do programa. Você verá quantas pessoas se qualificarão.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Definição**
>
>Você notou o número bloqueado? Esse número é um subconjunto de pessoas qualificadas e representa pessoas que não podem receber este email porque são:
>
>* Inscrição cancelada
>* Campanha de marketing suspensa
>* Incluído na lista de bloqueios
>* E-mail inválido
>* Email vazio
>
>Clique no número para obter uma lista detalhada de pessoas bloqueadas para emails.
>
>Use o botão ![—](assets/image2014-10-23-16-3a32-3a36-1.png) no bloco **Público-alvo** para ver quantas pessoas se qualificaram para receber o email com base nos critérios da lista inteligente. Subtraia o número Bloqueado do número Pessoas para obter o número total de pessoas que receberão o email.

>[!TIP]
>
>Não é necessário aguardar a conclusão da importação da lista. Você pode continuar trabalhando se quiser.

Fantástico! Agora é hora de escolher um email já existente ou criar um novo email para enviar a essas pessoas.

>[!MORELIKETHIS]
>
>* [Escolher um Email Existente](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [Criar um Email para um Programa de Email](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)
