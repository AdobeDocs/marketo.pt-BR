---
unique-page-id: 11382815
description: Instalação do Marketo [!DNL Outlook] Plugin pela TI - Documentação da Marketo - Documentação do produto
title: Instalação do Marketo [!DNL Outlook] Plugin pela TI
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 1%

---

# Instalação do plug-in do Marketo [!DNL Outlook] pela TI {#marketo-outlook-plugin-installation-by-it}

Às vezes, as políticas corporativas exigem que sua equipe de TI instale todos os softwares nos computadores de seus funcionários. Nesses casos, a TI geralmente faz isso remotamente usando seu próprio software de implantação. Este documento fornece as linhas de comando que você usaria como entradas durante o processo de implantação para instalar remotamente o plug-in do Outlook.

>[!PREREQUISITES]
>
>[Configurar](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) a Chave da Empresa.

Execute a seguinte linha de comando como &#39;System&#39; ou uma conta de usuário Administrativo com a opção /i para instalar.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Para solucionar problemas, você pode ativar o registro para criar um arquivo de log de saída.

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Para especificar um local dos arquivos de log, especifique o caminho do arquivo na linha de comando.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>O local de armazenamento do arquivo de log deve existir ou a instalação será anulada.

Consulte [a lista completa de opções da Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) se desejar experimentar níveis de log ou níveis de interface de usuário diferentes.

>[!MORELIKETHIS]
>
>[Desinstalação de Plug-in do Marketo [!DNL Outlook] pela TI](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
