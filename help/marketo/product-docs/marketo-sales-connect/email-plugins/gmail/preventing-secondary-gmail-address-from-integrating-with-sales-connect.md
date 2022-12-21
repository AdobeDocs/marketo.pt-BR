---
unique-page-id: 14352546
description: Impedindo que o endereço Gmail secundário se integre ao Sales Connect - Documentos do Marketo - Documentação do produto
title: Impedindo que o endereço Gmail secundário se integre ao Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Impedindo que o endereço Gmail secundário se integre ao Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integração de Gmail quebrada (por que meu Gmail pessoal está enviando emails) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

O motivo mais comum para uma conexão Gmail quebrada é uma integração acidental com a conta pessoal de um usuário. Isso pode acontecer quando um usuário clica em &quot;Conectar&quot; ou tenta enviar um email de sua conta pessoal. Isso pode ser muito tentador, pois a opção existirá ao acessar sua conta Gmail na mesma instância do Chrome que seu email de trabalho.

## Por que o Sales Connect tenta mesmo se integrar com meu Gmail pessoal? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

O Sales Connect integra-se ao Gmail por meio de uma extensão instalada no navegador Chrome. Sempre que a extensão detecta uma instância do Gmail aberta, ela oferece uma opção de integração com ela. Para evitar uma integração com sua conta pessoal do Gmail, recomendamos uma das três coisas...

Fazer Logon Como Outro Usuário Do Chrome (Recomendado)

Clique em [este link](https://support.google.com/chrome/answer/2364824?hl=en) para ler como criar outro perfil do Chrome.

**Prós**: Fazer logon como outro usuário abrirá uma nova instância do Chrome. Essa instância é uma janela totalmente nova do Chrome e nenhuma de suas extensões antigas existirá nessa. Ele também mantém cookies para que você não tenha que entrar no seu Gmail todas as vezes.

**Desvantagens**: Deve ter duas janelas do Chrome abertas.

Usar Outro Navegador

**Vantagens:** Usar outro navegador da Internet (IE ou Firefox) que não tenha a extensão instalada impedirá que isso aconteça.

**Desvantagens**: Usar vários navegadores pode ser irritante.

Usar Uma Janela Incógnito

**Vantagens:** Uma janela incógnita é como abrir uma versão nua do Chrome. Isso significa que ele não terá nenhuma de suas extensões instaladas e o Sales Connect não estará lá para se conectar.

**Desvantagens**: Você terá que entrar no Gmail toda vez que iniciar seu dia e novamente se você fechar a janela acidentalmente.
