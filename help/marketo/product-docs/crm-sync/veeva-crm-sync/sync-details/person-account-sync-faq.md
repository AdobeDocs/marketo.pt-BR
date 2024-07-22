---
description: Perguntas frequentes sobre a Sincronização de conta de pessoa - Documentação do Marketo - Documentação do produto
title: Perguntas frequentes sobre Sincronização de Conta de Pessoa
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Perguntas frequentes sobre Sincronização de Conta de Pessoa {#person-account-sync-faq}

O Marketo Engage sincroniza todo o banco de dados com o Veeva para o tipo de registros Conta de pessoa. Após a sincronização, ele aguarda 5 minutos e sincroniza novamente, o dia todo, todos os dias.

Contas pessoais podem ser configuradas em Veeva para atender às necessidades de sua organização.

>[!NOTE]
>
>Somente sincronizamos contas de nível &quot;Profissional&quot; como Contas de pessoa.

**O que é uma conta de pessoa?**

Uma conta de pessoa é muito semelhante ao objeto da conta no Veeva CRM. No entanto, uma conta de pessoa tem acesso aos campos de conta e de contato.

**O que acontece quando uma conta de pessoa é sincronizada com o Marketo?**

Uma conta de pessoa é sincronizada com a Marketo como uma empresa e como uma pessoa.

>[!NOTE]
>
>Os campos personalizados de uma conta de pessoa são copiados para a empresa e para a pessoa no Marketo.

**Como faço para diferenciar contas comerciais e contas pessoais?**

Use o filtro Conta &quot;É Pessoa&quot; na sua Smart List para separar contas pessoais das contas comerciais padrão.

**Qual campo de email devo usar para contas de pessoas?**

Há dois campos de email para uma conta de pessoa. Use o campo Endereço de email em seus formulários (não o Endereço de email de pessoa) para garantir que a eliminação de duplicação e outros processamentos de email da Marketo funcionem corretamente.

## Direção da sincronização {#sync-direction}

A sincronização dos campos relacionados ao contato da Conta de pessoa é bidirecional. Se você fizer alterações em um contato no Veeva CRM ou no Marketo, suas atualizações serão refletidas em ambos os sistemas. Os campos na conta só são sincronizados em uma direção, do Veeva CRM para o Marketo.

**E se forem feitas alterações em ambos os sistemas nos campos Contato da Conta de Pessoa ao mesmo tempo?**

Seríamos legais e deixaríamos a Veeva CRM ganhar. No entanto, é raro que esse tipo de colisão de dados ocorra.

**Os tipos de registros de Cliente Potencial ou Contato estão sincronizados com o Veeva CRM?**

O Veeva CRM só lida realmente com objetos de Conta pessoal e também tem Contas comerciais. Os tipos tradicionais de CRM de cliente potencial, contatos e oportunidades não estão realmente em uso nos sistemas tradicionais de Veeva CRM. Eles podem ser criados no Veeva CRM, mas não são oficialmente compatíveis usando esse conector.

**Posso converter uma pessoa em um contato no Marketo?**

Não, já que lead e contato não são tipos suportados para a sincronização com o Veeva CRM. Como resultado, não há suporte para a conversão.

**Posso forçar manualmente uma sincronização de um contato?**

Não, já que Contato não é um tipo de registro independente, a sincronização de uma pessoa com Veeva não é suportada.

**Cada campo padrão é sincronizado com o Marketo?**

Não, nem todos os campos padrão são úteis. Todos os campos personalizados podem fazer parte da sincronização.

>[!NOTE]
>
>O Marketo só sincronizará os campos aos quais o usuário do Marketo Sync tem acesso.

**A Marketo respeitará as regras de validação da Veeva?**

Sim, se houver um conflito, registraremos o resultado no Log de atividades do lead.

>[!MORELIKETHIS]
>
>* [Mapeamento de campo Veeva padrão](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Sincronizando Mensagens de Chamada e Chave de Chamada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
