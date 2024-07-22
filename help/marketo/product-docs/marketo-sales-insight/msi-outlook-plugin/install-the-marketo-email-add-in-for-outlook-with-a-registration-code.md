---
unique-page-id: 2949711
description: Instale o Suplemento de email do Marketo para Outlook com um código de registro - Documentação do Marketo - Documentação do produto
title: Instale o Suplemento de email do Marketo para Outlook com um código de registro
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: 40fe81d465d04be97ae5e216250b7e06e6d3791e
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 3%

---

# Instale o Suplemento de email do Marketo para Outlook com um código de registro {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Se os usuários conseguirem acessar as configurações do administrador em seus laptops, você poderá enviar um código de registro diretamente para eles.

Se não tiver recebido um email de convite, peça ao administrador do Marketo para convidá-lo.

>[!PREREQUISITES]
>
>Você deve ter [uma Licença do Suplemento de Email da Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>Não há suporte para a instalação em PCs nos quais a pasta de usuário do Windows contém caracteres que não sejam do inglês. Esta pasta é gerada automaticamente pelo Windows em `<System Root>\Users\` com base no nome de usuário do Windows e pode conter caracteres que não estejam em inglês se o nome de usuário do Windows não estiver em inglês. Entre em contato com a equipe de TI para verificar se há problemas de instalação.

>[!NOTE]
>
>Os recursos de Ações do Sales Insight, incluindo Enviar email de vendas, Adicionar à campanha de vendas e Tarefas, não estão disponíveis nos plug-ins de email do Sales Insight para Gmail e Outlook. No momento, os usuários só têm a capacidade de enviar um email rastreável com ou sem um modelo de email do Marketo por meio de seu cliente de email ao usar os plug-ins de email do Sales Insight.

## Baixar instalador {#download-installer}

1. Identifique a sua [versão do Microsoft Outlook](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}

1. Clique no link para baixar o instalador apropriado para sua versão do Microsoft Outlook.

   >[!NOTE]
   >
   >No momento, os links abaixo estão funcionando apenas no Microsoft Edge ou clicando com o botão direito do mouse no Chrome. Lamentamos o inconveniente.

   | Versão do Outlook | Outlook de 32 bits | Outlook de 64 bits |
   |---|---|---|
   | Outlook 2000 | Não suportado | N/D |
   | Outlook 2003 | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | N/D |
   | Outlook 2007 | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | N/D |
   | Outlook 2010 | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2013 | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2016 | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook 2019 | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |
   | Outlook para Mac | Não suportado | Não suportado |
   | Outlook Web App | Não suportado | Não suportado |
   | Office 365* | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup32.msi) | [Baixar](https://munchkin.marketo.net/MarketoAddInSetup64.msi) |

   *Versão do Office 365: somente cliente Windows (no Windows 10, Enterprise ou Pro).

   >[!IMPORTANT]
   >
   >A Microsoft lançou uma [nova versão do Outlook para Windows](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}. Esta nova versão não oferece suporte ao plug-in MSI Outlook existente. O plug-in MSI Outlook continuará a funcionar para áreas de trabalho do Windows que executam a versão clássica do Outlook. Para saber mais sobre o novo Outlook para Windows para organizações, [clique aqui](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"}.

## Copie seu código de registro {#copy-your-registration-code}

1. Copie o código de registro do email de convite recebido.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Feche o Microsoft Outlook.

   ![](assets/ent-key-close-outlook-hand.png)

## Instalar {#install}

1. Execute o instalador.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Se você receber um aviso de segurança, não se preocupe! Basta clicar em **Executar**.

1. Clique em **Avançar**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Preencha **Nome**, **Sobrenome**, **Endereço de email** e copie e cole o **Código de registro** do email no formulário e clique em **Avançar**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Se a instalação falhar, verifique com o departamento de TI se o tráfego HTTPS não está bloqueado. O instalador requer que o tráfego HTTPS seja aberto.

1. Clique em **Avançar** para instalar no local padrão.

   ![](assets/select-installation-folder-hand.png)

1. Clique em **Avançar**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Se você receber um aviso de segurança sobre um editor desconhecido, clique em **Sim**.

1. A instalação foi concluída, clique em **Fechar**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Agora abra o Microsoft Outlook e veja os botões Marketo.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Excelente! Agora os botões do Marketo estão em um lugar melhor.

Saiba mais sobre como usar as ações Mensagem e registro do Marketo com o Marketo.

>[!MORELIKETHIS]
>
>* [Enviar e Rastrear um Email com o Suplemento de Email do Marketo para Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Enviar e Rastrear do Outlook Usando um Modelo do Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
