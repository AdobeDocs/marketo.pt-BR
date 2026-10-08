---
description: Como personalizar cabeçalhos HTTP para domínios de página de aterrissagem, incluindo Strict-Transport-Security e X-Frame-Options.
title: Cabeçalhos da página de destino
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
TQID: 'https://experienceleague.adobe.com/ecRuR4V-YCsesHZpm9UrP1rPlOjBCediq-9DtXZRfBo'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: edda586e-0147-48f2-b791-992622a00783
    internal-label: Landing pages
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 4%
---
# Cabeçalhos da página de destino {#landing-page-headers}

Siga as etapas abaixo para personalizar alguns dos cabeçalhos HTTP nos domínios da sua página de aterrissagem.

1. No Marketo, clique em **[!UICONTROL Admin]**.

   ![](assets/landing-page-headers-1.png)

1. Clique em **[!UICONTROL Landing Pages]**.

   ![](assets/landing-page-headers-2.png)

1. Clique em **[!UICONTROL Editar]** ao lado de Cabeçalhos HTTP de landing pages.

   ![](assets/landing-page-headers-3.png)

1. Escolha as configurações desejadas e clique em **[!UICONTROL Salvar]** quando terminar.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>[!UICONTROL Segurança-Transporte-Restrita]</strong></td>
  <td>Use isso para garantir que as conexões com as páginas de aterrissagem sempre sejam fornecidas por HTTPS (só deve ser definido para assinaturas com Páginas de aterrissagem protegidas por SSL)</td>
 </tr>
 <tr>
  <td><strong>[!UICONTROL X-Frame-Options]</strong></td>
  <td>Permite definir se os ativos hospedados pela Marketo Engage podem ou não ser incorporados em páginas externas da Web</td>
 </tr>
</table>

>[!CAUTION]
>
>É importante analisar essas configurações com a equipe de TI para determinar como a política da organização deve ser definida. Configurações incorretas podem impedir que alguns visitantes acessem suas Landing Pages.
