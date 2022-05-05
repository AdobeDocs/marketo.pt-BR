---
description: Perguntas frequentes sobre sincronização de conta de pessoa - Documentos do Marketo - Documentação do produto
title: Perguntas frequentes sobre sincronização de conta de pessoa
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Perguntas frequentes sobre sincronização de conta de pessoa {#person-account-sync-faq}

O Marketo Engage sincroniza todo o banco de dados com Veeva para o tipo de registro Conta de pessoa . Depois da sincronização, ela aguarda 5 minutos e depois sincroniza novamente, o dia inteiro, todos os dias.

As contas de pessoa podem ser configuradas em Veeva para atender às necessidades de sua organização.

>[!NOTE]
>
>As contas Veeva padrão são Profissionais.

**O que é uma conta de pessoa?**

Uma conta de pessoa é muito semelhante ao objeto da conta no CRM Veeva. No entanto, uma conta de pessoa tem acesso aos campos da conta e aos campos de contato.

**O que acontece quando uma conta de pessoa é sincronizada com o Marketo?**

Uma conta de pessoa é sincronizada com o Marketo como uma empresa e como uma pessoa.

>[!NOTE]
>
>Os campos personalizados de uma conta de pessoa são copiados para a empresa e para a pessoa no Marketo.

**Como faço para diferenciar contas comerciais e contas pessoais?**

Use o filtro Conta &quot;É Pessoa&quot; em sua Smart List para separar contas de pessoas de contas comerciais padrão.

**Qual campo de email devo usar para contas de pessoas?**

Há dois campos de email para uma conta de pessoa. Use o campo Endereço de email em seus formulários (não o Endereço de email da pessoa) para garantir que a eliminação da duplicação da Marketo e outro processamento de email funcionem corretamente.

## Sincronizar Direção {#sync-direction}

A sincronização dos campos relacionados ao contato da Conta de pessoa é bidirecional. Se você fizer alterações em um contato no Veeva CRM ou Marketo, suas atualizações serão refletidas em ambos os sistemas. Os campos na conta só são sincronizados em uma direção, de Veeva CRM para Marketo.

**E se as alterações forem feitas em ambos os sistemas para campos de Contato na Conta de Pessoa ao mesmo tempo?**

Nós seríamos legais e deixaríamos Veeva CRM ganhar. No entanto, é raro que esse tipo de colisão de dados ocorra.

**Os tipos de registro de lead ou contato são sincronizados com Veeva CRM?**

Veeva CRM só lida com objetos de Conta de pessoa e também tem Contas comerciais. Os tradicionais tipos de CRM de Lead, Contatos e Oportunidades não são realmente usados nos sistemas tradicionais de CRM de Veeva. Eles podem ser criados no Veeva CRM e a sincronização pode trazê-los para o Marketo, mas não são suportados oficialmente usando esse conector.

**Posso converter uma pessoa em um contato no Marketo?**

Não, já que os tipos de lead e contato não são suportados para a sincronização com Veeva CRM. Como resultado, a conversão não é suportada.

**Posso forçar manualmente uma sincronização de um contato?**

Não, como o Contato não é um tipo de registro independente, sincronizar uma pessoa para Veeva não é suportado.

**Cada campo padrão é sincronizado com o Marketo?**

Não, nem todos os campos padrão são úteis. Todos os campos personalizados podem fazer parte da sincronização.

>[!NOTE]
>
>O Marketo só sincronizará os campos aos quais o Usuário do Marketo Sync tem acesso.

**A Marketo respeitará as regras de validação de Veeva?**

Sim, se houver um conflito, registraremos o resultado no Log de atividades do cliente potencial.

>[!MORELIKETHIS]
>
>* [Mapeamento de Campo de Veeva Padrão](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target=&quot;_blank&quot;}
>* [Sincronização de mensagens de chave de chamada e de chamada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}

