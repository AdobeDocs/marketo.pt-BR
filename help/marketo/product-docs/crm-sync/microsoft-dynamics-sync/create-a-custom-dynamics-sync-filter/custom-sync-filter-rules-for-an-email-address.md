---
unique-page-id: 10095307
description: Regras de filtro de sincronização personalizadas para um endereço de email - Documentação do Marketo - Documentação do produto
title: Regras de Filtro de Sincronização Personalizada para um Endereço de Email
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Regras de Filtro de Sincronização Personalizada para um Endereço de Email {#custom-sync-filter-rules-for-an-email-address}

Para impedir a sincronização de registros que não têm um endereço de email, siga estas regras.

* Quando um cliente potencial for criado OU quando o campo de endereço de email do cliente potencial for atualizado, verifique se ele tem um endereço de email e, em caso positivo, altere Sincronizar para Mkto para **[!UICONTROL True]**. Caso contrário, altere para **[!UICONTROL Falso]**.

* Quando um contato for criado OU quando o campo de endereço de email do contato for atualizado, verifique se o contato tem um endereço de email e, em caso positivo, altere Sync para Mkto para **[!UICONTROL True]** e altere Sync para Mkto para **[!UICONTROL True]** no registro de Conta. Caso contrário, altere para **[!UICONTROL Falso]**.

* Quando o campo Nome da empresa (parentcustomerid) do contato for atualizado, verifique se o campo Sincronizar com Mkto do contato é verdadeiro. Se for, altere também Sync para Mkto na conta para **[!UICONTROL True]**.

* Quando o campo Cliente em potencial (customerid) da oportunidade ou Contato (parentcontactid) for atualizado, verifique se o campo Sincronizar com Mkto da conta é verdadeiro ou se o campo Sincronizar com Mkto do contato é verdadeiro. Se for, altere Sync para Mkto na oportunidade para **[!UICONTROL True]** também.
