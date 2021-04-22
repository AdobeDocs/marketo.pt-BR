---
unique-page-id: 2949469
description: Etapas de configuração - Documentação do Marketo - Documentação do produto
title: Etapas de configuração
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '2004'
ht-degree: 0%

---

# Etapas de configuração {#setup-steps}

**Bem-vindo ao Marketo!**

Antes de mergulhar no Marketo, você precisa concluir algumas etapas.

Essas etapas incluem:

* configuração básica da conta
* marcar seus URLs de página inicial e links de email para melhorar a confiança e a capacidade de entrega
* sincronização do seu CRM
* adicionar código de rastreamento ao site corporativo

>[!NOTE]
>
>Você só precisará fazer essas etapas se sua empresa for **new to Marketo**. Caso contrário, a configuração pode já estar concluída.

Algumas etapas exigem a ajuda da sua equipe de TI.

>[!TIP]
>
>Se você [imprimir essa lista de verificação](/help/marketo/getting-started/setup-steps/setup-checklist.md), poderá desmarcar os itens ao concluí-los.

## Faça logon e crie usuários adicionais do Marketo {#log-in-and-create-additional-marketo-users}

1. Faça logon no Marketo [aqui](https://app.marketo.com/) usando as credenciais recebidas por email.

   ![](assets/new-login-screen-hand.jpg)

Parabéns! Agora você está no Marketo e pode começar a explorar. Talvez você queira convidar seus colegas da equipe de marketing para se associar a você. Você pode fazer isso adicionando novos usuários.

Vá para a área **Admin**.

>[!TIP]
>
>Enquanto estiver aqui, clique em **Minha Conta** para alterar suas configurações de conta e local, bem como definir um novo nome de assinatura.

![](assets/admin.png)

>[!NOTE]
>
>**Permissões de administrador necessárias**

Clique em **Usuários e funções**.

![](assets/image2015-1-6-13-3a14-3a43.png)

Clique em **Convidar novo usuário**.

![](assets/image2015-1-6-13-3a14-3a6.png)

Preencha o endereço de e-mail do seu colega, nome e sobrenome.

![](assets/image2016-5-24-10-3a11-3a12.png)

Opcionalmente, insira um motivo para o convite e uma data de expiração de acesso, usando o seletor de calendário. Clique em **OK**.

![](assets/image2016-5-24-10-3a13-3a9.png)

Clique em **Next**.

![](assets/image2016-5-24-10-3a14-3a9.png)

>[!TIP]
>
>Uma data de expiração é ideal para consultores ou partes interessadas externas de curto prazo, que precisam de acesso à Marketo apenas por um curto período.

>[!NOTE]
>
>Quando a data de expiração chegar, o usuário receberá uma notificação de expiração e a conta será bloqueada.

Selecione uma função e clique em **Next**. Os usuários padrão têm acesso a todas as áreas, exceto Administrador.

![](assets/image2016-5-24-10-3a14-3a51.png)

>[!NOTE]
>
>Além das cinco funções integradas, você também pode criar funções personalizadas. Saiba mais sobre como [Gerenciar funções de usuário e permissões](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).

Você pode ajustar o texto do convite. Clique em **Enviar**.

![](assets/image2016-5-24-10-3a15-3a52.png)

O novo usuário agora está listado na guia Usuários e deve receber um email com um link para criar uma senha e um logon. Próximo passo!

![](assets/image2016-5-24-10-3a23-3a10.png)

## Configurar seus contatos de suporte autorizados {#set-up-your-authorized-support-contacts}

Você pode ter recebido um email do Suporte da Marketo informando que é o administrador do Suporte ao cliente da Marketo para sua empresa. Nesse caso, você pode configurar **contatos de suporte autorizados** para sua equipe. Somente contatos de suporte autorizados podem entrar em contato com o Suporte ao Cliente da Marketo diretamente por meio do [Portal de suporte da Marketo](https://support.marketo.com).

>[!NOTE]
>
>O número de contatos de suporte que podem ser criados é determinado pelo pacote que você comprou. Esse limite é especificado no email do Suporte da Marketo.

Os documentos de contato de suporte autorizado foram transferidos para a Comunidade da Marketo. Consulte [este artigo](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341).

>[!NOTE]
>
>Somente as pessoas que fizeram logon na Comunidade do Marketo são exibidas na lista. Se não conseguir encontrar a pessoa, verifique se ela fez logon na Comunidade primeiro.

## Personalize seus URLs de página inicial com um CNAME {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>Você é um cliente do Launch Pack? Ignore esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial.

>[!NOTE]
>
>**Permissões de administrador necessárias**

Escolha um CNAME para suas landing pages. Alguns exemplos:

    * **go**.[CompanyDomain].com
    * **www2**.[CompanyDomain].com
    * **lp**.[CompanyDomain].com

>[!TIP]
>
>Mantenha curto! URLs mais curtos são mais fáceis de lembrar. Sugerimos &quot;ir&quot; como domínio.

A primeira parte (em negrito) é o `[LandingPageCNAME]`. Você precisará dele na Etapa 5.

Para recuperar a sequência de caracteres da conta que será substituída pelo CNAME da landing page, vá para a área de administração.

![](assets/admin.png)

Clique em **Páginas de aterrissagem**.

![](assets/image2015-1-6-13-3a52-3a6.png)

Copie a Cadeia de caracteres da conta das configurações da página de aterrissagem.

![](assets/image2015-1-6-13-3a53-3a19.png)

Este é o `[AccountString]`. Salve-o. Você precisará fornecê-lo à TI na Etapa 5.

Defina as configurações de domínio para que as páginas de aterrissagem usem o domínio de sua empresa em vez do da Marketo (onde estão hospedadas).

## Garanta a capacidade de entrega de email {#ensure-email-deliverability}

>[!NOTE]
>
>Você é um cliente do Launch Pack? Ignore esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial.

Há várias medidas que você pode tomar para garantir que os emails alcancem o maior número possível de suas pessoas.

    1. **Marca seus links de rastreamento**. Você pode escolher um CNAME para usar seu próprio domínio (em vez do Marketo) nos links incluídos nos emails do Marketo. Isso reforça sua marca de domínio e aumenta a confiança e a capacidade de entrega com seus recipients.
    1. **Adicione o Marketo à  de lista de permissões de email corporativo.** É uma prática recomendada comum enviar emails de teste para suas contas de teste antes de enviar emails para pessoas reais. Ao incluir na lista de permissões o Marketo, você pode impedir que esses emails de teste sejam bloqueados ou sinalizados como spam.
    1. **Configurar SPF e DKIM.** Essas tecnologias garantem aos recipients que seus emails do Marketo não são spam. Para ajudar a impedir que os filtros de spam dos recipients rejeitem seus emails do Marketo, siga estas etapas para [Configurar um SPF e DKIM para sua capacidade de delivery de email](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
    1. **Configure um registro MX para seu domínio.** Um registro MX permite receber emails para o domínio do qual você está enviando emails para processar respostas e responder automaticamente. Se você estiver enviando do seu domínio corporativo, provavelmente já terá isso configurado. Caso contrário, você geralmente pode configurar o para mapear para o registro MX do domínio corporativo.
    1. **Configurações recomendadas para o endereço de origem.** Você deve usar um domínio de email válido, existente e em funcionamento no Endereço de origem em todas as campanhas de email. Pode ser útil configurar um subdomínio de seu domínio corporativo em vez de enviar de seu domínio corporativo. Isso garantirá que os problemas da sua transmissão de e-mail corporativa não afetem sua transmissão de e-mail da Marketo e vice-versa. Além disso, o envio de emails de something@nonexistentdomain.com fará com que o email seja filtrado ou bloqueado. Qualquer domínio usado no endereço de origem do remetente deve ter uma conta postmaster@ e abuso@ válida e em funcionamento.
    Se estiver usando os aplicativos do Google para hospedar seu email corporativo, você não poderá criar emails de abuso@ ou postmaster@ em seu domínio. Para contornar isso, você precisa criar grupos chamados de &quot;abuso&quot; e &quot;postmaster&quot;. Os usuários que são membros desses grupos receberão emails enviados para esses endereços (por exemplo, postmaster@domain.com). Instruções detalhadas para criar grupos podem ser encontradas [aqui](https://support.google.com/a/answer/33343#adminconsole).

Escolha um CNAME para links de rastreamento de email (escolha um que seja _diferente_ da página de aterrissagem CNAME que você escolheu na Etapa 3). Alguns exemplos:

    * go2.[CompanyDomain].com
    * em.[CompanyDomain].com
    * wow.[CompanyDomain].com

A primeira parte é o CNAME de rastreamento de email, `[EmailTrackingCNAME]`. Você precisará fornecê-lo à TI na Etapa 5.

>[!CAUTION]
>
>Os CNAMEs de email e de página de aterrissagem devem ser diferentes. Além disso, evite CNAMEs como &quot;rastreamento&quot; ou &quot;link&quot;. Geralmente é sinalizado como spam

Para encontrar o link de rastreamento do Marketo, vá para a área **Admin**.

![](assets/admin.png)

Clique em **Email**.

![](assets/image2015-1-6-13-3a55-3a32.png)

Copie o Link de rastreamento das configurações de email.

O Link de rastreamento está no formato: `mkto-[a-z][4 digits].com`.

![](assets/email-tracking-link-hand.jpg)

Este é seu `[MktoTrackingLink]`. Salve-o. Você precisará fornecê-lo à TI na Etapa 5.

Colete domínios &quot;De&quot;. Faça uma lista de todos os domínios &quot;De&quot; (como em, `[Sender]@[FromDomain].com`) que você planeja usar para enviar emails do Marketo. Para a maioria, há apenas um.

Por exemplo, &#39;marketo.com&#39;, &#39;info.marketo.com,&#39;. Estes são `[FromDomain1]`,`[FromDomain2]`, etc. Salve-os. Você precisará fornecê-las à TI na Etapa 5.

Agora você tem todas as informações necessárias para enviar sua solicitação para TI!

## Solicitar que a TI configure protocolos {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Você é um cliente do Launch Pack? Ignore esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial.

Depois de coletar todas as informações necessárias, você está pronto para enviar uma solicitação para a TI. Você pode usar o texto abaixo como um modelo, substituindo o texto em negrito por suas próprias informações.

[Inclua um link para este artigo](/help/marketo/getting-started/setup-steps/configure-protocols-for-marketo.md).

Cole esse texto no email e substitua os espaços reservados em negrito:

>[!NOTE]
>
>Consulte as Etapas 3 e 4 acima para determinar o texto que substituirá os espaços reservados. Lembre-se de que `[LandingPageCNAME]` e `[EmailTrackingCNAME]` devem ser diferentes.

`---------------------------------------------`

Prezado Administrador de TI Incrível,

Nossa equipe de marketing agora está usando a plataforma Marketo para se comunicar com nossas pessoas. Para garantir um excelente delivery de email, precisamos fazer as seguintes alterações:

`1)` Para nossas páginas de aterrissagem, adicione uma Entrada de DNS (CNAME) para  **[LandingPageCNAME]**.**[CompanyDomain]**.com, apontando para  **[AccountString]**.mktoweb.com.

`2)` Para nossos links de rastreamento no email, adicione uma Entrada de DNS (CNAME) para  **[EmailTrackingCNAME]**.**[CompanyDomain]**.com, apontando para  **[MktoTrackingLink]**.

`3)` lista de permissões Marketo.

    * Se usarmos endereços IP na  de Lista de permissões de email, adicione os IPs listados abaixo: 
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    103.237.104.0/22
    
    94.236.119.0/26

OBSERVAÇÃO: Entre em contato com o Suporte da Marketo se desejar uma lista abreviada de IPs para lista de permissões específicos ao seu ambiente.

    * Se seu sistema antisspam usar From domains, adicione:

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Precisamos configurar o SPF e o DKIM para que o Marketo esteja autorizado a enviar emails assinados em nosso nome.

`a.` Para configurar o SPF, adicione a seguinte linha às nossas entradas DNS:

NO TXT **[Do Domínio]**:  v=spf1 mx ip4:**[IP(s) corporativo(s)]**
<br/>incluir: mktomail.com ~all

Se já houver um registro SPF existente em nossa entrada DNS, basta adicionar o seguinte a ele:

include:mktomail.com

`[`Substitua  **do** domínio por seu email do domínio (por exemplo: company.com) e  **** CorpIPcom o endereço IP do seu servidor de email corporativo (por exemplo: 255.255.255.255).  Se você estiver enviando emails de vários domínios por meio do Marketo, sua equipe de TI deve adicionar essa linha para cada domínio (em uma linha).`]`

`b.` Para DKIM, crie Registros de Recursos de DNS para cada domínio que gostaríamos de configurar. Abaixo estão os Registros de host e os Valores TXT para cada domínio que iremos assinar:

**`[DKIMDomain1]`**: O Registro do Host é  **`[HostRecord1]`** e o Valor TXT é  **[TXTValue1]**.

**`[DKIMDomain2]`**: O registro do host é  **`[HostRecord2]`** e o valor TXT é  **`[TXTValue2]`**.

`[`Copie o  **** HostRecordand  **** TXTValuepara cada  **** DKIMDomainen que você configurou depois de seguir as  [instruções aqui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). Não se esqueça de verificar cada domínio em **Admin > Email > DKIM** depois que sua equipe de TI concluir esta etapa.`]`

`5)` Precisamos garantir que haja um registro MX válido para nossos domínios FROM  **[FromDomain1]**,  **[FromDomain2]** etc. Você pode confirmar? Caso contrário, configure para mapear para nosso registro MX de domínio corporativo. Isso garantirá que possamos processar respostas/autorrespondedores para nossas correspondências do Marketo.

Informe quando você concluiu essas etapas, para que eu possa concluir o processo de configuração com o Marketo.

Atenciosamente! Você é o melhor!

Amor,

**`[Your Name]`**

`---------------------------------------------`

Envie o email para TI. Entendemos que pode levar algum tempo para que a TI conclua essas tarefas. Você pode continuar com a Etapa 7, mas lembre-se de que deve retornar a Etapa 6 para concluir a configuração do Marketo.

## Conclua a configuração do Marketo após a conclusão da TI {#complete-your-marketo-setup-after-it-finishes}

Depois que a TI concluir suas tarefas, siga estas etapas para adicionar sua página de aterrissagem e enviar emails para CNAMEs e ativar a assinatura DKIM.

Vá para a área **Admin** para Adicionar seu CNAME de página inicial

![](assets/admin.png)

Selecione Páginas de aterrissagem e clique em **Editar** na área Configurações.

![](assets/image2015-1-6-13-3a59-3a15.png)

Insira seu novo nome de domínio no campo Nome do domínio para páginas de aterrissagem. Isso deve estar na forma:

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/image2015-1-6-14-3a3-3a6.png)

No campo Fallback page , insira o URL para o qual você deseja que as pessoas acessem se uma landing page não estiver disponível. Você pode usar a página inicial da empresa se não tiver uma página de fallback. No campo Página inicial , insira o site da empresa.

![](assets/image2015-1-6-14-3a2-3a46.png)

Na área Admin , selecione Email para adicionar seu CNAME de email

![](assets/image2015-1-6-14-3a5-3a3.png)

Role para baixo e clique em **Editar**.

![](assets/edit-branding-domain.png)

No campo Domínio , insira o domínio de rastreamento de email. Isso deve estar na forma:

`[EmailTrackingCNAME].[CompanyDomain].com`. Clique em **Salvar**.

![](assets/new-branding-domain-9-1.png)

## Integre seu CRM {#integrate-your-crm}

Esta é provavelmente a etapa mais excitante de sua configuração - é hora de preencher o Marketo com todos esses leads e contatos que você armazenou em seu CRM!

Escolha entre as opções a seguir, dependendo do CRM que sua empresa usa.

    * [Integre o Marketo com o Salesforce.com](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [Integre o Marketo com o Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>Você precisa da assistência do administrador de CRM de sua empresa para concluir essas etapas.

## Adicionar código de rastreamento ao seu site {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Você é um cliente do Launch Pack? Ignore esta etapa. Seu consultor fornecerá instruções de código do Munchkin no documento de instruções de configuração de TI.

A Marketo tem o JavaScript de rastreamento personalizado (chamado Munchkin) que você pode usar para rastrear atividades de pessoas em qualquer página da Web. O Munchkin é necessário para integrar seu site ao Marketo. Siga estas etapas para [Adicionar código de rastreamento do Munchkin ao seu site](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).

>[!NOTE]
>
>Experiência com HTML necessária para adicionar o código de rastreamento.

Todas as etapas de configuração foram concluídas. Só resta mergulhar e usar o Marketo!
