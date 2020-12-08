---
unique-page-id: 11373011
description: Transição para o Editor de e-mail 2.0 - Documentos do Marketing - Documentação do produto
title: Transição para o Editor de email 2.0
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---


# Transição para o Editor de email 2.0 {#transitioning-to-email-editor}

A partir da versão [de 19 de](../../../../release-notes/2016/release-notes-spring-16.md)junho, todas as subscrições de marketing foram migradas para o Editor de e-mail 2.0. [Saiba mais](https://nation.marketo.com/docs/DOC-7038) sobre a desaprovação do Editor de email 1.0.

Os e-mails e modelos de e-mail na sua subscrição devem ter um número de versão. A versão pode ser encontrada na página de resumo do ativo.

![](assets/five-5.png)

Por padrão, todos os seus e-mails e modelos de e-mail existentes serão marcados como v1.0 se tiverem sido criados antes da versão do primeiro trimestre de 2016 ou após a versão quando o Editor de e-mail 2.0 estiver desativado. Com o Editor de email 2.0 ativado automaticamente, você verá o seguinte comportamento:

* Ao criar um novo email, o Seletor [de modelos de](email-template-picker-overview.md) email será exibido e você poderá escolher um modelo de email v2.0.
* Sempre que você criar ou editar um email com o Editor de email 2.0, o email resultante **sempre** será marcado como v2.0 (mesmo se você tiver usado um modelo de email v1.0).

Se sua subscrição tiver emails v1.0 antes da mudança para o Editor de email 2.0, você experimentará o seguinte comportamento com base no estado atual do ativo:

**Aprovado** - Clicar em &quot;Editar rascunho&quot; criará um rascunho v2.0 do email aprovado. Se você aprovar o rascunho v2.0, o estado aprovado do email se torna v2.0 e não há como reverter para v1.0.\
**Rascunho** - clicar em &quot;Editar rascunho&quot; marcará automaticamente esse rascunho como v2.0. Nesse ponto, não será possível descartar e reverter para v1.0 porque não há uma versão aprovada do ativo.\
**Aprovado com rascunho** - clicar em &quot;Editar rascunho&quot; marcará automaticamente esse rascunho como v2.0. Por isso, também não há como reverter o rascunho de volta para v1.0.

Se sua subscrição tiver modelos de e-mail v1.0 antes de mover para o Editor de e-mail 2.0, você experimentará o seguinte comportamento:

**Aprovado** - Clicar em &quot;Editar rascunho&quot; criará um rascunho v2.0 do modelo de email existente.\
**Rascunho** - clicar em &quot;Editar rascunho&quot; marcará automaticamente esse rascunho como v2.0. Nesse ponto, não seria possível descartar e reverter para v1.0 porque não há uma versão aprovada do ativo.\
**Aprovado com rascunho** - clicar em &quot;Editar rascunho&quot; marcará automaticamente esse rascunho como v2.0. Por isso, também não há como reverter o rascunho de volta para v1.0.

Se você aprovar um modelo de e-mail que era anterior à v1.0 (em qualquer um dos estados acima), você verá o seguinte comportamento:

Para emails v1.0 existentes que estavam usando o modelo (anteriormente v1.0):\
**Email** v1.0 aprovado - Um rascunho v2.0 será criado para este email, ainda usando o modelo v2.0 recém-aprovado. Ele também receberá quaisquer alterações de modelo.\
**Email** v1.0 de rascunho - o rascunho permanecerá v1.0 até que você clique em &quot;Editar rascunho&quot;. Depois disso, ele será automaticamente marcado como v2.0 e receberá quaisquer alterações no modelo.\
**Aprovado com email** Draft v1.0 - O rascunho permanecerá v1.0 até que você clique em &quot;Editar rascunho&quot;. Depois disso, ele será automaticamente marcado como v2.0 e receberá quaisquer alterações no modelo.

Para emails v2.0 existentes que estavam usando o modelo (anteriormente v1.0):\
**E-mail** v2.0 aprovado - Um rascunho v2.0 será criado para este e-mail, ainda &quot;usando&quot; o modelo recém-aprovado e receberá quaisquer alterações no modelo.\
**Email** v2.0 de rascunho - o rascunho permanecerá como está (v2.0) e receberá quaisquer alterações no modelo.\
**Aprovado com email** Draft v2.0 - O rascunho permanecerá como está (v2.0) e receberá quaisquer alterações de modelo.

>[!CAUTION]
>
>Se você aprovar o rascunho v2.0 de um modelo de email v1.0, o modelo se tornará v2.0. Não há **como** revertê-lo de volta para v1.0.

Observações

* Os emails aprovados **nunca** são alterados.

* Os modelos de e-mail aprovados **nunca** são alterados.

* Em alguns casos **raros** , um e-mail v1.0 não pode ser aberto no Editor de e-mail 2.0. Se isso ocorrer, descarte o rascunho e entre em contato com o suporte do Marketo.

>[!NOTE]
>
>**Artigos relacionados**
>
>* [Visão geral do Editor de email 2.0](email-editor-v2-0-overview.md)
>* [Sintaxe do modelo de email](email-template-syntax.md)

>



