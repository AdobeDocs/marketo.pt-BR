---
unique-page-id: 11382829
description: Desinstalação de plug-in do Marketo Outlook por TI - Documentos do Marketo - Documentação do produto
title: Desinstalação de plug-in do Marketo Outlook por TI
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 2%

---

# Desinstalação de plug-in do Marketo Outlook por TI {#marketo-outlook-plugin-uninstall-by-it}

Veja como a TI pode desinstalar o plug-in do Marketo Outlook remotamente.

Execute a linha de comando a seguir como &quot;Sistema&quot; ou uma conta de usuário Administrativo com o switch /x para desinstalar.

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Para solução de problemas, você pode habilitar o registro para criar um arquivo de log de saída.

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Para especificar um local dos arquivos de log, você pode especificar o caminho do arquivo na linha de comando.

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>Desinstalar o plug-in remotamente fechará o Outlook na máquina do usuário.

Consulte [Lista completa de switches da Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) se quiser tentar níveis de log diferentes ou níveis de interface do usuário.
