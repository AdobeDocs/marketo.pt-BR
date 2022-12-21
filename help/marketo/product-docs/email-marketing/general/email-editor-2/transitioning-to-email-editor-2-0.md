---
unique-page-id: 11373011
description: Transição para o Editor de email 2.0 - Documentos do Marketo - Documentação do produto
title: Transição para o Editor de email 2.0
exl-id: eb9ec8cc-d6e8-4839-a4d9-608d2f264cbb
source-git-commit: 64ff6900a761b9df796a9a7f417cca1ddc628cce
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---

# Transição para o Editor de email 2.0 {#transitioning-to-email-editor}

A partir da versão de 19 de junho, todas as assinaturas do Marketo foram migradas para o Editor de email 2.0. [Saiba mais](https://nation.marketo.com/docs/DOC-7038) sobre a descontinuação do Editor de email 1.0.

Os emails e modelos de email na sua assinatura devem ter um número de versão. A versão pode ser encontrada na página de resumo do ativo.

![](assets/five-5.png)

Por padrão, todos os emails e modelos de email existentes serão marcados como v1.0 se tiverem sido criados antes da versão do primeiro trimestre de 2016 ou após a versão em que o Editor de email 2.0 estiver desativado. Com o Editor de email 2.0 agora ativado automaticamente, você verá o seguinte comportamento:

* Ao criar um novo email, a variável [Seletor de modelo de email](email-template-picker-overview.md) será exibido e você poderá escolher um template de email v2.0.
* Sempre que você criar ou editar um email com o Editor de email 2.0, o email resultante **always** ser marcado como v2.0 (mesmo se você usou um template de email v1.0).

Se sua assinatura tiver emails v1.0 antes da mudança para o Editor de email 2.0, você terá o seguinte comportamento com base no estado atual do ativo:

**Aprovado** - Clicar em &quot;Editar rascunho&quot; criará um rascunho v2.0 do email aprovado. Se você aprovar o rascunho v2.0, o estado aprovado do email se tornará v2.0 e não há como reverter para v1.0.\
**Rascunho** - Clicar em &quot;Editar rascunho&quot; marcará automaticamente esse rascunho como v2.0. Nesse momento, não será possível descartar e reverter para v1.0 porque não há uma versão aprovada do ativo.
**Aprovado com rascunho** - Clicar em &quot;Editar rascunho&quot; marcará automaticamente esse rascunho como v2.0. Por isso, também não há como reverter o rascunho de volta para v1.0.

Se sua assinatura tiver modelos de email v1.0 antes de migrar para o Editor de email 2.0, você terá o seguinte comportamento:

**Aprovado** - Clicar em &quot;Editar rascunho&quot; criará um rascunho v2.0 do modelo de email existente.
**Rascunho** - Clicar em &quot;Editar rascunho&quot; marcará automaticamente esse rascunho como v2.0. Nesse momento, não seria possível descartar e reverter para v1.0 porque não há uma versão aprovada do ativo.
**Aprovado com rascunho** - Clicar em &quot;Editar rascunho&quot; marcará automaticamente esse rascunho como v2.0. Por isso, também não há como reverter o rascunho de volta para v1.0.

Se você aprovar um template de email que era anteriormente v1.0 (em qualquer um dos estados acima), você verá o seguinte comportamento:

Para emails v1.0 existentes que estavam usando o modelo (anteriormente v1.0):\
**Email v1.0 aprovado** - Um rascunho v2.0 será criado para esse email, ainda usando o template v2.0 recém-aprovado. Ele também receberá quaisquer alterações no modelo.\
**Email v1.0 de rascunho** - O rascunho permanecerá v1.0 até você clicar em &quot;Editar rascunho&quot;. Depois disso, ele será marcado automaticamente como v2.0 e receberá quaisquer alterações no modelo.\
**Aprovado com email v1.0 de rascunho** - O rascunho permanecerá v1.0 até você clicar em &quot;Editar rascunho&quot;. Depois disso, ele será marcado automaticamente como v2.0 e receberá quaisquer alterações no modelo.

Para emails v2.0 existentes que estavam usando o modelo (anteriormente v1.0):\
**Email v2.0 aprovado** - Um rascunho v2.0 será criado para esse email, ainda &quot;usando&quot; o modelo recém-aprovado e receberá quaisquer alterações no modelo.\
**Email v2.0 de rascunho** - O rascunho permanecerá como está (v2.0) e receberá quaisquer alterações no modelo.\
**Aprovado com email v2.0 de rascunho** - O rascunho permanecerá como está (v2.0) e receberá quaisquer alterações no modelo.

>[!CAUTION]
>
>Se você aprovar o rascunho v2.0 de um template de email v1.0, o modelo se tornará v2.0. Há **de jeito nenhum** para revertê-la para v1.0.

O que deve ser observado

* Emails aprovados são **never** alterado.

* Os modelos de email aprovados são **never** alterado.

* Em alguns **raros** caso, um Email v1.0 não pode ser aberto no Editor de email 2.0. Se isso ocorrer, descarte o rascunho e entre em contato com o Suporte do Marketo.

>[!MORELIKETHIS]
>
>* [Visão geral do Editor de email 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Sintaxe do modelo de email](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)

