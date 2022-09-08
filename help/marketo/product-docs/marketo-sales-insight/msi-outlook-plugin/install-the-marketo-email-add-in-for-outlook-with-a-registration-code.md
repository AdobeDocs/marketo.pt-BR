---
unique-page-id: 2949711
description: Instale o complemento de email do Marketo para Outlook com um código de registro - Marketo Docs - Documentação do produto
title: Instalar o Suplemento de Email do Marketo para Outlook com um Código de Registro
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
source-git-commit: 0dec1dc142a7296ce9d5db91493f654dbe7ee99a
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 5%

---

# Instalar o Suplemento de Email do Marketo para Outlook com um Código de Registro {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

Se os usuários conseguirem acessar as configurações do administrador em seus laptops, você poderá enviar um código de registro diretamente para eles.

Caso não tenha recebido um e-mail de convite, peça ao administrador da Marketo para convidá-lo.

>[!PREREQUISITES]
>
>Você deve ser [emitida uma Licença do Marketo Email Add-in](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/issue-a-marketo-email-add-in-license.md).

>[!IMPORTANT]
>
>A instalação não é suportada em PCs onde a pasta Usuário do Windows contém caracteres que não são em inglês. Esta pasta é gerada automaticamente pelo Windows em <System Root>\Usuários\ com base no nome de usuário do Windows e pode conter caracteres que não sejam em inglês se o nome de usuário do Windows for um nome que não seja em inglês. Entre em contato com a equipe de TI para verificar se você está tendo problemas de instalação.

>[!NOTE]
>
>Em 1/1/20, a versão mais recente do plug-in do Outlook parou de oferecer suporte ao modo offline.

## Baixar instalador {#download-installer}

1. Identifique o [Versão do Microsoft Outlook](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c)

1. Clique no link para baixar o instalador apropriado para sua versão do Microsoft Outlook.

   >[!NOTE]
   >
   >No momento, os links abaixo estão funcionando somente no Microsoft Edge ou clicando com o botão direito do mouse no Chrome. Desculpe por qualquer inconveniência.

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

   *Versão do Office 365: Somente cliente Windows (no Windows 10, Enterprise ou Pro).

## Copiar seu código de registro {#copy-your-registration-code}

1. Copie o código de registro do email de convite recebido.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Feche o Microsoft Outlook.

   ![](assets/ent-key-close-outlook-hand.png)

## Instalar {#install}

1. Execute o instalador.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Se receber um aviso de segurança, não se preocupe! Basta clicar em **Executar**.

1. Clique em **Próximo**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Preencha o **Nome**, **Sobrenome**, **Endereço de email**, em seguida, copie e cole o **Código de registro** do email para o formulário e clique em **Próximo**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Se a instalação falhar, verifique com seu departamento de TI para garantir que o tráfego HTTPS não esteja bloqueado. O instalador requer que o tráfego HTTPS seja aberto.

1. Clique em **Próximo** para instalar no local padrão.

   ![](assets/select-installation-folder-hand.png)

1. Clique em **Próximo**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Se você receber um prompt de segurança sobre um editor desconhecido, clique em **Sim**.

1. A instalação está concluída agora, clique em **Fechar**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Agora, abra o Microsoft Outlook e veja os botões do Marketo.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Excelente! Agora os botões Marketo estão em um lugar melhor.

Saiba mais sobre como usar as ações Mensagem do Marketo e Registrar com Marketo .

>[!MORELIKETHIS]
>
>* [Enviar e rastrear um email com o complemento de email do Marketo para Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md)
>* [Enviar e rastrear a partir do Outlook usando um modelo do Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md)

