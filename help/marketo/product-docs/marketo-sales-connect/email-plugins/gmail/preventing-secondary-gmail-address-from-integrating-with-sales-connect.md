---
unique-page-id: 14352546
description: Impedir que o endereço Gmail secundário seja integrado ao Sales Connect - Documentação do Marketo - Documentação do produto
title: Impedir que o endereço secundário do Gmail seja integrado ao Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 2%

---

# Impedindo a Integração do Endereço Gmail Secundário com o [!DNL Sales Connect] {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integração com o Gmail interrompida (por que meu Gmail pessoal está enviando emails) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

O motivo mais comum para uma conexão Gmail interrompida é uma integração acidental com a conta pessoal de um usuário. Isso pode acontecer quando um usuário clica em &quot;Conectar&quot; ou quando tenta enviar um email de sua conta pessoal. Pode ser muito tentador fazer isso porque a opção existirá ao acessar sua conta do Gmail na mesma instância do [!DNL Chrome] que seu email comercial.

## Por que o [!DNL Sales Connect] tenta sequer integrar com o meu Gmail pessoal? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

[!DNL Sales Connect] integra-se ao Gmail por meio de uma extensão instalada no navegador [!DNL Chrome]. Sempre que a extensão detectar uma instância do Gmail aberta, ela oferecerá uma opção para se integrar a ela. Para evitar uma integração com sua conta pessoal do Gmail, recomendamos uma destas três coisas...

Entrar Como Outro [!DNL Chrome]Usuário (Recomendado)

Clique [neste link](https://support.google.com/chrome/answer/2364824?hl=en) para ler como criar outro [!DNL Chrome]Perfil.

**Vantagens**: entrar como outro usuário abrirá uma nova instância de [!DNL Chrome]. Esta instância é uma janela totalmente nova do [!DNL Chrome], e nenhuma das extensões antigas existirá nesta. Ele também mantém cookies para que você não precise entrar no Gmail todas as vezes.

**Contras**: deve ter duas janelas de [!DNL Chrome]abertas.

Usar Outro Navegador

**Vantagens:** usar outro navegador da Internet (IE ou Firefox) que não tenha a extensão instalada impedirá que isso aconteça.

**Contras**: usar vários navegadores pode ser incômodo.

Usar Uma Janela Incógnito

**Vantagens:** uma janela incógnita é como abrir uma versão desnuda de [!DNL Chrome]. Isso significa que nenhuma de suas extensões estará instalada e o [!DNL Sales Connect] não estará lá para se conectar.

**Contras**: você terá que entrar no Gmail toda vez que iniciar o dia e novamente se fechar a janela acidentalmente.
