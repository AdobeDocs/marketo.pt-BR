---
unique-page-id: 10095307
description: Saiba como configurar regras de filtro de sincronização personalizadas para endereços de email no Dynamics. Use fluxos de trabalho para definir Sincronizar com o Mkto com base no fato de o cliente potencial ou o contato ter um email.
title: Regras de filtro de sincronização personalizado para um endereço de email
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/SPEV9J4rabu7tMrPEOW8JYg2r7ihtTzE6OmJZvkOIZ4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 221
ht-degree: 7%

---

# Regras de filtro de sincronização personalizado para um endereço de email {#custom-sync-filter-rules-for-an-email-address}

Para impedir a sincronização de registros que não têm um endereço de email, siga estas regras.

* Quando um cliente potencial for criado OU quando o campo de endereço de email do cliente potencial for atualizado, verifique se ele tem um endereço de email e, em caso positivo, altere Sincronizar para Mkto para **[!UICONTROL Verdadeiro]**. Caso contrário, altere para **[!UICONTROL Falso]**

* Quando um contato for criado OU quando o campo de endereço de email do contato for atualizado, verifique se o contato tem um endereço de email e, em caso positivo, altere Sync para Mkto para **[!UICONTROL True]** e altere Sync para Mkto para **[!UICONTROL True]** no registro de Conta. Caso contrário, altere para **[!UICONTROL Falso]**

* Quando o campo Nome da empresa (parentcustomerid) do contato for atualizado, verifique se o campo Sincronizar com Mkto do contato é verdadeiro. Se for, altere também Sync para Mkto na conta para **[!UICONTROL True]**
* Quando o campo Cliente em potencial (customerid) da oportunidade ou Contato (parentcontactid) for atualizado, verifique se o campo Sincronizar com Mkto da conta é verdadeiro ou se o campo Sincronizar com Mkto do contato é verdadeiro. Se for, altere Sync para Mkto na oportunidade para **[!UICONTROL True]** também
