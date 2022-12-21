---
unique-page-id: 10095307
description: Regras de filtro de sincronização personalizada para um endereço de email - Documentos do Marketo - Documentação do produto
title: Regras de Filtro de Sincronização Personalizado para um Endereço de Email
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Regras de Filtro de Sincronização Personalizado para um Endereço de Email {#custom-sync-filter-rules-for-an-email-address}

Para evitar a sincronização de registros que não têm um endereço de email, siga essas regras.

* Quando um cliente potencial é criado OU quando o campo de endereço de email do cliente potencial é atualizado, verifique se o cliente potencial tem um endereço de email e, em caso afirmativo, altere Sync para Mkto **Verdadeiro**. Caso contrário, altere para **Falso**

* Quando um contato é criado OU quando o campo de endereço de email do contato é atualizado, verifique se o contato tem um endereço de email e, em caso afirmativo, altere Sync para Mkto **Verdadeiro** e altere Sincronizar para Mkto para **Verdadeiro** no registro da conta. Caso contrário, altere para **Falso**

* Quando o campo Company Name (parentcustomerid) do contato for atualizado, verifique se o campo Sync to Mkto do contato é verdadeiro. Se estiver, altere Sync para Mkto na conta para **Verdadeiro** also
* Quando o campo Cliente potencial (customerid) da oportunidade ou Contato (parentcontactid) for atualizado, verifique se o campo Sincronizar para Mkto da conta é verdadeiro ou se o campo Sincronizar para Mkto do contato é verdadeiro. Se estiver, altere Sincronizar para Mkto na oportunidade para **Verdadeiro** also
