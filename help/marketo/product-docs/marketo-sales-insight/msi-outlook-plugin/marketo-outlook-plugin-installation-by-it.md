---
unique-page-id: 11382815
description: Instalação do plug-in do Marketo Outlook por TI - Documentos do Marketing - Documentação do produto
title: Instalação do plug-in do Marketo Outlook por TI
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Instalação do plug-in do Marketo Outlook por TI {#marketo-outlook-plugin-installation-by-it}

Às vezes, as políticas corporativas exigem que sua equipe de TI instale todo o software nos computadores dos funcionários. Nesses casos, a TI costuma fazer isso remotamente usando seu próprio software de implantação. Este doc fornece as linhas de comando que você usaria como entradas durante o processo de implantação para instalar remotamente o plug-in do Outlook.

>[!PREREQUISITES]
>
>[Configure ](http://docs.marketo.com/display/DOCS/Install+the+Marketo+Add-in+for+Outlook+with+an+Enterprise+Key) a chave corporativa.

Execute a seguinte linha de comando como &quot;Sistema&quot; ou uma conta de usuário administrativo com a opção /i a ser instalada.  `<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemplo**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Para solucionar problemas, você pode ativar o registro para criar um arquivo de registro de saída.  `<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemplo**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Para especificar um local dos arquivos de log, você pode especificar o caminho do arquivo na linha de comando.  `<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Exemplo**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>O local do armazenamento do arquivo de log deve existir ou a instalação será abortada.

Consulte [a lista completa de switches](https://support.microsoft.com/en-us/kb/227091) da Microsoft se você quiser tentar níveis de log ou níveis de interface do usuário diferentes.

>[!NOTE]
>
>**Artigos relacionados**
>
>[Desinstalação do plug-in do Marketo Outlook por TI](marketo-outlook-plugin-uninstall-by-it.md)

