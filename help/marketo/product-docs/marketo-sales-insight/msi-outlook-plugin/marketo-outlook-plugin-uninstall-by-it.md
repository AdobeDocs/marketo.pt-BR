---
unique-page-id: 11382829
description: Saiba como o departamento de TI pode desinstalar o plug-in do Marketo Outlook. Remova o suplemento dos computadores dos usuários quando necessário.
title: Desinstalação do Marketo [!DNL Outlook] Plugin pela TI
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/p2CjKHycrJRHLpphyn2qsUEKP-dWh2OlTezwrOn9Ljw
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 2%

---

# Desinstalação do plug-in do Marketo [!DNL Outlook] pela TI {#marketo-outlook-plugin-uninstall-by-it}

Veja como o departamento de TI pode desinstalar o Plug-in [!DNL Outlook] do Marketo remotamente.

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
>Desinstalar o plug-in remotamente forçará o fechamento de [!DNL Outlook] no computador do usuário.

Consulte [lista completa de opções da Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) se desejar experimentar níveis de log ou níveis de interface de usuário diferentes.
