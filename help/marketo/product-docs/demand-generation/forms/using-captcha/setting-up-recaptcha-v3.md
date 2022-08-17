---
description: Configuração do reCAPTCHA v3 - Documentos do Marketo - Documentação do produto
title: Configuração do reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: 1803d6355747f4b6300509a3d361bf235dd56f44
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Configurando o reCAPTCHA {#setting-up-recaptcha}

Texto de introdução

## Configuração do reCAPTCHA v3 {#setting-up-recaptcha-v3}

Texto: Descrever a v3 - as etapas a seguir são executadas fora do Marketo Engage.

1. Ir para [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;} e clique no Admin Console v3.

1. Faça logon/se inscreva em uma conta da Google.

1. Clique no botão Create (sinal de +) para criar uma nova chave.

1. Crie um rótulo para identificar a chave que deve ser usada para o Marketo Engage.

1. Escolher tipo **reCAPTCHA v3**. No momento, o Marketo Engage não é compatível com o reCAPTCHA v2.

1. Adicione cada domínio que a assinatura do Marketo Engage usa. Domínios não definidos aqui retornarão erros em formulários em que reCAPTCHA está ativado.

   * 123-ABC-456.mktoweb.com
   * app-pod.marketo.com
   * qualquer domínio de landing page e alias configurado na assinatura

1. Defina um proprietário e um endereço de email adicional que deve receber alertas sobre esse serviço.

1. Aceite os Termos de Serviço do reCAPTCHA.

1. Clique em **Enviar**.

>[!NOTE]
>
>Mantenha a chave do site e a chave secreta acessíveis para a configuração do Marketo Engage.

## Configuração do CAPTCHA no Marketo Engage {#setting-up-captcha-in-marketo-engage}

1. No Marketo, clique em **Administrador** e selecione **CAPTCHA**.

PICC

1. Clique em **Editar** nas configurações CAPTCHA.

PICC

1. Clique no menu suspenso CAPTCHA e escolha reCAPTCHA v3.

PICC

1. Insira a chave secreta e a chave do site. Clique em **Salvar** quando concluído.

PICC
