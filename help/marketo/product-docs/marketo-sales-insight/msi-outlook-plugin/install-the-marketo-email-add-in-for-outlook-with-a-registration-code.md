---
unique-page-id: 2949711
description: Instale o Suplemento de Email do Marketo para  [!DNL Outlook] com um Código de Registro - Documentação do Marketo - Documentação do produto
title: Instalar o Suplemento de Email do Marketo para  [!DNL Outlook]  com um Código de Registro
exl-id: d7a877c2-f71e-44da-b323-04f6cdb44eb0
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 6%

---

# Instalar o Suplemento de Email do Marketo para [!DNL Outlook] com um Código de Registro {#install-the-marketo-email-add-in-for-outlook-with-a-registration-code}

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

1. Identifique a sua [versão do Microsoft Outlook](https://support.office.com/en-us/article/what-version-of-outlook-do-i-have-b3a9568c-edb5-42b9-9825-d48d82b2257c){target="_blank"}.

1. Na tabela abaixo, clique no link para baixar o arquivo .ZIP apropriado para sua versão do Microsoft Outlook.

1. Descompacte o arquivo para acessar o arquivo .MSI necessário e continue com a instalação.

   >[!NOTE]
   >
   >No momento, os links abaixo estão funcionando apenas no [!DNL Microsoft Edge] ou clicando com o botão direito do mouse em [!DNL Chrome]. Lamentamos o inconveniente.

<table><thead>
  <tr>
    <th>Versão do Outlook</th>
    <th>Outlook de 32 bits</th>
    <th>Outlook de 64 bits</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Outlook 2000</td>
    <td>Não suportado</td>
    <td>N/D</td>
  </tr>
  <tr>
    <td>Outlook 2003</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Baixar</a></td>
    <td>N/D</td>
  </tr>
  <tr>
    <td>Outlook 2007</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Baixar</a></td>
    <td>N/D</td>
  </tr>
  <tr>
    <td>Outlook 2010</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Baixar</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Baixar</a></td>
  </tr>
  <tr>
    <td>Outlook 2013</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Baixar</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Baixar</a></td>
  </tr>
  <tr>
    <td>Outlook 2016</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Baixar</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Baixar</a></td>
  </tr>
  <tr>
    <td>Outlook 2019</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Baixar</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Baixar</a></td>
  </tr>
  <tr>
    <td>Outlook para Mac</td>
    <td>Não suportado</td>
    <td>Não suportado</td>
  </tr>
  <tr>
    <td>Outlook Web App</td>
    <td>Não suportado</td>
    <td>Não suportado</td>
  </tr>
  <tr>
    <td>Office 365*</td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup32.zip">Baixar</a></td>
    <td><a href="https://munchkin.marketo.net/MarketoAddInSetup64.zip">Baixar</a></td>
  </tr>
</tbody></table>

*[!DNL Office] versão 365: somente cliente [!DNL Windows] (em [!DNL Windows] 10, [!DNL Enterprise] ou [!DNL Pro]).

>[!IMPORTANT]
>
>A Microsoft lançou uma [nova versão do Outlook para Windows](https://techcommunity.microsoft.com/t5/outlook-blog/new-outlook-for-windows-now-available/ba-p/3932068){target="_blank"}. Esta nova versão não oferece suporte ao plug-in MSI Outlook existente. O plug-in MSI Outlook continuará a funcionar para áreas de trabalho do Windows que executam a versão clássica do Outlook. Para saber mais sobre o novo Outlook para Windows para organizações, [clique aqui](https://techcommunity.microsoft.com/t5/outlook-blog/the-new-outlook-for-windows-for-organization-admins/ba-p/3929169){target="_blank"}.

## Copie seu código de registro {#copy-your-registration-code}

1. Copie o código de registro do email de convite recebido.

   ![](assets/image2016-7-22-10-3a45-3a10.png)

1. Fechar [!DNL Microsoft Outlook].

   ![](assets/ent-key-close-outlook-hand.png)

## Instalar {#install}

1. Execute o instalador.

   ![](assets/image2016-7-25-10-3a23-3a33.png)

   >[!NOTE]
   >
   >Se você receber um aviso de segurança, não se preocupe! Basta clicar em **Executar**.

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/welcome-to-the-setup-wizard-hand.png)

1. Preencha **[!UICONTROL Nome]**, **[!UICONTROL Sobrenome]**, **[!UICONTROL Endereço de email]** e copie e cole o **[!UICONTROL Código de registro]** do email no formulário e clique em **[!UICONTROL Avançar]**.

   ![](assets/enter-your-information-hands.png)

   >[!TIP]
   >
   >Se a instalação falhar, verifique com o departamento de TI se o tráfego HTTPS não está bloqueado. O instalador requer que o tráfego HTTPS seja aberto.

1. Clique em **[!UICONTROL Avançar]** para instalar no local padrão.

   ![](assets/select-installation-folder-hand.png)

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/confirm-installation-hand.png)

   >[!NOTE]
   >
   >Se você receber um aviso de segurança sobre um editor desconhecido, clique em **[!UICONTROL Sim]**.

1. A instalação foi concluída, clique em **[!UICONTROL Fechar]**.

   ![](assets/image2014-9-23-15-3a52-3a11.png)

1. Agora abra [!DNL Microsoft Outlook] e veja os botões do Marketo.

   ![](assets/image2016-8-24-15-3a47-3a38.png)

   Excelente! Agora os botões do Marketo estão em um lugar melhor.

Saiba mais sobre como usar as ações Mensagem e registro do Marketo com o Marketo.

>[!MORELIKETHIS]
>
>* [Enviar e Rastrear um Email com o Suplemento de Email do Marketo para Outlook](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-an-email-with-the-email-add-in-for-outlook.md){target="_blank"}
>* [Enviar e Rastrear do Outlook Usando um Modelo do Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/send-and-track-from-outlook-using-a-marketo-template.md){target="_blank"}
