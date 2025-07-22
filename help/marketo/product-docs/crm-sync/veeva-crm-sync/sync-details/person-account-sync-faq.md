---
description: Perguntas frequentes sobre a Sincronização de conta de pessoa - Documentação do Marketo - Documentação do produto
title: Perguntas frequentes sobre Sincronização de Conta de Pessoa
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Perguntas frequentes sobre Sincronização de Conta de Pessoa {#person-account-sync-faq}

O Marketo Engage sincroniza todo o banco de dados com [!DNL Veeva] para o tipo de registros Conta de pessoa. Após a sincronização, ele aguarda 5 minutos e sincroniza novamente, o dia todo, todos os dias.

Contas de pessoas podem ser configuradas no [!DNL Veeva] para atender às necessidades da sua organização.

>[!NOTE]
>
>Somente sincronizamos contas de nível &quot;Profissional&quot; como Contas de pessoa.

**O que é uma conta de pessoa?**

Uma conta de pessoa é muito semelhante ao objeto de conta no [!DNL Veeva] CRM. No entanto, uma conta de pessoa tem acesso aos campos de conta e de contato.

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

A sincronização dos campos relacionados ao contato da Conta de pessoa é bidirecional. Se você fizer alterações em um contato no [!DNL Veeva] CRM ou no Marketo, suas atualizações serão refletidas em ambos os sistemas. Os campos na conta só são sincronizados em uma direção, do [!DNL Veeva] CRM para o Marketo.

**E se forem feitas alterações em ambos os sistemas nos campos Contato da Conta de Pessoa ao mesmo tempo?**

Nós seríamos legais e deixaríamos [!DNL Veeva] CRM ganhar. No entanto, é raro que esse tipo de colisão de dados ocorra.

**Os tipos de registros de Cliente Potencial ou Contato estão sincronizados com o [!DNL Veeva] CRM?**

O CRM [!DNL Veeva] só lida realmente com objetos de Conta de Pessoa e também tem Contas Comerciais. Os tipos tradicionais de CRM de Cliente Potencial, Contatos e Oportunidades não estão realmente em uso nos sistemas tradicionais de CRM do [!DNL Veeva]. Eles podem ser criados no [!DNL Veeva] CRM, mas não têm suporte oficial usando esse conector.

**Posso converter uma pessoa em um contato no Marketo?**

Não, já que o Cliente Potencial e o Contato não são tipos compatíveis para a sincronização com o CRM [!DNL Veeva]. Como resultado, não há suporte para a conversão.

**Posso forçar manualmente uma sincronização de um contato?**

Não, já que Contato não é um tipo de registro independente, não há suporte para sincronização de uma pessoa com [!DNL Veeva].

**Cada campo padrão é sincronizado com o Marketo?**

Não, nem todos os campos padrão são úteis. Todos os campos personalizados podem fazer parte da sincronização.

>[!NOTE]
>
>O Marketo só sincronizará os campos aos quais o usuário do Marketo Sync tem acesso.

**A Marketo respeitará as regras de validação [!DNL Veeva]?**

Sim, se houver um conflito, registraremos o resultado no Log de atividades do lead.

>[!MORELIKETHIS]
>
>* [Padrão [!DNL Veeva] Mapeamento de campos](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Sincronizando Mensagens de Chamada e Chave de Chamada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
