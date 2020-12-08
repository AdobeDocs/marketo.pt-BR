---
unique-page-id: 11382829
description: Desinstalação do plug-in do Marketo Outlook por TI - Documentos do Marketing - Documentação do produto
title: Desinstalação do plug-in do Marketo Outlook por TI
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Desinstalação do plug-in do Marketo Outlook por TI {#marketo-outlook-plugin-uninstall-by-it}

Veja como a TI pode desinstalar remotamente o plug-in do Marketo Outlook.

Execute a seguinte linha de comando como &quot;Sistema&quot; ou uma conta de usuário administrativo com a opção /x para desinstalar.
`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Exemplo**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Para solucionar problemas, você pode ativar o registro para criar um arquivo de log de saída.  `<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemplo**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Para especificar um local dos arquivos de log, você pode especificar o caminho do arquivo na linha de comando.  `<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemplo**
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>Desinstalar o plug-in remotamente fechará o Outlook com força na máquina do usuário.

Consulte a lista completa de switches [da](https://support.microsoft.com/en-us/kb/227091) Microsoft se você quiser tentar níveis de log ou níveis de interface do usuário diferentes.