---
unique-page-id: 11382815
description: Saiba como o departamento de TI pode instalar o plug-in do Marketo Outlook para a organização. Implante o suplemento em escala para usuários do Outlook.
title: Instalação do Marketo [!DNL Outlook] Plugin pela TI
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/7Gq4FJlVf9jvqL2Bz34oQVL8HtBNYCjEHl32g-0RXYk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 195
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
