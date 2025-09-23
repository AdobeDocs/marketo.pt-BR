---
unique-page-id: 11373011
description: Transição para o Editor de email 2.0 - Documentação do Marketo - Documentação do produto
title: Transição para o Editor de email 2.0
exl-id: eb9ec8cc-d6e8-4839-a4d9-608d2f264cbb
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Transição para [!DNL Email Editor 2.0] {#transitioning-to-email-editor}

A partir da versão de junho de 2019, todas as assinaturas do Marketo passaram para [!DNL Email Editor 2.0]. [Saiba mais](https://nation.marketo.com/docs/DOC-7038) sobre a descontinuação de [!DNL Email Editor 1.0].

Emails e templates de email em sua assinatura devem ter um número de versão. A versão pode ser encontrada na página de resumo do ativo.

![](assets/five-5.png)

Por padrão, todos os emails e modelos de email existentes serão marcados como v1.0 se tiverem sido criados antes da versão do primeiro trimestre de 1916 ou após o lançamento, quando o Editor de email 2.0 estiver desativado. Com o Editor de email 2.0 ativado automaticamente, você verá o seguinte comportamento:

* Ao criar um novo email, o [Seletor de Modelo de Email](email-template-picker-overview.md) será exibido e você poderá escolher um modelo de email v2.0.
* Sempre que você criar ou editar um email com [!DNL Email Editor 2.0], o email resultante será **sempre** marcado como v2.0 (mesmo se você tiver usado um modelo de email v1.0).

Se sua assinatura tiver emails v1.0 antes de migrar para o [!DNL Email Editor 2.0], você terá o seguinte comportamento com base no estado atual do ativo:

**Aprovado** - Clicar em &quot;Editar rascunho&quot; criará um rascunho v2.0 do email aprovado. Se você aprovar o rascunho da v2.0, o estado aprovado do email se tornará v2.0 e não haverá como reverter para a v1.0.
**Rascunho** - Clicar em &quot;Editar Rascunho&quot; marcará automaticamente esse rascunho como v2.0. Nesse momento, não será possível descartar e reverter para a v1.0 porque não há uma versão aprovada do ativo.
**Aprovado com Rascunho** - Clicar em &quot;Editar Rascunho&quot; marcará automaticamente esse rascunho como v2.0. Por causa disso, também não há como reverter o rascunho para a v1.0.

Se sua assinatura tiver modelos de email v1.0 antes de migrar para o [!DNL Email Editor 2.0], você terá o seguinte comportamento:

**Aprovado** - Clicar em &quot;Editar rascunho&quot; criará um rascunho v2.0 do modelo de email existente.
**Rascunho** - Clicar em &quot;Editar Rascunho&quot; marcará automaticamente esse rascunho como v2.0. Nesse momento, não seria possível descartar e reverter para a v1.0 porque não há uma versão aprovada do ativo.
**Aprovado com Rascunho** - Clicar em &quot;Editar Rascunho&quot; marcará automaticamente esse rascunho como v2.0. Por causa disso, também não há como reverter o rascunho para a v1.0.

Se você aprovar um template de email que era v1.0 anteriormente (em qualquer um dos estados acima), verá o seguinte comportamento:

Para emails da v1.0 existentes que estavam usando o modelo (anteriormente v1.0):
**Email v1.0 aprovado** - Um rascunho v2.0 será criado para este email, ainda usando o modelo v2.0 recém-aprovado. Ele também receberá todas as alterações no modelo.
**Email v1.0 de rascunho** - O rascunho permanecerá v1.0 até que você clique em &quot;Editar rascunho&quot;. Depois disso, ele será marcado automaticamente como v2.0 e receberá todas as alterações do modelo.
**Aprovado com email v1.0 de rascunho** - O rascunho permanecerá v1.0 até que você clique em &quot;Editar rascunho&quot;. Depois disso, ele será marcado automaticamente como v2.0 e receberá todas as alterações do modelo.

Para emails da v2.0 existentes que estavam usando o modelo (anteriormente v1.0):
**Email v2.0 aprovado** - Um rascunho v2.0 será criado para este email, ainda &quot;usando&quot; o modelo recém-aprovado, e receberá todas as alterações no modelo.
**Email v2.0 de rascunho** - O rascunho permanecerá como está (v2.0) e receberá todas as alterações de modelo.
**Aprovado com o rascunho v2.0 email** - O rascunho permanecerá como está (v2.0) e receberá todas as alterações no modelo.

>[!CAUTION]
>
>Se você aprovar o rascunho v2.0 de um modelo de email v1.0, o modelo se tornará v2.0. Não há **nenhuma maneira** de revertê-lo para v1.0.

Itens a Observar

* Os emails aprovados **nunca** foram alterados.

* Os modelos de email aprovados **nunca** foram alterados.

* Em alguns casos **raros**, um email v1.0 não pode ser aberto em [!DNL Email Editor 2.0]. Se isso ocorrer, descarte o rascunho e entre em contato com o Suporte da Marketo.

>[!MORELIKETHIS]
>
>* [[!DNL Email Editor 2.0] Visão geral](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Sintaxe do modelo de email](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)
