---
unique-page-id: 11382829
description: Desinstalação do plug-in do Marketo Outlook pelo TI - Documentação do Marketo - Documentação do produto
title: Desinstalação do plug-in do Marketo Outlook pela TI
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '119'
ht-degree: 2%

---

# Desinstalação do plug-in do Marketo Outlook pela TI {#marketo-outlook-plugin-uninstall-by-it}

Veja como o departamento de TI pode desinstalar o plug-in do Marketo Outlook remotamente.

Execute a seguinte linha de comando como as as ‘System’ ou uma conta de usuário Administrativo com a opção /x para desinstalar.

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Para solucionar problemas, você pode ativar o registro para criar um arquivo de log de saída.

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Para especificar um local dos arquivos de log, especifique o caminho do arquivo na linha de comando.

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Exemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>Desinstalar o plug-in remotamente forçará o fechamento do Outlook no computador do usuário.

Consulte [lista completa de opções da Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) se desejar experimentar níveis de log ou níveis de interface de usuário diferentes.
