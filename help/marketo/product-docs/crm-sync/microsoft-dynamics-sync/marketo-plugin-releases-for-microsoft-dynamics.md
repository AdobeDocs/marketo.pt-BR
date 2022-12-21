---
unique-page-id: 10099389
description: Versões de plug-in do Marketo para Microsoft Dynamics - Documentos do Marketo - Documentação do produto
title: Versões de plug-in do Marketo para o Microsoft Dynamics
exl-id: c9c25e11-bcf7-49bf-920a-4182af27d278
source-git-commit: 1379fcbdc0a8673b1d6cb17a9d573d3625d5a1b8
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 7%

---

# Versões de plug-in do Marketo para o Microsoft Dynamics {#marketo-plugin-releases-for-microsoft-dynamics}

Ao sincronizar com o Microsoft Dynamics pela primeira vez, você baixa a versão mais recente dos plug-ins do Marketo. Periodicamente, o Marketo atualiza esses plug-ins, de modo que você pode retornar ao mesmo local para baixar a nova versão.

[Baixe o plug-in mais recente](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) correspondente à sua versão do Dynamics.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-1.png)

## Atualização da sua solução do Dynamics {#updating-your-dynamics-solution}

1. Importe a versão mais recente da solução pela versão existente do Dynamics CRM (por exemplo: se o Dynamics CRM tiver a versão 1.4 e a versão mais recente for 1.5, você importaria _over_ versão 1.4).

1. Você verá o seguinte pop-up. Selecionar **Atualizar** e **Manter personalizações**, depois clique em **Importar**.

![](assets/marketo-plugin-releases-for-microsoft-dynamics-2.png)

## Versões mais recentes {#latest-versions}

>[!NOTE]
>
>Essas versões funcionam para versões locais e online do Dynamics.

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
   <td colspan="1">Suporte para sincronização de campos Multiselect Optionset (esse recurso está disponível somente para V9.X e superior). .</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.2.0.0</td> 
   <td colspan="1">10/16/20</td> 
   <td colspan="1">Adição de Suporte para Sincronização do Campaign com o MS Dynamics.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.24</td> 
   <td colspan="1">8/22/18</td> 
   <td colspan="1">Adição de suporte para lead pronto para uso para o processo de contato do Microsoft Dynamics versão 9.x.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.23</td> 
   <td colspan="1">6/27/18</td> 
   <td colspan="1">Correção de erros: Erro no processo de negócios ao tentar instalar as soluções da Marketo para o Dynamics 2013.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.22</td> 
   <td colspan="1">9/29/17</td> 
   <td colspan="1">Correção de erros: Revisão interna.</td> 
  </tr> 
  <tr> 
   <td colspan="1"><p>4.0.0.21</p></td> 
   <td colspan="1">11/9/16</td> 
   <td colspan="1">Correção de erros: O plug-in não assinou eventos que capturam a alteração de estado do objeto personalizado. Essa correção é específica do Dynamics CRM On Premise 2011. </td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.20</td> 
   <td colspan="1">7/22/16</td> 
   <td colspan="1">Correção de erros: As atualizações da função de contato da oportunidade não foram capturadas completamente.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.19</td> 
   <td colspan="1">6/28/16</td> 
   <td colspan="1"><p>Correção de erros: Uma transação de atualização desnecessária na função de oportunidade do cliente no log de marketing foi anotada quando a oportunidade foi criada. </p><p>Correção de erros: Uma transação de exclusão extra foi registrada ao excluir a entidade customeroportunityrole.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.18</td> 
   <td colspan="1">5/31/16</td> 
   <td colspan="1">Correção de erros: Atualização e exclusão de objetos personalizados assíncronos.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.17</td> 
   <td colspan="1">4/8/16</td> 
   <td colspan="1">Correção de erros: Quando o lead tinha um filtro de sincronização definido como NO e a oportunidade e o contato não tinham um filtro de sincronização, o log de criação não era gerado para o contato e a oportunidade quando o lead era qualificado.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.16</td> 
   <td colspan="1">3/29/16</td> 
   <td>Correção de erros: Um evento Atribuir foi registrado quando o filtro de sincronização foi desativado.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.15</td> 
   <td colspan="1">3/3/16</td> 
   <td colspan="1">Correção de erros: O cliente não pôde criar um lead no CRM porque o usuário de logon não tinha permissão de Configuração do Marketo.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.14</td> 
   <td colspan="1">1/18/16</td> 
   <td colspan="1">Correção de erros: Limites de acesso criados para usuários normais do Dynamics para lidar com questões de segurança.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.13</td> 
   <td colspan="1">12/30/15</td> 
   <td>Correção de erros: As atualizações no Dynamics não estavam sincronizando o Marketo para etapas e imagens.</td> 
  </tr> 
  <tr> 
   <td colspan="1">4.0.0.12</td> 
   <td colspan="1">11/12/15</td> 
   <td colspan="1">Correção de erros: Os registros de lead estavam sincronizando com o Marketo quando o filtro de sincronização estava definido como falso.</td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Baixe a solução de gerenciamento de clientes potenciais da Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)
