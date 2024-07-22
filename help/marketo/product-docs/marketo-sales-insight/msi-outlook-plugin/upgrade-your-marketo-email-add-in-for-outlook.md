---
unique-page-id: 2949279
description: Atualizar o suplemento de email do Marketo para Outlook - Documentação do Marketo - Documentação do produto
title: Atualizar o Suplemento de Email do Marketo para Outlook
exl-id: 079f1142-8062-448c-aa07-59ecd89a718f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 15%

---

# Atualizar o Suplemento de Email do Marketo para Outlook {#upgrade-your-marketo-email-add-in-for-outlook}

Quando uma nova versão do Suplemento de email do Marketo para Outlook estiver disponível, siga estas instruções para atualizar.

>[!NOTE]
>
>A partir de 01/10/20, a versão mais recente do plug-in do Outlook não é mais compatível com o modo offline. Isso entrará em vigor após a instalação/atualização em ou após 10/1.

## Baixar instalador {#download-installer}

Baixe o instalador apropriado para sua versão do Microsoft Outlook.

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th colspan="2">Instalação de Convite para Usuário Único</th> 
   <th colspan="2">Instalação da Chave Corporativa</th> 
  </tr> 
  <tr> 
   <td><strong>Versão do Outlook</strong></td> 
   <td><strong>32 bits</strong></td> 
   <td><strong>64 bits</strong></td> 
   <td><strong>32 bits</strong></td> 
   <td><strong>64 bits</strong></td> 
  </tr> 
  <tr> 
   <td>Outlook 2000</td> 
   <td>Não suportado</td> 
   <td>N/D</td> 
   <td>Não suportado</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Outlook 2003</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td>N/D</td> 
   <td>Não suportado</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Outlook 2007</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td>N/D</td> 
   <td>Não suportado</td> 
   <td>N/D</td> 
  </tr> 
  <tr> 
   <td>Outlook 2010</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Baixar</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Baixar</a></td> 
  </tr> 
  <tr> 
   <td>Outlook 2013</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Baixar</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Baixar</a></td> 
  </tr> 
  <tr> 
   <td>Outlook 2016</td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Baixar</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Baixar</a></td> 
  </tr> 
  <tr> 
   <td colspan="1">Outlook 2019</td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Baixar</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Baixar</a></td> 
  </tr> 
  <tr> 
   <td>Outlook para Mac</td> 
   <td>Não suportado</td> 
   <td>Não suportado</td> 
   <td>Não suportado</td> 
   <td>Não suportado</td> 
  </tr> 
  <tr> 
   <td colspan="1">Outlook Web App</td> 
   <td colspan="1">Não suportado</td> 
   <td colspan="1">Não suportado</td> 
   <td colspan="1">Não suportado</td> 
   <td colspan="1">Não suportado</td> 
  </tr> 
  <tr> 
   <td colspan="1">Office 365*</td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Baixar</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup32.msi" rel="nofollow">Baixar</a></td> 
   <td colspan="1"><a href="https://munchkin.marketo.net/MarketoAddInSetup64.msi" rel="nofollow">Baixar</a></td> 
  </tr> 
 </tbody> 
</table>

&#42;Versão do Office 365: somente cliente Windows (no Windows 10, Enterprise ou Pro).

## Atualizar {#upgrade}

1. Identifique a sua [versão do Microsoft Outlook](https://support.microsoft.com/en-us/office/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c?ui=en-us&amp;rs=en-us&amp;ad=us).

1. Selecione sua versão na lista acima.

1. Execute o instalador.

   ![](assets/image2014-9-23-16-3a53-3a56.png)

1. Clique em **Avançar**.

   ![](assets/image2014-9-23-16-3a54-3a8.png)

   >[!NOTE]
   >
   >Em certos casos, os dados estarão ausentes. Copie do email de registro e feche o Outlook.

1. Feche o Microsoft Outlook.

   ![](assets/ent-key-close-outlook-hand.png)

1. Você perceberá que todas as suas informações estão pré-preenchidas. Basta clicar em **Avançar**.

   ![](assets/image2014-9-23-16-3a54-3a40.png)

   >[!TIP]
   >
   >Se a instalação falhar, peça ao seu departamento de TI para garantir que o tráfego HTTPS não seja bloqueado. O instalador requer que o tráfego HTTPS seja aberto.

1. Clique em **Avançar** para instalar no local padrão.

   ![](assets/image2014-9-23-16-3a54-3a55.png)

1. Clique em **Avançar**.

   ![](assets/image2014-9-23-16-3a55-3a20.png)

1. A instalação foi concluída. Clique em **Fechar**.

   ![](assets/image2014-9-23-16-3a55-3a34.png)

1. Agora abra o Microsoft Outlook para ver a versão mais recente dos botões do Marketo.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

>[!MORELIKETHIS]
>
>* [Enviar e Rastrear um Email com o Suplemento de Email do Marketo para Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [Enviar e Rastrear do Outlook Usando um Modelo do Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)
