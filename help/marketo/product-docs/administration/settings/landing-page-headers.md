---
description: Cabeçalhos da página de aterrissagem - Documentação do Marketo - Documentação do produto
title: Cabeçalhos da página de destino
exl-id: 58eaa0cd-2a2b-4abe-9180-f60a2a1dcc87
feature: Administration, Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '131'
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
>É importante analisar essas configurações com a equipe de TI para determinar como a política da sua organização deve ser definida. Configurações incorretas podem impedir que alguns visitantes acessem suas Landing Pages.
