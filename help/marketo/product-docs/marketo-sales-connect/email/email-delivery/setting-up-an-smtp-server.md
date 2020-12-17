---
unique-page-id: 14746594
description: Configuração de um servidor SMTP - Documentos do Marketing - Documentação do produto
title: Configuração de um servidor SMTP
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---


# Configuração de um Servidor SMTP {#setting-up-an-smtp-server}

## Visão geral {#overview}

**O que é um servidor SMTP?**

**** Simple  **** Mail  **** Transfer  **** Protocol, este é o servidor responsável pelo envio do correio de saída. Ao enviar um email do seu cliente de email, você está usando o mesmo serviço para entregar seu email.

**Por que quero configurar meu servidor SMTP com o Sales Connect?**

Ele permite que você utilize a reputação do domínio e a capacidade de entrega da sua empresa, e que não tenha que depender de outros. Nossos Servidores MSC padrão são parte de um pool IP compartilhado, o que significa enviar de uma reputação compartilhada. Recomendamos que sua equipe configure seu próprio canal de delivery com o Sales Connect.

**Como o Sales Connect envia com meu servidor SMTP?**

Seguindo [estas etapas](http://docs.marketo.com/x/ZgPh).

![](assets/1.png)

`<pre><em>SMTP Server Setup Page in Sales Connect</em><br> </pre>` **Preciso configurar alguma coisa no meu cliente de e-mail?**

Quanto a um canal delivery, não. Depois que você tiver instalado nosso suplemento, o Sales Connect aproveitará o mesmo canal de delivery que você configurou para enviar emails.

## Obtendo as credenciais SMTP {#getting-the-smtp-credentials}

**Como obtenho minhas credenciais SMTP?**

Entre em contato com sua equipe de TI para descobrir que canal de delivery sua empresa está usando para enviar emails e como obter acesso às suas credenciais SMTP. Dependendo de como seu servidor está configurado, você pode ter alguns valores personalizados para o Nome do servidor SMTP ou Porta do servidor. Se você não tiver uma equipe de TI dedicada, entre em contato com seu provedor de e-mail.

**Quais são minhas opções se minha empresa usar o Office365?**

Prós

* Fácil de configurar
* Qualquer usuário com uma conta do Office365 terá acesso a este servidor SMTP

Cons

* A limitação pode ocorrer
* Cada usuário deve configurar
* A alteração da senha O365 de um usuário resultará em uma conexão interrompida

Se estiver usando o Office365 ou o Exchange Online, você pode se conectar ao servidor SMTP usando um conjunto padrão de credenciais. Lembre-se de que o Office365 não é um serviço de delivery de email em massa, embora isso funcione bem para o envio de emails únicos. Ao enviar emails em massa, o Office 365 pode limitar seus emails, o que pode resultar em delivery com falha. Para saber mais sobre este artigo da Microsoft sobre [como configurar o envio de cliente SMTP](http://support.office.com/en-us/article/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-365-69f58e99-c550-4274-ad18-c805d654b4c4).
`<blockquote>  <p>“You can only send from one email address unless your device can store login credentials for multiple Office 365 mailboxes. Office 365 imposes a limit of 30 messages sent per minute, and a limit of 10,000 recipients per day.”</p> </blockquote>`\
Se você decidir usar o Office365 como canal de delivery, precisará digitar essas credenciais. As mesmas credenciais não podem ser usadas no grupo porque o Office365 usa o email e a senha do usuário para conexão.

Microsoft e envio em massa

[Clique ](http://technet.microsoft.com/en-us/library/exchange-online-limits.aspx#RecipientLimits) aqui para saber mais sobre envio em massa no Office365. 
`<blockquote>  <p>“Exchange Online customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.”</p> </blockquote>`\
**E se minha empresa usa o Gmail?**

Você não precisará obter quaisquer credenciais SMTP se sua equipe quiser usar o Gmail como seu canal delivery com o Sales Connect. O Sales Connect permite que os usuários tenham acesso ao canal do Gmail por meio de nossa integração OAuth. Os usuários podem habilitar isso integrando sua conta do Sales Connect ao Gmail.

![](assets/2.png)

**Posso compartilhar as mesmas credenciais SMTP com toda a minha equipe?**

Isso depende do canal do delivery que você está usando. Por exemplo, serviços como o Sparkpost permitem que as credenciais sejam baseadas em domínio, de modo que qualquer pessoa que envia com um domínio específico seja autenticada para enviar por esse servidor. Se esse for o caso, então sim, você pode compartilhar as credenciais com a equipe.

Se você estiver se conectando ao Office365, as credenciais serão baseadas em endereço de email. Isso significa que somente o endereço de email que estabeleceu a conexão será autenticado para enviar emails por meio desse canal de delivery, portanto, as credenciais devem ser compartilhadas **e não**.

![](assets/3.png)

