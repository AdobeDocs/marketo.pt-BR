---
unique-page-id: 11382815
description: Instalação do plug-in do Marketo Outlook por TI - Documentos do Marketing - Documentação do produto
title: Instalação do plug-in do Marketo Outlook por TI
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---


# Instalação do plug-in do Marketo Outlook por TI {#marketo-outlook-plugin-installation-by-it}

Às vezes, as políticas corporativas exigem que sua equipe de TI instale todo o software nos computadores dos funcionários. Nesses casos, a TI costuma fazer isso remotamente usando seu próprio software de implantação. Este doc fornece as linhas de comando que você usaria como entradas durante o processo de implantação para instalar remotamente o plug-in do Outlook.

>[!PREREQUISITES]
>
>[Configure ](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) a chave corporativa.

Execute a seguinte linha de comando como &quot;Sistema&quot; ou uma conta de usuário administrativo com a opção /i a ser instalada.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Para solucionar problemas, você pode ativar o registro para criar um arquivo de registro de saída.

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Para especificar um local dos arquivos de log, você pode especificar o caminho do arquivo na linha de comando.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>O local do armazenamento do arquivo de log deve existir ou a instalação será abortada.

Consulte [a lista completa de switches](https://support.microsoft.com/en-us/kb/227091) da Microsoft se você quiser tentar níveis de log ou níveis de interface do usuário diferentes.

>[!MORELIKETHIS]
>
>[Desinstalação do plug-in do Marketo Outlook por TI](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
