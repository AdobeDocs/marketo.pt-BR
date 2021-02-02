---
unique-page-id: 10095307
description: Regras de filtro de sincronização personalizada para um endereço de email - Documentos do marketing - Documentação do produto
title: Regras de filtro de sincronização personalizada para um endereço de email
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---


# Regras de filtro de sincronização personalizada para um endereço de email {#custom-sync-filter-rules-for-an-email-address}

Para impedir a sincronização de registros que não tenham um endereço de email, siga estas regras.

* Quando um cliente potencial é criado OU quando o campo de endereço de email do cliente potencial é atualizado, verifique se o cliente potencial tem um endereço de email e, se tiver, altere Sincronizar para Mkto para **Verdadeiro**. Caso contrário, mude para **False**

* Quando um contato for criado OU quando o campo de endereço de email do contato for atualizado, verifique se o contato tem um endereço de email e, se tiver, altere Sincronizar para Mkto **True** e altere Sincronizar para Mkto para **True** no registro da conta. Caso contrário, altere para **False**

* Quando o campo Nome da Empresa do contato (parentcustomerid) for atualizado, verifique se o campo Sincronizar para Mkto do contato é verdadeiro. Se estiver, altere Sync para Mkto na conta para **True** também
* Quando o campo Cliente potencial (customerid) da oportunidade ou Contato (parentcontactid) for atualizado, verifique se o campo Sincronizar para Mkto da conta é verdadeiro ou se o campo Sincronizar para Mkto do contato é verdadeiro. Se estiver, altere Sync para Mkto na oportunidade para **True** também
