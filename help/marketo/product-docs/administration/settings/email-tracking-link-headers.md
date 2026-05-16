---
description: Como personalizar os cabeçalhos de link de rastreamento de email no Admin em Email, incluindo Strict-Transport-Security for HTTPS, com orientação de revisão de TI.
title: Cabeçalhos do link de rastreamento de email
exl-id: 2db1f1b3-3afe-4710-a8b1-b06fbf09ec8c
feature: Administration
TQID: https://experienceleague.adobe.com/myoUsAnpIvAZVY-ar4iQl9xDHr886vAH-l0YXtM1mfg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 119
ht-degree: 10%

---

# Cabeçalhos do link de rastreamento de email {#email-tracking-link-headers}

Siga as etapas abaixo para personalizar os cabeçalhos do link de rastreamento de email.

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/email-tracking-link-headers-1.png)

1. Clique em **[!UICONTROL Email]**.

   ![](assets/email-tracking-link-headers-2.png)

1. Role para baixo até Opções de cabeçalho personalizadas. Escolha as configurações desejadas e clique em **[!UICONTROL Salvar alterações]**.

   ![](assets/email-tracking-link-headers-3.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>Use isso para garantir que os links de rastreamento sempre sejam distribuídos por HTTPS (deve ser definido somente para assinaturas com links de rastreamento protegidos por SSL)</td>
 </tr>
</table>

>[!CAUTION]
>
>É importante analisar essas configurações com a equipe de TI para determinar como a política da organização deve ser definida. Configurações incorretas podem impedir que alguns visitantes acessem seus links de email.
