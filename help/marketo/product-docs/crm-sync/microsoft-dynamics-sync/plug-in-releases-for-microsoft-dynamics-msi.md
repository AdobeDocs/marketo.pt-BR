---
unique-page-id: 10099102
description: Versões de plug-in do  [!DNL Microsoft Dynamics] MSI - Documentação do Marketo - Documentação do produto
title: Versões de plug-in para  [!DNL Microsoft Dynamics] MSI
exl-id: 830f7dc3-07fd-429b-b0fd-290ffdda88e6
feature: Microsoft Dynamics
source-git-commit: 6fb25aab33dfc0f6792950a7d5d802a9e4be8303
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Versões de plug-in para [!DNL Microsoft Dynamics] MSI {#plug-in-releases-for-microsoft-dynamics-msi}

Ao sincronizar pela primeira vez com o [!DNL Microsoft Dynamics], você baixará e instalará a versão mais recente dos plug-ins para o Marketo Sales Insight (MSI). Periodicamente, o Marketo atualiza esses plug-ins para que você possa retornar ao mesmo lugar para baixar a nova versão.

Se você estiver usando a solução de sincronização nativa do CRM da Marketo para [!DNL Dynamics], [baixe o plug-in mais recente](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md){target="_blank"} correspondente à sua versão [!DNL Dynamics]. Para aqueles que têm uma sincronização personalizada e compraram o Marketo Sales Insight, o [pacote está aqui](https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip){target="_blank"}.

>[!NOTE]
>
>Essas versões funcionam para as versões local e online do [!DNL Dynamics].

## Atualização da solução MSI {#upgrading-your-msi-solution}

1. Importe a versão mais recente da solução _sobre a versão existente_ do seu CRM [!DNL Dynamics] pressionando o botão **[!UICONTROL Importar]** no [!DNL Dynamics].

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-1.png)

>[!NOTE]
>
>Exemplo: se o seu CRM do [!DNL Dynamics] tiver a versão 2.0.0.20 e a última versão for 2.0.0.21, você importaria _sobre_ a versão 2.0.0.20.

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-2.png)

1. Selecione o **[!UICONTROL Preparo para a Atualização]** e **[!UICONTROL Manter personalizações]** e clique em **[!UICONTROL Importar]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-3.png)

1. Clique em **[!UICONTROL Avançar]**.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-4.png)

1. Após uma importação bem-sucedida, você verá duas soluções MSI: MarketoSalesInsight e MarketoSalesInsight_Upgrade. Selecione a solução mais antiga e clique em Aplicar atualização da solução.

   ![](assets/plug-in-releases-for-microsoft-dynamics-msi-5.png)

E é isso! Após a atualização, você verá apenas uma Solução MSI.

## Atualizações de versão {#version-updates}

<table>
 <tbody>
  <tr>
   <th>Data de lançamento</th>
   <th>Versão</th>
   <th>Observações</th>
  </tr>
  <tr>
   <td>14/02/24</td>
   <td>2.00.31</td>
   <td>Alterações na paginação em atividade da Web anônima.
   <p>
   Criptografar informações da chave secreta da visualização do usuário. A senha precisa ser alterada após a importação do novo pacote para que a criptografia ocorra.
   <p>
   Ao atualizar o plug-in do MSI para Dynamics, é recomendável atualizar a chave secreta da API do SOAP e as credenciais do MSI como uma forma de atualização para garantir que nenhuma permissão de acesso ocorra com o novo pacote que está sendo instalado.</td>
  </tr>
  <tr>
   <td>18/10/23</td>
   <td>2.00.30</td>
   <td>Consolidação do registro de erros MSI e remoção de notificações de informações para exibição na entidade de erro do Marketo.</td>
  </tr>
  <tr>
   <td>19/05/23</td>
   <td>2.00.29</td>
   <td>Correção de problemas de paginação de Atividade da Web e Momentos interessantes no painel global.</td>
  </tr>
  <tr>
   <td>23/03/23</td>
   <td>2.00.28</td>
   <td>Criado um <a href="https://mktg-cdn.marketo.com/community/MarketoSalesInsight_NonNative.zip">novo pacote</a> para MSI para conexões não nativas com o CRM.</td>
  </tr>
  <tr>
   <td>03/02/22</td>
   <td>2.0.0.27</td>
   <td>Layout de conta para Insights: momentos interessantes, alterações de pontuação, atividades da Web, atividades de email.</td>
  </tr>
  <tr>
   <td>05/01/22</td>
   <td>2.0.0.26</td>
   <td>Pontuação de adoção de programa para enviar email.</td>
  </tr>
  <tr>
   <td>28/10/21</td>
   <td>2.0.0.25</td>
   <td>Métricas de pontuação de adoção de produtos, novo Painel global (Atividade da Web, Email, Melhores opções).</td>
  </tr>
  <tr>
   <td>10/02/21</td>
   <td>2.0.0.22</td>
   <td>Remova a Auditoria automática ativada e as alterações na documentação na solução MSI.</td>
  </tr>
  <tr>
   <td>01/10/20</td>
   <td>2.0.0.21</td>
   <td>Correção de erros: atribuição de acesso aos campos de configuração da API MSI para usuários com a função Sales Insight.</td>
  </tr>
  <tr>
   <td>20/07/20</td>
   <td>2.0.0.20</td>
   <td>Correção de erros: adicione uma mensagem de validação para registros não sincronizados.</td>
  </tr>
  <tr>
   <td>12/06/20</td>
   <td>2.0.0.19</td>
   <td>Correção de erros: para ocultar a senha secreta MSI na configuração da API do MSD.</td>
  </tr>
  <tr>
   <td>26/05/20</td>
   <td>2.0.0.18</td>
   <td>Correção de erros: Para alterar a validação da ID de atribuição do MSI para exibir botões MSI.</td>
  </tr>
  <tr>
   <td>21/05/20</td>
   <td>2.0.0.17</td>
   <td>Correção de erros: reexiba o campo do proprietário e torne os campos não obrigatórios.</td>
  </tr>
  <tr>
   <td>28/04/20</td>
   <td>2.0.0.16</td>
   <td>Correção de erros: removendo a dependência do link de configuração do mapa de site do MSD CRM.</td>
  </tr>
 </tbody>
</table>
