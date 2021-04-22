---
unique-page-id: 1147114
description: Tokens de campo personalizado do membro do programa - Documentos do Marketo - Documentação do produto
title: Tokens de campo personalizado do membro do programa
exl-id: 3046dec8-b885-4b08-baa9-896bcf3594b2
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 2%

---

# Tokens de campo personalizados do membro do programa {#program-member-custom-field-tokens}

## Suporte de token para campos personalizados do membro do programa {#token-support-for-program-member-custom-fields}

Na parte de trás dos recursos Campos personalizados do membro do programa, o suporte está sendo estendido para os Campos personalizados do membro do programa nas estruturas de token.

Os tokens PMCF serão suportados no domínio membro da família de tokens.

Tokens de Membro são usados para campos do escopo do Membro do Programa. A partir do estado atual, Tokens de Membro também são usados para inserir valores exclusivos de parceiros de serviços integrados. `{{member.webinar url}}` O token resolve automaticamente o URL de confirmação exclusivo da pessoa gerado pelo provedor de serviços. {{member.registration code}} resolve o código de registro fornecido pelo provedor de serviços.

>[!NOTE]
>
>* Os Campos Personalizados do Membro do Programa podem ser usados somente no contexto de um programa.
>* Os tokens de campos personalizados do membro do programa não podem ser usados em: scripts de email, pré-cabeçalho de email, tokens de data em etapas de espera ou trechos.
>* O Status de Membro do Programa não é suportado em Tokens de Membro.


## Usando tokens de campo personalizados de membro do programa no Assets {#using-program-member-custom-field-tokens-in-assets}

Você pode inserir tokens de campos personalizados de membros do programa em emails, páginas de aterrissagem, SMS, notificações por push e Webhooks.

**E-mails**

1. Selecione o email desejado e clique em **Editar rascunho**.

   ![](assets/program-member-custom-field-tokens-1.png)

1. Clique no ícone Inserir token.

   ![](assets/program-member-custom-field-tokens-2.png)

1. Encontre e selecione o Token de Campo Personalizado do Membro do Programa desejado, insira um valor padrão e clique em **Inserir**.

   ![](assets/program-member-custom-field-tokens-3.png)

1. Clique em **Salvar**.

   ![](assets/program-member-custom-field-tokens-4.png)

>[!NOTE]
>
>Não se esqueça de aprovar seu email.

**páginas**

1. Selecione a Landing Page e clique em **Editar rascunho**.

   ![](assets/program-member-custom-field-tokens-5.png)

   >[!NOTE]
   >
   >O designer da landing page é aberto em uma nova janela.

1. Clique duas vezes na caixa de rich text à qual deseja adicionar o token.

   ![](assets/program-member-custom-field-tokens-6.png)

1. Clique no local em que deseja que o token fique e clique no ícone Inserir token.

   ![](assets/program-member-custom-field-tokens-7.png)

1. Localize e selecione o token desejado.

   ![](assets/program-member-custom-field-tokens-8.png)

1. Insira um valor padrão e clique em **Insert**.

   ![](assets/program-member-custom-field-tokens-9.png)

1. Clique em **Salvar**.

   ![](assets/program-member-custom-field-tokens-10.png)

**SMS**

1. Selecione o SMS desejado e clique em **Editar Rascunho**.

   ![](assets/program-member-custom-field-tokens-11.png)

1. Clique no botão **`{{ Token`**.

   ![](assets/program-member-custom-field-tokens-12.png)

1. Localize e selecione o Token de campo personalizado do membro do programa desejado. Insira um valor padrão e clique em Insert.

   ![](assets/program-member-custom-field-tokens-13.png)

1. Clique no menu suspenso Ações de SMS e selecione **Aprovar e fechar**.

   ![](assets/program-member-custom-field-tokens-14.png)

**Notificações por push**

1. Selecione a notificação por push desejada e clique em **Editar Rascunho**.

   ![](assets/program-member-custom-field-tokens-15.png)

1. Clique em **Notificações por push**.

   ![](assets/program-member-custom-field-tokens-16.png)

1. Clique na mensagem no editor e no botão `{{` para obter o seletor de token.

   ![](assets/program-member-custom-field-tokens-17.png)

1. Localize e selecione o Token de campo personalizado do membro do programa desejado. Insira um valor padrão e clique em **Insert**.

   ![](assets/program-member-custom-field-tokens-18.png)

1. Clique em **Finish** para salvar e sair (ou **Next** para revisar primeiro).

   ![](assets/program-member-custom-field-tokens-19.png)

>[!NOTE]
>
>Se o Campo Personalizado do Membro do Programa para um Membro do programa não tiver valor, o token será substituído pelo valor padrão se tiver sido fornecido.

## Usando tokens de campo personalizados de membro do programa em campanhas {#using-program-member-custom-field-tokens-in-campaigns}

Tokens de campo personalizado de membro do programa podem ser usados em:

* Criar tarefa
* Criar tarefa na Microsoft
* Momentos interessantes
* Alterar ações de fluxo do valor de dados
* Webhooks
