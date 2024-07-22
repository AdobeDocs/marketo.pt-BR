---
unique-page-id: 14352546
description: Impedir que o endereço Gmail secundário seja integrado ao Sales Connect - Documentação do Marketo - Documentação do produto
title: Impedindo que o Endereço Gmail Secundário seja Integrado ao Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Impedindo que o Endereço Gmail Secundário seja Integrado ao Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integração com o Gmail interrompida (por que meu Gmail pessoal está enviando emails) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

O motivo mais comum para uma conexão Gmail interrompida é uma integração acidental com a conta pessoal de um usuário. Isso pode acontecer quando um usuário clica em &quot;Conectar&quot; ou quando tenta enviar um email de sua conta pessoal. Isso pode ser muito tentador, pois a opção existirá ao acessar sua conta do Gmail na mesma instância do Chrome que seu email comercial.

## Por que o Sales Connect tenta sequer integrar com meu Gmail pessoal? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

O Sales Connect integra-se ao Gmail por meio de uma extensão instalada no navegador Chrome. Sempre que a extensão detectar uma instância do Gmail aberta, ela oferecerá uma opção para se integrar a ela. Para evitar uma integração com sua conta pessoal do Gmail, recomendamos uma destas três coisas...

Fazer Logon Como Outro Usuário Do Chrome (Recomendado)

Clique em [este link](https://support.google.com/chrome/answer/2364824?hl=en) para ler como criar outro Perfil do Chrome.

**Vantagens**: entrar como outro usuário abrirá uma nova instância do Chrome. Essa instância é uma janela totalmente nova do Chrome e nenhuma das extensões antigas existirá nessa. Ele também mantém cookies para que você não precise entrar no Gmail todas as vezes.

**Contras**: deve ter duas janelas do Chrome abertas.

Usar Outro Navegador

**Vantagens:** usar outro navegador da Internet (IE ou Firefox) que não tenha a extensão instalada impedirá que isso aconteça.

**Contras**: usar vários navegadores pode ser incômodo.

Usar Uma Janela Incógnito

**Vantagens:** uma janela incógnita é como abrir uma versão desnuda do Chrome. Isso significa que nenhuma de suas extensões estará instalada e o Sales Connect não estará lá para se conectar.

**Contras**: você terá que entrar no Gmail toda vez que iniciar o dia e novamente se fechar a janela acidentalmente.
