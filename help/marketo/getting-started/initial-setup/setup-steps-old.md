---
unique-page-id: 2949469
description: Etapas de configuração - Documentos do Marketo - Documentação do produto
title: Etapas de configuração
hide: true
hidefromtoc: true
exl-id: ef6b7311-55ca-4384-a24c-714eae89a57d
feature: Getting Started
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '2087'
ht-degree: 1%

---

# Etapas de configuração {#setup-steps}

**Bem-vindo ao Adobe Marketo Engage!**

Antes de mergulhar no uso do Marketo, há algumas etapas que você precisa concluir.

Essas etapas incluem:

* Alguma configuração básica de conta
* Adição de uma marca aos URLs da sua página de aterrissagem e links de email para melhorar a confiança e a capacidade de entrega
* Sincronizando seu CRM
* Adicionar código de rastreamento ao site corporativo

>[!NOTE]
>
>Você só precisará fazer essas etapas se sua empresa for **nova no Marketo**. Caso contrário, a configuração pode já ter sido feita.

Algumas etapas exigem a ajuda da sua equipe de TI.

>[!TIP]
>
>Se você [imprimir esta lista de verificação](/help/marketo/getting-started/initial-setup/setup-checklist.md){target="_blank"}, poderá desmarcá-los ao concluí-los.

## Fazer logon e criar usuários adicionais do Marketo {#log-in-and-create-additional-marketo-users}

>[!IMPORTANT]
>
>Se sua assinatura do Marketo foi criada em/após 31 de julho de 2023 ou já foi migrada para o [Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}, as etapas para adicionar um usuário descritas abaixo não se aplicam a você. Em vez disso, consulte [este artigo](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}.

Faça logon no Marketo [aqui](https://app.marketo.com/){target="_blank"} usando as credenciais recebidas por email.

![](assets/setup-steps-1.png)

Parabéns! Agora você está no Marketo e pode começar a explorar. Convite seus colegas da equipe de marketing para se juntarem a você. Você pode fazer isso adicionando novos usuários.

Vá para a área **[!UICONTROL Administrador]**.

>[!TIP]
>
>Enquanto estiver aqui, você pode clicar em **[!UICONTROL Minha conta]** para alterar as configurações de conta e local, bem como definir um novo nome de assinatura.

![](assets/setup-steps-2.png)

>[!NOTE]
>
>**Permissões de administrador necessárias**

Clique em **[!UICONTROL Usuários e funções]**.

![](assets/setup-steps-3.png)

Clique em **[!UICONTROL Convidar novo usuário]**.

![](assets/setup-steps-4.png)

Preencha o endereço de email do colega, nome e sobrenome. _A definição de uma data de expiração de acesso é opcional_. Clique em **[!UICONTROL Avançar]**.

![](assets/setup-steps-5.png)

>[!TIP]
>
>Uma data de expiração é ótima para participantes externos ou consultores de curto prazo que precisam apenas de acesso à Marketo por um curto período.

>[!NOTE]
>
>Quando a data de expiração chegar, o usuário receberá uma notificação de expiração e a conta será bloqueada.

Selecione uma função e clique em **[!UICONTROL Avançar]**. Usuários padrão têm acesso a todas as áreas, exceto Admin.

![](assets/setup-steps-6.png)

>[!NOTE]
>
>Além das cinco funções integradas, você também pode criar funções personalizadas. Saiba mais sobre [Gerenciamento de funções e permissões de usuário](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"}.

Fique à vontade para ajustar o texto do convite. Clique em **Enviar**.

![](assets/setup-steps-7.png)

O novo usuário agora está listado na guia **[!UICONTROL Usuários]** e deve receber um email com um link para criar uma senha e um logon. Próxima etapa!

![](assets/setup-steps-8.png)

## Configurar os contatos de suporte autorizados {#set-up-your-authorized-support-contacts}

Talvez você tenha recebido um email do Suporte da Marketo informando que é o administrador do Suporte ao cliente da Marketo da sua empresa. Em caso afirmativo, você pode configurar **contatos de suporte autorizados** para sua equipe. Somente contatos de suporte autorizados podem entrar em contato diretamente com o Suporte ao Cliente da Marketo através do [Portal de Suporte da Marketo](https://support.marketo.com){target="_blank"}.

>[!NOTE]
>
>O número de contatos de suporte que você pode criar é determinado pelo pacote que você adquiriu. Esse limite é especificado em seu email no Suporte da Marketo.

Os documentos do Contato de suporte autorizado foram movidos para a Comunidade da Marketo. Consulte [este artigo](https://nation.marketo.com/t5/Knowledgebase/Managing-Authorized-Support-Contacts/ta-p/254341){target="_blank"}.

>[!NOTE]
>
>Somente as pessoas que fizeram logon na Comunidade da Marketo aparecem na lista. Se não conseguir encontrar a pessoa, primeiro faça logon na Comunidade.

## Personalizar os URLs da sua landing page com um CNAME {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>Você é cliente do Launch Pack? Você pode ignorar esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial.

>[!NOTE]
>
>**Permissões de administrador necessárias**

Escolha um CNAME para suas landing pages. Alguns exemplos:

    * **ir**.[DomínioDaEmpresa].com
    * **www2**.[DomínioDaEmpresa].com
    * **lp**.[DomínioDaEmpresa].com

>[!TIP]
>
>Mantenha curto! URLs mais curtos são mais fáceis de lembrar. Sugerimos &quot;go&quot; como o domínio.

A primeira parte (em negrito) é o `[LandingPageCNAME]`. Você vai precisar na Etapa 5.

Para recuperar a Munchkin ID que você substituirá pela sua página de aterrissagem CNAME, vá para a área de Administrador.

![](assets/setup-steps-9.png)

Clique em **Minha conta**.

![](assets/setup-steps-10.png)

Copie a [!UICONTROL Cadeia de caracteres da conta] das configurações da página de aterrissagem.

![](assets/setup-steps-11.png)

Este é o `[Munchkin ID]`. Salve. Você precisará fornecê-lo à TI na Etapa 5.

Defina as configurações de domínio para que as páginas de aterrissagem usem o domínio de sua empresa em vez do da Marketo (onde estão hospedadas).

## Garantir a capacidade de entrega de e-mails {#ensure-email-deliverability}

>[!NOTE]
>
>Você é cliente do Launch Pack? Você pode ignorar esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial.

Há várias medidas que você pode tomar para garantir que os emails cheguem ao maior número de pessoas possível.

* **Crie uma marca nos links de rastreamento**. Você pode escolher um CNAME para usar seu próprio domínio (em vez do Marketo) nos links incluídos em emails do Marketo. Isso reforça a marca do seu domínio e aumenta a confiança e a capacidade de entrega dos seus recipients.
* **Adicione o Marketo incluir na lista de permissões ao seu arquivo de pesquisa de email corporativo.** É uma prática recomendada enviar emails de teste para suas contas de teste antes de enviar emails para pessoas reais. Incluir na lista de permissões Com o ➡ Marketo, você pode impedir que esses emails de teste sejam bloqueados ou sinalizados como spam.
* **Configurar SPF e DKIM.** Essas tecnologias garantem aos recipients que os emails do Marketo não são spam. Para ajudar a impedir que os filtros de spam dos destinatários rejeitem seus emails do Marketo, siga estas etapas para [Configurar um SPF e um DKIM para sua capacidade de entrega de email](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **Configure um registro MX para o seu domínio.** Um registro MX permite que você receba emails do domínio do qual você está enviando emails para processar respostas e respostas automáticas. Se estiver enviando do domínio corporativo, provavelmente você já tem essa configuração. Caso contrário, geralmente é possível configurar o para mapear para o registro MX do domínio corporativo.
* **Configurações Recomendadas para o Endereço do Remetente.** Você deve usar um domínio de email válido, existente e em funcionamento no Endereço do remetente em todas as campanhas de email. Pode ser útil configurar um subdomínio do domínio corporativo em vez de enviar a partir desse domínio. Isso garantirá que os problemas no fluxo de correio corporativo não afetem o fluxo de correio da Marketo e vice-versa. Além disso, o envio de emails de `something@nonexistentdomain.com` fará com que emails sejam filtrados ou bloqueados. Qualquer domínio usado no endereço &quot;De&quot; do remetente deve ter uma conta postmaster@ e abuse@ válida e funcional.

Se você estiver usando os aplicativos Google para hospedar emails corporativos, não será possível criar emails de abuso@ ou postmaster@ no seu domínio. Para contornar isso, você precisa criar grupos chamados &quot;abuso&quot; e &quot;postmaster&quot;. Os usuários membros desses grupos receberão emails enviados para esses endereços (por exemplo, postmaster@domain.com). Instruções detalhadas para a criação de grupos podem ser encontradas [aqui](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

Escolha um CNAME para links de rastreamento de email (escolha um que seja _diferente_ do CNAME da página de aterrissagem que você escolheu na Etapa 3). Alguns exemplos:

* go2[DomínioDaEmpresa].com
* em.[DomínioDaEmpresa].com
* uau.[DomínioDaEmpresa].com

A primeira parte é o rastreamento de email CNAME, `[EmailTrackingCNAME]`. Você precisará fornecê-lo à TI na Etapa 5.

>[!CAUTION]
>
>Os CNAMEs de email e de páginas iniciais devem ser diferentes. Além disso, evite CNAMEs como &quot;track&quot; ou &quot;link&quot;. Geralmente é sinalizado como spam

Para encontrar o link de rastreamento do Marketo, vá para a área **[!UICONTROL Administrador]**.

![](assets/setup-steps-12.png)

Clique em **[!UICONTROL Email]**.

![](assets/setup-steps-13.png)

Copie o [!UICONTROL Link de Acompanhamento] das configurações de email.

O [!UICONTROL Link de Rastreamento] está no formato: `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

Este é o seu `[MktoTrackingLink]`. Salve. Você precisará fornecê-lo à TI na Etapa 5.

Colete domínios &quot;From&quot;. Faça uma lista de todos os domínios &quot;From&quot; (como em `[Sender]@[FromDomain].com`) que você planeja usar para enviar emails do Marketo. Para a maioria, há apenas um.

Por exemplo, &#39;marketo.com,&#39; &#39;info.marketo.com,&#39;. Estes são `[FromDomain1]`,`[FromDomain2]`, etc. Salve-os. Você precisará fornecê-las à TI na Etapa 5.

Agora você tem todas as informações necessárias para enviar sua solicitação ao departamento de TI.

## Peça à TI para configurar protocolos {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Você é cliente do Launch Pack? Você pode ignorar esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial.

Depois de coletar todas as informações necessárias, você estará pronto para enviar uma solicitação para a TI. Você pode usar o texto abaixo como um modelo, substituindo o texto em negrito com suas próprias informações.

[Incluir um link para este artigo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md).

Cole esse texto no email e substitua os espaços reservados em negrito:

>[!NOTE]
>
>Consulte as Etapas 3 e 4 acima para determinar o texto para substituir os espaços reservados. Lembre-se de que `[LandingPageCNAME]` e `[EmailTrackingCNAME]` devem ser diferentes.

`----------------------------------------------`

Prezado excelente administrador de TI,

Agora, nossa Equipe de marketing está usando a plataforma Marketo para se comunicar com nosso pessoal. Para garantir uma excelente capacidade de delivery de email, precisamos fazer as seguintes alterações:

`1)` Para suas páginas de aterrissagem, adicione uma Entrada de DNS (CNAME) para **[LandingPageCNAME]**.**[CompanyDomain]**.com, apontando para **[Munchkin ID]**.mktoweb.com.

`2)` Para os links de rastreamento no email, adicione uma Entrada DNS (CNAME) para **[EmailTrackingCNAME]**.**[CompanyDomain]**.com, indicando **[MktoTrackingLink]**.

`3)` Incluir na lista de permissões Marketo.

    * Se usarmos endereços IP em nossa Inclui na lista de permissões por email, adicione os IPs listados abaixo:
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
>Entre em contato com o Suporte da Marketo incluir na lista de permissões se desejar obter uma lista abreviada de IPs para resolver problemas específicos de seu ambiente.

    * Se nosso sistema antisspam usa Domínios From, adicione estes:

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` Precisamos configurar o SPF e o DKIM para que a Marketo esteja autorizada a enviar emails assinados em nosso nome.

`a.` Para configurar o SPF, adicione a seguinte linha às suas entradas de DNS:

IN TXT **[Do Domínio]**: v=spf1 mx ip4:**[IP(s) Corporativo(s)]**
<br/>incluir: mktomail.com ~all

Se já tivermos um registro SPF existente em nossa entrada DNS, basta adicionar o seguinte a ele:

include:mktomail.com

`[`Substituir **Do Domínio** pelo Email do Domínio (ex: company.com) e **CorpIP** pelo endereço IP do servidor de email corporativo (ex: 255.255.255.255).  Se você for enviar emails de vários domínios por meio do Marketo, peça à sua equipe de TI para adicionar essa linha para cada domínio (em uma linha).`]`

`b.` Para o DKIM, crie Registros de Recursos de DNS para cada domínio que gostaríamos de configurar. Abaixo estão os Registros do host e Valores TXT para cada domínio que estaremos assinando:

**`[DKIMDomain1]`**: O Registro do Host é **`[HostRecord1]`** e o Valor TXT é **[TXTValue1]**.

**`[DKIMDomain2]`**: o Registro do Host é **`[HostRecord2]`** e o Valor TXT é **`[TXTValue2]`**.

`[`Copie o **HostRecord** e o **TXTValue** para cada **DKIMDomain** configurado após seguir as [instruções aqui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). Não se esqueça de verificar cada domínio em **Admin > Email > DKIM** depois que sua equipe de TI concluir esta etapa.`]`

`5)` Precisamos garantir que haja um registro MX válido para nossos domínios FROM **[FromDomain1]**, **[FromDomain2]** etc. Você pode confirmar? Caso contrário, configure o para mapear para nosso registro MX de domínio corporativo. Isso garantirá que possamos processar respostas/respostas automáticas para nossas correspondências do Marketo.

Avise-me quando você concluir essas etapas, para que eu possa concluir o processo de configuração com o Marketo.

Obrigado! Você é o melhor!

Amor,

**`[Your Name]`**

`----------------------------------------------`

Envie o e-mail para TI. Sabemos que pode levar algum tempo para que a TI conclua essas tarefas. Você pode continuar na Etapa 7, mas lembre-se de retornar a Etapa 6 para concluir a configuração do Marketo.

## Conclua a configuração do Marketo após a conclusão da TI {#complete-your-marketo-setup-after-it-finishes}

Depois que a equipe de TI concluir as tarefas, siga estas etapas para adicionar CNAMEs de página de aterrissagem e email e para ativar a assinatura do DKIM.

Vá para a área **[!UICONTROL Administrador]** para Adicionar sua página de aterrissagem CNAME

![](assets/setup-steps-15.png)

Selecione Landing Pages e clique em **[!UICONTROL Editar]** na área [!UICONTROL Configurações].

![](assets/setup-steps-16.png)

Insira o novo nome de domínio no campo **[!UICONTROL Nome do Domínio para Páginas de Aterrissagem]**. Isso deve estar no formato:

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

No campo de página **[!UICONTROL Fallback]**, insira a URL para a qual você deseja que as pessoas acessem se uma página de aterrissagem não estiver disponível. Você pode usar a home page de sua empresa se não tiver uma página de fallback. No campo **[!UICONTROL Página inicial]**, digite o site da empresa.

![](assets/setup-steps-18.png)

Na área [!UICONTROL Administrador], selecione **[!UICONTROL Email]** para adicionar seu CNAME de email

![](assets/setup-steps-19.png)

Role para baixo até [!UICONTROL Domínios de marca]. Selecione seu domínio e clique em **[!UICONTROL Editar]**.

![](assets/setup-steps-20.png)

No campo Domain, insira o domínio de rastreamento de email. Isso deve estar no formato:

`[EmailTrackingCNAME].[CompanyDomain].com`. Clique em **[!UICONTROL Salvar]**.

![](assets/setup-steps-21.png)

## Integrar seu CRM {#integrate-your-crm}

Esta é provavelmente a etapa mais emocionante da sua configuração - é hora de encher o Marketo com todos esses leads e contatos que você armazenou em seu CRM!

Escolha uma das opções a seguir, dependendo do CRM que sua empresa usa.

    * [Integrar o Marketo com [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [Integrar o Marketo com [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>Você precisa da assistência do administrador de CRM da sua empresa para concluir essas etapas.

## Adicionar código de rastreamento ao seu site {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Você é cliente do [!DNL Launch Pack]? Você pode ignorar esta etapa. O consultor fornecerá a você [!DNL Munchkin] instruções de código em seu documento de instruções de configuração de TI.

O Marketo tem JavaScript de rastreamento personalizado (chamado [!DNL Munchkin]) que você pode usar para rastrear atividades de pessoas em qualquer página da Web. O [!DNL Munchkin] é necessário para integrar seu site à Marketo. Siga estas etapas para [Adicionar [!DNL Munchkin] Código de Rastreamento ao seu Site](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>É necessária experiência com o HTML para adicionar o código de rastreamento.

## Expectativas de desempenho {#performance-expectations}

O que você pode esperar do Marketo em termos de desempenho? Pode variar, dependendo do tamanho e da complexidade de suas campanhas de marketing. Mas você pode esperar níveis de desempenho iguais aos descritos na coluna &quot;Padrão&quot; em várias tabelas encontradas na [Descrição do produto Marketo Engage](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. As colunas &quot;Desempenho&quot; e &quot;Desempenho Adicional&quot; referem-se a pacotes de camada de desempenho que fornecem [níveis de desempenho mais altos](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

Todas as etapas de configuração foram concluídas. A única coisa que resta é mergulhar e usar o Marketo!
