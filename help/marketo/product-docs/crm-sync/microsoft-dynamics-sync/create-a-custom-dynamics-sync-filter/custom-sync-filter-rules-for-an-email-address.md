---
unique-page-id: 10095307
description: Regras de filtro de sincronização personalizadas para um endereço de email - Documentação do Marketo - Documentação do produto
title: Regras de Filtro de Sincronização Personalizada para um Endereço de Email
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Regras de Filtro de Sincronização Personalizada para um Endereço de Email {#custom-sync-filter-rules-for-an-email-address}

Para impedir a sincronização de registros que não têm um endereço de email, siga estas regras.

* Quando um cliente potencial for criado OU quando o campo de endereço de email do cliente potencial for atualizado, verifique se o cliente potencial tem um endereço de email e, em caso positivo, altere Sincronizar para Marcar para **True**. Caso contrário, altere para **Falso**

* Quando um contato for criado OU quando o campo de endereço de email do contato for atualizado, verifique se o contato tem um endereço de email e, em caso positivo, altere Sincronizar para Marcar para **True** e altere Sync para Mkto para **True** no registro Account. Caso contrário, altere para **Falso**

* Quando o campo Nome da empresa (parentcustomerid) do contato for atualizado, verifique se o campo Sincronizar com Mkto do contato é verdadeiro. Se estiver, altere Sync para Mkto na conta para **True** também
* Quando o campo Cliente em potencial (customerid) da oportunidade ou Contato (parentcontactid) for atualizado, verifique se o campo Sincronizar com Mkto da conta é verdadeiro ou se o campo Sincronizar com Mkto do contato é verdadeiro. Se for, altere Sync para Mkto na oportunidade de **True** também
