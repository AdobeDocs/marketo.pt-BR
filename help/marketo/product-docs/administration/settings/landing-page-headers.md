---
description: Cabeçalhos de página de aterrissagem - Documentos do Marketo - Documentação do produto
title: Cabeçalhos de página de aterrissagem
hide: true
hidefromtoc: true
source-git-commit: 921c3279b53bc18ac753b1e3f0672a70fe11abe7
workflow-type: tm+mt
source-wordcount: '129'
ht-degree: 0%

---

# Cabeçalhos de página de aterrissagem {#landing-page-headers}

Siga as etapas abaixo para personalizar alguns cabeçalhos HTTP nos domínios da Landing page.

1. No Marketo, clique em **Administrador**.

   ![](assets/landing-page-headers-1.png)

1. Clique em **Páginas de aterrissagem**.

   ![](assets/landing-page-headers-2.png)

1. Clique em **Editar** ao lado de Cabeçalhos HTTP de página inicial.

   ![](assets/landing-page-headers-3.png)

1. Escolha as configurações desejadas e clique em **Salvar** quando concluído.

   ![](assets/landing-page-headers-4.png)

<table>
 <tr>
  <td><strong>Strict-Transport-Security</strong></td>
  <td>Use essa opção para garantir que as conexões com as Páginas de aterrissagem sejam sempre veiculadas por HTTPS (só deve ser definido para assinaturas com Páginas de aterrissagem seguras por SSL)</td>
 </tr>
 <tr>
  <td><strong>X-Frame-Options</strong></td>
  <td>Permite definir se os ativos hospedados pelo Marketo Engage podem ou não ser incorporados em páginas da Web externas</td>
 </tr>
</table>

>[!CAUTION]
>
>É importante analisar essas configurações com a equipe de TI para determinar a política da organização a ser definida. Configurações incorretas podem impedir que alguns visitantes acessem suas Páginas de aterrissagem.
