---
unique-page-id: 10099389
description: Versões de plug-in do Marketo para  [!DNL Microsoft Dynamics]  - Documentação do Marketo - Documentação do produto
title: Versões de plug-in do Marketo para  [!DNL Microsoft Dynamics]
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---

# Versões de plug-ins do Marketo para [!DNL Microsoft Dynamics] {#marketo-plugin-releases-for-microsoft-dynamics}

Ao sincronizar pela primeira vez com o [!DNL Microsoft Dynamics], você baixará a versão mais recente dos plug-ins para o Marketo. Periodicamente, o Marketo atualiza esses plug-ins, para que você possa retornar ao mesmo lugar para baixar a nova versão.

[Baixe o plug-in mais recente](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) correspondente à sua versão [!DNL Dynamics].

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Atualizando sua Solução [!DNL Dynamics] {#updating-your-dynamics-solution}

1. Importe a versão mais recente da solução sobre a versão existente do seu [!DNL Dynamics] CRM (por exemplo: se o seu [!DNL Dynamics] CRM tiver a versão 1.4 e a versão mais recente for a 1.5, você importaria _sobre_ a versão 1.4).

1. Você verá o seguinte pop-up. Selecione **Atualizar** e **Manter personalizações** e clique em **Importar**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Versões mais recentes {#latest-versions}

>[!NOTE]
>
>Essas versões funcionam para as versões local e online do [!DNL Dynamics].

<table> 
 <tbody> 
  <tr> 
   <th style="width:15%">Versão</th> 
   <th style="width:20%">Data de lançamento</th> 
   <th style="width:65%">Observações</th> 
  </tr>
  <tr> 
   <td>5.0.2.1</td> 
   <td>19/01/24</td> 
   <td>Correção de erros: foram corrigidos erros relacionados à sincronização de entidades personalizadas.</td> 
  </tr> 
  <tr> 
   <td>5.0.2.0</td> 
   <td>24/03/23</td> 
   <td>Correção de erros: correção de erros que impediam a mesclagem de contatos no MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">16/10/20</td> 
   <td colspan="1">Adição de Suporte para Sincronização de Campanha com MS [!DNL Dynamics].</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">22/08/18</td> 
   <td colspan="1">Adição de suporte para o processo de qualificação de lead para contato pronto para [!DNL Microsoft Dynamics] Versão 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">27/06/18</td> 
   <td colspan="1">Correção de erros: Erro do Processo Comercial ao tentar instalar as Soluções da Marketo para [!DNL Dynamics] 2013.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.24</td> 
   <td>22/08/18</td> 
   <td>Adição de suporte para o processo de qualificação de lead para contato pronto para uso para o Microsoft Dynamics versão 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">09/11/16</td> 
   <td colspan="1">Correção de erros: o plug-in não se inscreveu em eventos que capturavam a alteração de estado do objeto personalizado. Esta correção é específica para o [!DNL Dynamics] CRM On Premise 2011. </td> 
  </tr> 
  <tr> 
   <td>4.0.0.22</td> 
   <td>29/09/17</td> 
   <td>Correção de erros: revisão interna.</td> 
  </tr> 
  <tr> 
   <td><p>4.0.0.21</p></td> 
   <td>09/11/16</td> 
   <td>Correção de erros: o plug-in não se inscreveu em eventos que capturavam a alteração de estado do objeto personalizado. Essa correção é específica do Dynamics CRM no local 2011.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.20</td> 
   <td>22/07/16</td> 
   <td>Correção de erros: as atualizações da função de contato da oportunidade não foram capturadas completamente.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.19</td> 
   <td>28/06/16</td> 
   <td>Correção de erros: uma transação de atualização desnecessária na função customeroportunityrole no log marketo foi anotada quando a oportunidade foi criada.<p>Correção de erros: uma transação de exclusão extra foi registrada ao excluir a entidade customeropportunity role.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.18</td> 
   <td>31/05/16</td> 
   <td>Correção de erros: a atualização e a exclusão de objetos personalizados se tornaram assíncronas.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.17</td> 
   <td>08/04/16</td> 
   <td>Correção de erros: quando o lead tinha um filtro de sincronização definido como NÃO, e a oportunidade e o contato não tinham um filtro de sincronização, o Log de Criação não era gerado para o contato e a oportunidade quando o lead era qualificado.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.16</td> 
   <td>29/03/16</td> 
   <td>Correção de erros: um evento Assign foi registrado quando o filtro sync estava desativado.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.15</td> 
   <td>03/03/16</td> 
   <td>Correção de erros: o cliente não pôde criar um cliente potencial no CRM porque o usuário que fez logon não tinha permissão de Configuração do Marketo.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">18/01/16</td> 
   <td colspan="1">Correção de erros: limites de acesso criados para usuários normais do [!DNL Dynamics] para resolver problemas de segurança.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">30/12/15</td> 
   <td>Correção de erros: as atualizações no [!DNL Dynamics] não estavam sendo sincronizadas com o Marketo para etapas e imagens.</td> 
  </tr> 
  <tr> 
   <td>4.0.0.12</td> 
   <td>12/11/15</td> 
   <td>Correção de erros: os registros de cliente potencial estavam sendo sincronizados com o Marketo quando o filtro de sincronização estava definido como falso.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Baixar a Solução Marketo de Gerenciamento de Clientes Potenciais](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
