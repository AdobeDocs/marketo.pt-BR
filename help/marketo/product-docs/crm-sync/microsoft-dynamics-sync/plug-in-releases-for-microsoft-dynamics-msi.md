---
unique-page-id: 10099102
description: Versões de plug-in do Microsoft Dynamics MSI - Documentação do Marketo - Documentação do produto
title: Versões de plug-in do MSI do Microsoft Dynamics
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 8%

---

# Versões de plug-in do MSI do Microsoft Dynamics {#plug-in-releases-for-microsoft-dynamics-msi}

Ao sincronizar pela primeira vez com o Microsoft Dynamics, você baixa e instala a versão mais recente dos plug-ins para o Marketo Sales Insight (MSI). Periodicamente, o Marketo Engage atualiza esses plug-ins para que você possa retornar ao mesmo lugar para baixar a nova versão.

Se você estiver usando a solução de sincronização do CRM nativa da Marketo para o Dynamics, [baixar o plug-in mais recente](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} corresponding to your Dynamics release. For those who have a custom sync and have purchased Marketo Sales Insight, the [package is here](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>Essas versões funcionam para versões local e online do Dynamics.

## Atualização da solução MSI {#upgrading-your-msi-solution}

1. Importar a versão mais recente da solução _sobre a versão existente_ do seu Dynamics CRM pressionando o botão **[!UICONTROL Importar]** botão no Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Exemplo: se seu Dynamics CRM tiver a versão 2.0.0.20 e a versão mais recente for 2.0.0.21, você importaria _sobre_ versão 2.0.0.20.

1. Clique em **[!UICONTROL Próximo]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Selecionar **[!UICONTROL Estágio para atualização]** e **[!UICONTROL Manter personalizações]** e, em seguida, clique em **[!UICONTROL Importar]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Clique em **[!UICONTROL Próximo]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Após uma importação bem-sucedida, você verá duas soluções MSI: MarketoSalesInsight e MarketoSalesInsight_Upgrade. Selecione a solução mais antiga e clique em Aplicar atualização da solução.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

E é isso! Após a atualização, você verá apenas uma Solução MSI.

## Atualizações de versão {#version-updates}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th colspan="1">Data de lançamento</th> 
   <th colspan="1">Versão</th> 
   <th colspan="1">Observações</th> 
  </tr> 
  <tr> 
   <td colspan="1">02/03/22</td> 
   <td colspan="1">2.0.0.27</td> 
   <td colspan="1">Layout de conta para Insights: momentos interessantes, alterações de pontuação, atividades da Web, atividades de email</td> 
  </tr>
  <tr> 
   <td colspan="1">01/05/22</td> 
   <td colspan="1">2.0.0.26</td> 
   <td colspan="1">Pontuação de adoção de programa para enviar email</td> 
  </tr>
  <tr> 
   <td colspan="1">10/28/21</td> 
   <td colspan="1">2.0.0.25</td> 
   <td colspan="1">Métricas de pontuação de adoção de produtos, novo Painel global (Atividade da Web, Email, Melhores opções)</td> 
  </tr>
  <tr> 
   <td colspan="1">02/10/21</td> 
   <td colspan="1">2.0.0.22</td> 
   <td colspan="1">Remoção da Auditoria automática ativada e alterações na documentação da solução MSI</td> 
  </tr>
  <tr> 
   <td colspan="1">10/01/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">Correção de erros: atribuição de acesso aos campos de configuração da API MSI para usuários com a função Sales Insight</td> 
  </tr> 
  <tr> 
   <td colspan="1">07/20/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">Correção de erros: adicionar uma mensagem de validação para registros não sincronizados</td> 
  </tr> 
  <tr> 
   <td colspan="1">06/12/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">Correção de erros: para ocultar a senha secreta MSI na configuração da API MSD</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/26/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">Correção de erros: Para alterar a validação da ID de atribuição do MSI para exibir botões do MSI</td> 
  </tr> 
  <tr> 
   <td colspan="1">05/21/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">Correção de erros: reexiba o campo do proprietário e torne os campos não obrigatórios</td> 
  </tr> 
  <tr> 
   <td colspan="1">04/28/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">Correção de erros: Remoção da dependência do link de configuração do mapa de site do CRM MSD</td> 
  </tr> 
 </tbody> 
</table>
