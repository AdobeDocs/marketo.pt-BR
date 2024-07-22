---
description: Configure a seção Banco de Dados para sua nova instância do Marketo Engage.
title: Novas Práticas Recomendadas da Instância - Lista de Verificação do Banco de Dados
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
source-git-commit: df8087dbaf2b621d0d877eba1c16f160ee9bf460
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 9%

---

# Novas Práticas Recomendadas da Instância: Lista de Verificação do Banco de Dados {#new-instance-best-practices-database-checklist}

A seção Banco de dados é onde você encontrará os principais atributos das pessoas na sua instância. Saiba mais sobre as etapas necessárias para navegar pelas diferentes listas e segmentações no banco de dados, bem como gerenciar registros de pessoas.

Lembre-se de [baixar as listas de verificação](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) e acompanhar seu progresso.

## Listas inteligentes do sistema {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Todas as pessoas</td>
    <td><li>Determine a implementação de uma sincronização 1:1 com seu CRM ou a aplicação de filtros para limitar quem se move de um sistema para outro e quando.</li> 
    <li>Revise o número total de pessoas e pessoas comercializáveis no seu <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html" target="_blank">banco de dados de Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Lista de bloqueios</td>
    <td><li>Definir critérios de inclui na lista de bloqueios. Considere adicionar domínios do concorrente ao seu <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank">incluo na lista de bloqueios do</a> para impedir que eles recebam qualquer um de seus emails.</li></td>
  </tr>
  <tr>
    <td>Campanha de marketing suspensa</td>
    <td><li>Defina os critérios de <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">Marketing Suspenso</a>.</li></td>
  </tr>
  <tr>
    <td>Endereços de e-mail com mensagens devolvidas </td>
    <td><li>Defina seus critérios para endereços de email devolvidos.</li>
    <li>Revise as pessoas na categoria "Email inválido" e determine se seus emails precisam ser <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank">redefinidos manualmente</a>.</li></td>
  </tr>
  <tr>
    <td>Possíveis duplicatas</td>
    <td><li>Revise Pessoas na lista Duplicatas possíveis.</li> 
    <li>Defina sua estratégia de gerenciamento de duplicatas para determinar se deseja <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank">mesclar pessoas manualmente</a>.</li>  
    <li>Se você tiver uma integração com o CRM, defina um processo e uma conta para <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">o efeito da mesclagem de clientes potenciais no seu CRM</a>.</li></td>
  </tr>
  <tr>
    <td>Nenhum programa de aquisição</td>
    <td><li>Estabeleça campanhas em seus modelos de programas que definem um Programa de aquisição, especialmente se estiver usando formulários globais.</li></td>
  </tr>
  <tr>
    <td>Pessoas com inscrição cancelada</td>
    <td><li>Revise seus critérios para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html" target="_blank">pessoas que cancelaram sua assinatura</a>.</li></td>
  </tr>
</tbody>
</table>

## Agrupar listas inteligentes {#group-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Agrupar listas inteligentes</td>
    <td><li>Esteja ciente de criar listas inteligentes de grupo para que não haja listas duplicadas.</li>
    <li>Rastreie as listas mestras no banco de dados.</li></td>
  </tr>
</tbody>
</table>

## Segmentação {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:21%">Área</th>
    <th style="width:79%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentação</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html" target="_blank">Crie segmentações</a> com base nas necessidades da sua empresa. Cada assinatura é limitada a 20 segmentações e 100 segmentos em cada segmentação.</li></td>
  </tr>
</tbody>
</table>
