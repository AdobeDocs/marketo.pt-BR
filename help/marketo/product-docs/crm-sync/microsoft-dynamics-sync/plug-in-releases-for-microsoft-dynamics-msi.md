---
unique-page-id: 10099102
description: Versões de plug-in para Microsoft Dynamics MSI - Documentos do Marketo - Documentação do produto
title: Versões de plug-in para o Microsoft Dynamics MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 5%

---

# Versões de plug-in para Microsoft Dynamics MSI {#plug-in-releases-for-microsoft-dynamics-msi}

Ao sincronizar com o Microsoft Dynamics pela primeira vez, você baixa e instala a versão mais recente dos plug-ins para Marketo Sales Insight (MSI). Periodicamente, o Marketo atualiza esses plug-ins, de modo que você pode retornar ao mesmo local para baixar a nova versão.

Por favor [baixe o plug-in mais recente](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) correspondente à sua versão do Dynamics.

>[!NOTE]
>
>Essas versões funcionam para versões locais e online do Dynamics.

## Atualizar sua solução MSI {#upgrading-your-msi-solution}

1. Importe a versão mais recente da solução _sobre a versão existente_ do seu Dynamics CRM pressionando o botão **Importar** no Dynamics.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Exemplo: se o Dynamics CRM tiver a versão 2.0.0.20 e a versão mais recente for 2.0.0.21, você importaria _sobre_ a versão 2.0.0.20.

1. Clique em **Next**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Selecione **Estágio para atualização** e **Manter personalizações** e clique em **Importar**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Clique em **Next**.

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
   <td colspan="1">1°/10/20</td> 
   <td colspan="1">2.0.0.21</td> 
   <td colspan="1">Correção de erros: Atribuir acesso aos campos de configuração da API MSI para usuários com a função Informações de vendas</td> 
  </tr> 
  <tr> 
   <td colspan="1">20/07/20</td> 
   <td colspan="1">2.0.0.20</td> 
   <td colspan="1">Correção de erros: Adicionar uma mensagem de validação para registros não sincronizados</td> 
  </tr> 
  <tr> 
   <td colspan="1">12/06/20</td> 
   <td colspan="1">2.0.0.19</td> 
   <td colspan="1">Correção de erros: Para ocultar a senha secreta MSI na configuração da API MSD</td> 
  </tr> 
  <tr> 
   <td colspan="1">26/05/20</td> 
   <td colspan="1">2.0.0.18</td> 
   <td colspan="1">Correção de erros: Alteração da validação da ID da função MSI para exibição de botões MSI</td> 
  </tr> 
  <tr> 
   <td colspan="1">21/05/20</td> 
   <td colspan="1">2.0.0.17</td> 
   <td colspan="1">Correção de erros: Mostrar campo do proprietário e tornar campos não obrigatórios</td> 
  </tr> 
  <tr> 
   <td colspan="1">28/04/20</td> 
   <td colspan="1">2.0.0.16</td> 
   <td colspan="1">Correção de erros: Removendo a dependência de link da configuração do mapa de site do MSD CRM</td> 
  </tr> 
 </tbody> 
</table>
