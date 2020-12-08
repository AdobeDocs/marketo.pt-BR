---
unique-page-id: 14352546
description: Impedindo a integração do endereço de correio eletrônico secundário ao Sales Connect - Documentos do Marketing - Documentação do produto
title: Impedindo a integração do endereço de correio secundário ao Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# Impedindo a integração do endereço de correio secundário ao Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integração de Gmail Quebrada (por que meus e-mails pessoais do Gmail estão sendo enviados) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

O motivo mais comum para uma conexão Gmail quebrada é uma integração acidental com a conta pessoal do usuário. Isso pode acontecer quando um usuário clica em &quot;Connect&quot; ou tenta enviar um email de sua conta pessoal. Isso pode ser muito tentador, pois a opção existirá ao acessar sua conta do Gmail na mesma instância do Chrome que seu email de trabalho.

## Por que o Sales Connect tenta se integrar ao meu Gmail pessoal? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

O Sales Connect é integrado ao Gmail por meio de uma extensão instalada no navegador Chrome. Sempre que a extensão detecta uma instância do Gmail aberta, ela oferta uma opção para integrar com ela. Para evitar uma integração com sua conta pessoal do Gmail, recomendamos uma das três coisas...

Fazer Logon Como Outro Usuário Do Chrome (Recomendado)

Clique [neste link](http://support.google.com/chrome/answer/2364824?hl=en) para ler como criar outro Perfil do Chrome.

**Vantagens**: Fazer logon como outro usuário abrirá uma nova instância do Chrome. Esta instância é uma nova janela do Chrome, e nenhuma das suas extensões antigas existirá nesta. Ele também mantém cookies para que você não precise fazer logon no seu Gmail todas as vezes.

**Cons**: Deve ter duas janelas do Chrome abertas.

Usar outro navegador

**Vantagens:** Usar outro navegador da Internet (IE ou Firefox) que não tenha a extensão instalada impedirá que isso ocorra.

**Cons**: Usar vários navegadores pode ser irritante.

Usar Uma Janela Incognito

**Vantagens:** Uma janela incógnita é como abrir uma versão nua do Chrome. Ou seja, não terá nenhuma de suas extensões instaladas e o Sales Connect não estará lá para se conectar.

**Cons**: Você terá que entrar no Gmail toda vez que start seu dia, e novamente se você acidentalmente fechar a janela.
