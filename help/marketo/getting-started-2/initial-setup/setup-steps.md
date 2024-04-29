---
description: Etapas De Configuração - Documentação Do Marketo - Documentação Do Produto
title: Etapas de configuração
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: f9bf2082968737277b3c976659802992f975ec9a
workflow-type: tm+mt
source-wordcount: '1696'
ht-degree: 0%

---

# Etapas de configuração {#setup-steps}

**ATUALIZAÇÃO DESTE ARTIGO**

Bem-vindo ao Marketo Engage!

Antes de mergulhar no uso do Marketo, há algumas etapas que você precisa concluir.

Essas etapas incluem:

* Alguma configuração básica de conta
* Adição de uma marca aos URLs da sua página de aterrissagem e links de email para melhorar a confiança e a capacidade de entrega
* Sincronizando seu CRM
* Adicionar código de rastreamento ao site corporativo

>[!NOTE]
>
>Você só precisará fazer essas etapas se a empresa estiver **novo no Marketo**. Caso contrário, a configuração pode já ter sido feita.

Algumas etapas exigem a ajuda da sua equipe de TI.

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

A primeira parte (a negrito) é a seguinte: `[LandingPageCNAME]`. Você vai precisar na Etapa 5.

Para recuperar a ID do Munchkin que você substituirá pela sua página de aterrissagem CNAME, vá para a área de Administração.

![](assets/setup-steps-9.png)

Clique em **Minha conta**.

![](assets/setup-steps-10.png)

Copie o [!UICONTROL String de conta] das configurações da página de aterrissagem.

![](assets/setup-steps-11.png)

Este é o `[Munchkin ID]`. Salve. Você precisará fornecê-lo à TI na Etapa 5.

Defina as configurações de domínio para que as páginas de aterrissagem usem o domínio de sua empresa em vez do da Marketo (onde estão hospedadas).

## Garantir a capacidade de entrega de e-mails {#ensure-email-deliverability}

>[!NOTE]
>
>Você é cliente do Launch Pack? Você pode ignorar esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial.

Há várias medidas que você pode tomar para garantir que os emails cheguem ao maior número de pessoas possível.

* **Marque seus links de rastreamento**. Você pode escolher um CNAME para usar seu próprio domínio (em vez do Marketo) nos links incluídos em emails do Marketo. Isso reforça a marca do seu domínio e aumenta a confiança e a capacidade de entrega dos seus recipients.
* **Adicione o Marketo ao seu incluo na lista de permissões de e-mail corporativo.** É uma prática recomendada enviar emails de teste para suas contas de teste antes de enviar emails para pessoas reais. Incluir na lista de permissões Com o ➡ Marketo, você pode impedir que esses emails de teste sejam bloqueados ou sinalizados como spam.
* **Configure o SPF e o DKIM.** Essas tecnologias garantem aos recipients que os emails do Marketo não são spam. Para ajudar a impedir que os filtros de spam dos recipients rejeitem seus emails do Marketo, siga estas etapas para [Configurar um SPF e um DKIM para a capacidade de entrega de emails](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **Configure um registro MX para seu domínio.** Um registro MX permite receber emails do domínio do qual você está enviando email para processar respostas e respostas automáticas. Se estiver enviando do domínio corporativo, provavelmente você já tem essa configuração. Caso contrário, geralmente é possível configurar o para mapear para o registro MX do domínio corporativo.
* **Configurações recomendadas para o endereço do remetente.** Você deve usar um domínio de email válido, existente e funcional no Endereço do remetente em todas as campanhas de email. Pode ser útil configurar um subdomínio do domínio corporativo em vez de enviar a partir desse domínio. Isso garantirá que os problemas no fluxo de correio corporativo não afetem o fluxo de correio da Marketo e vice-versa. Além disso, o envio de e-mails de `something@nonexistentdomain.com` fará com que o email seja filtrado ou bloqueado. Qualquer domínio usado no endereço &quot;De&quot; do remetente deve ter uma conta postmaster@ e abuse@ válida e funcional.

Se você estiver usando os aplicativos Google para hospedar emails corporativos, não será possível criar emails de abuso@ ou postmaster@ no seu domínio. Para contornar isso, você precisa criar grupos chamados &quot;abuso&quot; e &quot;postmaster&quot;. Os usuários membros desses grupos receberão emails enviados para esses endereços (por exemplo, postmaster@domain.com). As instruções detalhadas para criar grupos podem ser encontradas [aqui](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

Escolha um CNAME para links de rastreamento de email (escolha um que seja _diferente_ na landing page CNAME que você escolheu na Etapa 3). Alguns exemplos:

* go2[Domínio da empresa].com
* em.[Domínio da empresa].com
* uau.[Domínio da empresa].com

A primeira parte é o rastreamento de email CNAME, `[EmailTrackingCNAME]`. Você precisará fornecê-lo à TI na Etapa 5.

>[!CAUTION]
>
>Os CNAMEs de email e de páginas iniciais devem ser diferentes. Além disso, evite CNAMEs como &quot;track&quot; ou &quot;link&quot;. Geralmente é sinalizado como spam

Para encontrar o link de rastreamento do Marketo, acesse o **[!UICONTROL Admin]** área.

![](assets/setup-steps-12.png)

Clique em **[!UICONTROL E-mail]**.

![](assets/setup-steps-13.png)

Copie o [!UICONTROL Link de rastreamento] das configurações de email.

A variável [!UICONTROL Link de rastreamento] está no formato: `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-14.png)

Este é o seu `[MktoTrackingLink]`. Salve. Você precisará fornecê-lo à TI na Etapa 5.

Colete domínios &quot;From&quot;. Faça uma lista de todos os domínios &quot;From&quot; (como em, `[Sender]@[FromDomain].com`) que planeja usar para enviar emails do Marketo. Para a maioria, há apenas um.

Por exemplo, &#39;marketo.com,&#39; &#39;info.marketo.com,&#39;. Estes são `[FromDomain1]`,`[FromDomain2]`, etc. Salve-os. Você precisará fornecê-las à TI na Etapa 5.

Agora você tem todas as informações necessárias para enviar sua solicitação ao departamento de TI.

## Peça à TI para configurar protocolos {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Você é cliente do Launch Pack? Você pode ignorar esta etapa. O consultor fornecerá um documento de instruções de configuração de TI durante a chamada inicial.

Depois de coletar todas as informações necessárias, você estará pronto para enviar uma solicitação para a TI. Você pode usar o texto abaixo como um modelo, substituindo o texto em negrito com suas próprias informações.

[Incluir um link para este artigo](/help/marketo/getting-started/setup/configure-protocols-for-marketo.md).

Cole esse texto no email e substitua os espaços reservados em negrito:

>[!NOTE]
>
>Consulte as Etapas 3 e 4 acima para determinar o texto para substituir os espaços reservados. Lembre-se `[LandingPageCNAME]` e `[EmailTrackingCNAME]` deve ser diferente.

`----------------------------------------------`

Prezado excelente administrador de TI,

Agora, nossa Equipe de marketing está usando a plataforma Marketo para se comunicar com nosso pessoal. Para garantir uma excelente capacidade de delivery de email, precisamos fazer as seguintes alterações:

`1)` Para nossas páginas de aterrissagem, adicione uma Entrada de DNS (CNAME) para **[LandingPageCNAME]**.**[Domínio da empresa]**.com, apontando para **[ID do Munchkin]**.mktoweb.com.

`2)` Para os links de rastreamento no email, adicione uma Entrada de DNS (CNAME) para **[EmailTrackingCNAME]**.**[Domínio da empresa]**.com, apontando para **[MktoTrackingLink]**.

`3)` Incluir na lista de permissões navegar no Marketo.

    * Se usarmos endereços IP em nosso arquivo de Inclui na lista de permissões de email, adicione os IPs listados abaixo:
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

`4)` Precisamos configurar o SPF e o DKIM para que a Marketo seja autorizada a enviar emails assinados em nosso nome.

`a.` Para configurar o SPF, adicione a seguinte linha às suas entradas de DNS:

EM TXT **[Do Domínio]**: v=spf1 mx ip4:**[IP(s) corporativo(s)]**
<br/>incluir: mktomail.com ~all

Se já tivermos um registro SPF existente em nossa entrada DNS, basta adicionar o seguinte a ele:

incluir:mktomail.com

`[`Substituir **Do Domínio** com seu Email do domínio (por exemplo: company.com) e **CorpIP** com o endereço IP do seu servidor de email corporativo (ex: 255.255.255.255).  Se você for enviar emails de vários domínios por meio do Marketo, a equipe de TI deve adicionar essa linha para cada domínio (em uma linha).`]`

`b.` Para DKIM, crie Registros de Recursos DNS para cada domínio que gostaríamos de configurar. Abaixo estão os Registros do host e Valores TXT para cada domínio que estaremos assinando:

**`[DKIMDomain1]`**: o registro do host é **`[HostRecord1]`** e o Valor de TXT for **[ValorDaTVt1]**.

**`[DKIMDomain2]`**: o registro do host é **`[HostRecord2]`** e o Valor de TXT for **`[TXTValue2]`**.

`[`Copie o **HostRecord** e **TXTValue** para cada **DKIMDomain** você configurou o após seguir o [instruções aqui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). Não se esqueça de verificar cada domínio no **Admin > Email > DKIM** depois que sua equipe de TI concluir esta etapa.`]`

`5)` Precisamos garantir que haja um registro MX válido para nossos domínios FROM **[DoDomínio1]**, **[DoDomínio2]**, etc. Você pode confirmar? Caso contrário, configure o para mapear para nosso registro MX de domínio corporativo. Isso garantirá que possamos processar respostas/respostas automáticas para nossas correspondências do Marketo.

Avise-me quando você concluir essas etapas, para que eu possa concluir o processo de configuração com o Marketo.

Obrigado! Você é o melhor!

Amor,

**`[Your Name]`**

`----------------------------------------------`

Envie o e-mail para TI. Sabemos que pode levar algum tempo para que a TI conclua essas tarefas. Você pode continuar na Etapa 7, mas lembre-se de retornar a Etapa 6 para concluir a configuração do Marketo.

## Conclua a configuração do Marketo após a conclusão da TI {#complete-your-marketo-setup-after-it-finishes}

Depois que o departamento de TI concluir as tarefas, siga estas etapas para adicionar uma landing page e CNAMEs de email e ativar a assinatura DKIM.

Vá para a **[!UICONTROL Admin]** área para adicionar sua página de aterrissagem CNAME

![](assets/setup-steps-15.png)

Selecione Landing Pages e clique em **[!UICONTROL Editar]** no [!UICONTROL Configurações] área.

![](assets/setup-steps-16.png)

Insira o novo nome de domínio no campo **[!UICONTROL Nome de domínio para páginas de aterrissagem]**. Isso deve estar no formato:

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-17.png)

No **[!UICONTROL Fallback]** , insira o URL para o qual você deseja que as pessoas acessem se uma landing page não estiver disponível. Você pode usar a home page de sua empresa se não tiver uma página de fallback. No **[!UICONTROL Página inicial]** insira o site da empresa.

![](assets/setup-steps-18.png)

No [!UICONTROL Admin] , selecione **[!UICONTROL E-mail]** para adicionar seu CNAME de email

![](assets/setup-steps-19.png)

Role para baixo até [!UICONTROL Domínios de marca]. Selecione o domínio e clique em **[!UICONTROL Editar]**.

![](assets/setup-steps-20.png)

No campo Domain, insira o domínio de rastreamento de email. Isso deve estar no formato:

`[EmailTrackingCNAME].[CompanyDomain].com`. Clique em **[!UICONTROL Salvar]**.

![](assets/setup-steps-21.png)

## Integrar seu CRM {#integrate-your-crm}

Esta é provavelmente a etapa mais emocionante da sua configuração - é hora de encher o Marketo com todos esses leads e contatos que você armazenou em seu CRM!

Escolha uma das opções a seguir, dependendo do CRM que sua empresa usa.

    * [Integrar o Marketo com o [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
    * [Integrar o Marketo com o [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

>[!NOTE]
>
>Você precisa da assistência do administrador de CRM da sua empresa para concluir essas etapas.

## Adicionar código de rastreamento ao seu site {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Você é um [!DNL Launch Pack] cliente? Você pode ignorar esta etapa. Seu consultor fornecerá a você [!DNL Munchkin] instruções de código em seu documento de instruções de configuração de TI.

O Marketo tem um rastreamento personalizado de JavaScript (chamado [!DNL Munchkin]) que você pode usar para rastrear atividades de pessoas em qualquer página da Web. [!DNL Munchkin] O é necessário para integrar o site à Marketo. Siga estas etapas para [Adicionar [!DNL Munchkin] Código de rastreamento para seu site](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>Experiência com HTML necessária para adicionar o código de rastreamento.

## Expectativas de desempenho {#performance-expectations}

O que você pode esperar do Marketo em termos de desempenho? Pode variar, dependendo do tamanho e da complexidade de suas campanhas de marketing. Mas você pode esperar níveis de desempenho iguais aos descritos na coluna &quot;Padrão&quot; em várias das tabelas encontradas no [Descrição do produto Marketo Engage](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. The "Performance" and "Performance Plus" columns refer to performance tier packages that provide [higher performance levels](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

Todas as etapas de configuração foram concluídas. A única coisa que resta é mergulhar e usar o Marketo!
