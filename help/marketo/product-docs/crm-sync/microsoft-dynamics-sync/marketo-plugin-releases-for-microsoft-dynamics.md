---
unique-page-id: 10099389
description: Versões de plug-in do Marketo para Microsoft Dynamics - Documentação do Marketo - Documentação do produto
title: Versões de plug-ins do Marketo para o Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 7%

---

# Versões de plug-ins do Marketo para o Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

Ao sincronizar pela primeira vez com o Microsoft Dynamics, você baixa a versão mais recente dos plug-ins para o Marketo. Periodicamente, o Marketo atualiza esses plug-ins, para que você possa retornar ao mesmo lugar para baixar a nova versão.

[Baixar o plug-in mais recente](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} correspondente à sua versão do Dynamics.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Atualização da Solução Dynamics {#updating-your-dynamics-solution}

1. Importar a versão mais recente da solução sobre a versão existente do Dynamics CRM (por exemplo: se o Dynamics CRM tiver a versão 1.4 e a versão mais recente for a 1.5, você importaria _sobre_ versão 1.4).

1. Você verá o seguinte pop-up. Selecionar **Atualizar** e **Manter personalizações** e, em seguida, clique em **Importar**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Versões mais recentes {#latest-versions}

>[!NOTE]
>
>Essas versões funcionam para versões local e online do Dynamics.

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Versão</th> 
   <th colspan="1">Data de lançamento</th> 
   <th>Observações</th> 
  </tr> 
  <tr> 
   <td colspan="1">5.0.1.1</td> 
   <td colspan="1">02/04/21</td> 
   <td colspan="1">Suporte para sincronização de campos de Conjunto de opções de seleção múltipla (esse recurso está disponível somente para a versão V9.X e posteriores). .</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">Adição de suporte para sincronização do Campaign com o MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">Adição de suporte para o processo de qualificação de lead para contato pronto para uso para o Microsoft Dynamics versão 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">Correção de erros: Erro do processo comercial ao tentar instalar as Soluções da Marketo para o Dynamics 2013.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">Correção de erros: revisão interna.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">Correção de erros: o plug-in não se inscreveu em eventos que capturavam a alteração de estado do objeto personalizado. Essa correção é específica do Dynamics CRM no local 2011. </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">Correção de erros: as atualizações da função de contato da oportunidade não foram capturadas completamente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>Correção de erros: uma transação de atualização desnecessária na função customeroportunityrole no log marketo foi anotada quando a oportunidade foi criada. </p><p>Correção de erros: uma transação de exclusão extra foi registrada ao excluir a entidade customeropportunity role.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">Correção de erros: a atualização e a exclusão de objetos personalizados se tornaram assíncronas.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">Correção de erros: quando o lead tinha um filtro de sincronização definido como NÃO, e a oportunidade e o contato não tinham um filtro de sincronização, o Log de Criação não era gerado para o contato e a oportunidade quando o lead era qualificado.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>Correção de erros: um evento Assign foi registrado quando o filtro sync estava desativado.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">Correção de erros: o cliente não pôde criar um cliente potencial no CRM porque o usuário que fez logon não tinha permissão de Configuração do Marketo.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">Correção de erros: limites de acesso criados para usuários normais do Dynamics solucionarem problemas de segurança.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>Correção de erros: as atualizações no Dynamics não estavam sendo sincronizadas com o Marketo para etapas e imagens.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">Correção de erros: os registros de cliente potencial estavam sendo sincronizados com o Marketo quando o filtro de sincronização estava definido como falso.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Baixe a solução de gerenciamento líder da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}
