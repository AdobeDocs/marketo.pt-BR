---
unique-page-id: 2949469
description: Etapas de configuração - Documentação do Marketo - Documentação do produto
title: Etapas de configuração
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
source-git-commit: 3f0ccfcb22e0b84c6d1e60b750af955cb442bd36
workflow-type: tm+mt
source-wordcount: '2002'
ht-degree: 0%

---

# Etapas de configuração {#setup-steps}

**Bem-vindo ao Marketo Engage!**

Antes de mergulhar no Marketo, você precisa concluir algumas etapas.

Essas etapas incluem:

* Algumas configurações básicas da conta
* Criar a marca dos URLs de página inicial e links de email para melhorar a confiança e a capacidade de entrega
* Sincronização do seu CRM
* Adicionar código de rastreamento ao site corporativo

>[!NOTE]
>
>Você só precisará fazer essas etapas se sua empresa estiver **novo no Marketo**. Caso contrário, a configuração pode já estar concluída.

Algumas etapas exigem a ajuda da sua equipe de TI.

>[!TIP]
>
>Se você [imprimir esta lista de verificação](/help/marketo/getting-started/setup-steps/setup-checklist.md){target=&quot;_blank&quot;}, você pode desmarcar os itens ao concluí-los.

## Fazer logon e criar usuários adicionais do Marketo {#log-in-and-create-additional-marketo-users}

1. Faça logon no Marketo [here](https://app.marketo.com/){target=&quot;_blank&quot;} usando as credenciais recebidas por email.

   ![](assets/setup-steps-1.png)

Parabéns! Agora você está no Marketo e pode começar a explorar. Talvez você queira convidar seus colegas da equipe de marketing para se associar a você. Você pode fazer isso adicionando novos usuários.

Vá para o **Administrador** área.

>[!TIP]
>
>Enquanto estiver aqui, clique em **Minha conta** para alterar as configurações da conta e do local, bem como definir um novo nome de assinatura.

![](assets/setup-steps-2.png)

>[!NOTE]
>
>**Permissões de administrador necessárias**

Clique em **Usuários e funções**.

![](assets/setup-steps-3.png)

Clique em **Convidar novo usuário**.

![](assets/setup-steps-4.png)

Preencha o endereço de e-mail do seu colega, nome e sobrenome. _A definição de uma data de expiração de acesso é opcional_. Clique em **Próximo**.

![](assets/setup-steps-5.png)

>[!TIP]
>
>Uma data de expiração é ideal para parceiros externos ou consultores de curto prazo que precisam apenas de acesso Marketo por um curto período.

>[!NOTE]
>
>Quando a data de expiração chegar, o usuário receberá uma notificação de expiração e a conta será bloqueada.

Selecione uma função e clique em **Próximo**. Os usuários padrão têm acesso a todas as áreas, exceto Administrador.

![](assets/setup-steps-6.png)

>[!NOTE]
>
>Além das cinco funções integradas, você também pode criar funções personalizadas. Saiba mais sobre [Gerenciando funções e permissões do usuário](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target=&quot;_blank&quot;}.

Você pode ajustar o texto do convite. Clique em **Enviar**.

![](assets/setup-steps-7.png)

O novo usuário agora está listado na guia Usuários e deve receber um email com um link para criar uma senha e um logon. Próximo passo!

![](assets/setup-steps-8.png)

## Configurar seus contatos de suporte autorizados {#set-up-your-authorized-support-contacts}

Você pode ter recebido um email do Suporte da Marketo informando que é o administrador do Suporte ao cliente da Marketo para sua empresa. Nesse caso, você pode configurar **contatos de suporte autorizados** para a sua equipe. Somente contatos de suporte autorizados podem entrar em contato com o Suporte ao cliente da Marketo diretamente por meio do [Portal de suporte Marketo](https://support.marketo.com){target=&quot;_blank&quot;}.

>[!NOTE]
>
>O número de contatos de suporte que podem ser criados é determinado pelo pacote que você comprou. Esse limite é especificado no email do Suporte da Marketo.

Os documentos de contato de suporte autorizado foram transferidos para a Comunidade da Marketo. Consulte [este artigo](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target=&quot;_blank&quot;}.

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

A primeira parte (a negrito) é a `[LandingPageCNAME]`. Você precisará disso na Etapa 5.

Para recuperar a sequência de caracteres da conta que será substituída pelo CNAME da landing page, vá para a área de administração.

![](assets/setup-steps-9.png)

Clique em **Páginas de aterrissagem**.

![](assets/setup-steps-10.png)

Copie a Cadeia de caracteres da conta das configurações da página de aterrissagem.

![](assets/setup-steps-11.png)

Este é o `[AccountString]`. Salve-o. Você precisará fornecê-lo à TI na Etapa 5.

Defina as configurações de domínio para que as páginas de aterrissagem usem o domínio de sua empresa em vez do da Marketo (onde estão hospedadas).

## Garantir a entregabilidade por email {#ensure-email-deliverability}

>[!NOTE]
>
>Você é um cliente do Launch Pack? Ignore esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial.

Há várias medidas que você pode tomar para garantir que os emails alcancem o maior número possível de suas pessoas.

* **Criar uma marca nos links de rastreamento**. Você pode escolher um CNAME para usar seu próprio domínio (em vez do Marketo) nos links incluídos nos emails do Marketo. Isso reforça sua marca de domínio e aumenta a confiança e a capacidade de entrega com seus recipients.
* **Adicione o Marketo à sua  de lista de permissões de email corporativo.** É uma prática recomendada comum enviar emails de teste para suas contas de teste antes de enviar emails para pessoas reais. Ao incluir na lista de permissões o Marketo, você pode impedir que esses emails de teste sejam bloqueados ou sinalizados como spam.
* **Configure o SPF e o DKIM.** Essas tecnologias garantem aos recipients que seus emails do Marketo não são spam. Para ajudar a impedir que os filtros de spam dos recipients rejeitem seus emails do Marketo, siga estas etapas para [Configurar um SPF e DKIM para sua capacidade de delivery de email](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **Configure um registro MX para seu domínio.** Um registro MX permite receber emails para o domínio do qual você está enviando emails para processar respostas e responder automaticamente. Se você estiver enviando do seu domínio corporativo, provavelmente já terá isso configurado. Caso contrário, você geralmente pode configurar o para mapear para o registro MX do domínio corporativo.
* **Configurações recomendadas para o endereço de origem.** Você deve usar um domínio de email válido, existente e em funcionamento no Endereço de origem em todas as campanhas de email. Pode ser útil configurar um subdomínio de seu domínio corporativo em vez de enviar de seu domínio corporativo. Isso garantirá que os problemas da sua transmissão de e-mail corporativa não afetem sua transmissão de e-mail da Marketo e vice-versa. Além disso, enviar correio de `something@nonexistentdomain.com` O fará com que o email seja filtrado ou bloqueado. Qualquer domínio usado no endereço de origem do remetente deve ter uma conta postmaster@ e abuso@ válida e em funcionamento.

Se estiver usando os aplicativos Google para hospedar seu email corporativo, você não poderá criar emails de abuso@ ou postmaster@ em seu domínio. Para contornar isso, você precisa criar grupos chamados de &quot;abuso&quot; e &quot;postmaster&quot;. Os usuários que são membros desses grupos receberão emails enviados para esses endereços (por exemplo, postmaster@domain.com). Instruções detalhadas sobre a criação de grupos podem ser encontradas [here](https://support.google.com/a/answer/33343#adminconsole){target=&quot;_blank&quot;}.

Escolha um CNAME para links de rastreamento de email (escolha um que seja _different_ na página de aterrissagem CNAME, você escolheu na Etapa 3). Alguns exemplos:

* vá2.[CompanyDomain].com
* em.[CompanyDomain].com
* uau.[CompanyDomain].com

A primeira parte é o CNAME de rastreamento de email, `[EmailTrackingCNAME]`. Você precisará fornecê-lo à TI na Etapa 5.

>[!CAUTION]
>
>Os CNAMEs de email e de página de aterrissagem devem ser diferentes. Além disso, evite CNAMEs como &quot;rastreamento&quot; ou &quot;link&quot;. Geralmente é sinalizado como spam

Para encontrar o link de rastreamento do Marketo, acesse **Administrador** área.

![](assets/setup-steps-12.png)

Clique em **Email**.

![](assets/setup-steps-13.png)

Copie o Link de rastreamento das configurações de email.

O Link de rastreamento está no formato: `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

Este é o seu `[MktoTrackingLink]`. Salve-o. Você precisará fornecê-lo à TI na Etapa 5.

Colete domínios &quot;De&quot;. Faça uma lista de todos os domínios &quot;De&quot; (como em, `[Sender]@[FromDomain].com`) que você planeja usar para enviar emails do Marketo. Para a maioria, há apenas um.

Por exemplo, &#39;marketo.com&#39;, &#39;info.marketo.com,&#39;. Estes `[FromDomain1]`,`[FromDomain2]`, etc. Salve-os. Você precisará fornecê-las à TI na Etapa 5.

Agora você tem todas as informações necessárias para enviar sua solicitação para TI!

## Pedir à TI para configurar protocolos {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Você é um cliente do Launch Pack? Ignore esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial.

Depois de coletar todas as informações necessárias, você está pronto para enviar uma solicitação para a TI. Você pode usar o texto abaixo como um modelo, substituindo o texto em negrito por suas próprias informações.

[Incluir um link para este artigo](/help/marketo/getting-started/setup-steps/configure-protocols-for-marketo.md).

Cole esse texto no email e substitua os espaços reservados em negrito:

>[!NOTE]
>
>Consulte as Etapas 3 e 4 acima para determinar o texto que substituirá os espaços reservados. Lembre-se `[LandingPageCNAME]` e `[EmailTrackingCNAME]` deve ser diferente.

`---------------------------------------------`

Prezado Administrador de TI Incrível,

Nossa equipe de marketing agora está usando a plataforma Marketo para se comunicar com nossas pessoas. Para garantir um excelente delivery de email, precisamos fazer as seguintes alterações:

`1)` Em nossas páginas de aterrissagem, adicione uma Entrada de DNS (CNAME) para **[LandingPageCNAME]**.**[CompanyDomain]**.com, apontando para **[AccountString]**.mktoweb.com.

`2)` Para nossos links de rastreamento no email, adicione uma Entrada de DNS (CNAME) para **[EmailTrackingCNAME]**.**[CompanyDomain]**.com, apontando para **[MktoTrackingLink]**.

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

>[!NOTE]
>
>Entre em contato com o Suporte da Marketo se desejar uma lista abreviada de IPs para lista de permissões específicos ao seu ambiente.

    * Se seu sistema antisspam usar From domains, adicione:

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Precisamos configurar o SPF e o DKIM para que o Marketo esteja autorizado a enviar emails assinados em nosso nome.

`a.` Para configurar o SPF, adicione a seguinte linha às nossas entradas DNS:

NO TXT **[Do Domínio]**: v=spf1 mx ip4:**[IP(s) corporativo(s)]**
<br/>incluem: mktomail.com ~all

Se já houver um registro SPF existente em nossa entrada DNS, basta adicionar o seguinte a ele:

include:mktomail.com

`[`Substituir **Do Domínio** com seu Email do domínio (por exemplo: company.com) e **CorpIP** com o endereço IP do servidor de email corporativo (por exemplo: 255.255.255.255).  Caso envie emails de vários domínios por meio do Marketo, sua equipe de TI deve adicionar essa linha para cada domínio (em uma linha).`]`

`b.` Para DKIM, crie Registros de Recursos de DNS para cada domínio que gostaríamos de configurar. Abaixo estão os Registros de host e os Valores TXT para cada domínio que iremos assinar:

**`[DKIMDomain1]`**: O Registro do Host é **`[HostRecord1]`** e o valor TXT é **[TXTValue1]**.

**`[DKIMDomain2]`**: O Registro do Host é **`[HostRecord2]`** e o valor TXT é **`[TXTValue2]`**.

`[`Copie o **HostRecord** e **TXTValue** para cada **DKIMDomain** você configurou depois de seguir o [instruções aqui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). Não se esqueça de verificar cada domínio em **Admin > Email > DKIM** depois que sua equipe de TI concluir esta etapa.`]`

`5)` Precisamos garantir que haja um registro MX válido para nossos domínios FROM **[FromDomain1]**, **[FromDomain2]**, etc. Você pode confirmar? Caso contrário, configure para mapear para nosso registro MX de domínio corporativo. Isso garantirá que possamos processar respostas/autorrespondedores para nossas correspondências do Marketo.

Informe quando você concluiu essas etapas, para que eu possa concluir o processo de configuração com o Marketo.

Atenciosamente! Você é o melhor!

Amor,

**`[Your Name]`**

`---------------------------------------------`

Envie o email para TI. Entendemos que pode levar algum tempo para que a TI conclua essas tarefas. Você pode continuar com a Etapa 7, mas lembre-se de que deve retornar a Etapa 6 para concluir a configuração do Marketo.

## Conclua a configuração do Marketo após a conclusão da TI {#complete-your-marketo-setup-after-it-finishes}

Depois que a TI concluir suas tarefas, siga estas etapas para adicionar sua página de aterrissagem e enviar emails para CNAMEs e ativar a assinatura DKIM.

Vá para o **Administrador** área para adicionar o CNAME da página inicial

![](assets/setup-steps-15.png)

Selecione Páginas de aterrissagem e clique em **Editar** na área Configurações .

![](assets/setup-steps-16.png)

Insira seu novo nome de domínio no campo Nome do domínio para páginas de aterrissagem. Isso deve estar na forma:

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

No campo Fallback page , insira o URL para o qual você deseja que as pessoas acessem se uma landing page não estiver disponível. Você pode usar a página inicial da empresa se não tiver uma página de fallback. No campo Página inicial , insira o site da empresa.

![](assets/setup-steps-18.png)

Na área Admin , selecione Email para adicionar seu CNAME de email

![](assets/setup-steps-19.png)

Role para baixo até Domínios de marca. Selecione seu domínio e clique em **Editar**.

![](assets/setup-steps-20.png)

No campo Domínio , insira o domínio de rastreamento de email. Isso deve estar na forma:

`[EmailTrackingCNAME].[CompanyDomain].com`. Clique em **Salvar**.

![](assets/setup-steps-21.png)

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

A Marketo tem o JavaScript de rastreamento personalizado (chamado Munchkin) que você pode usar para rastrear atividades de pessoas em qualquer página da Web. O Munchkin é necessário para integrar seu site ao Marketo. Siga estas etapas para [Adicionar o código de rastreamento do Munchkin ao seu site](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target=&quot;_blank&quot;}.

>[!NOTE]
>
>Experiência com HTML necessária para adicionar o código de rastreamento.

Todas as etapas de configuração foram concluídas. A única coisa que resta é mergulhar e usar o Marketo!
