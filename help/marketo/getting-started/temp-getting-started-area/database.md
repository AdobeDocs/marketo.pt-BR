---
description: Configuração da seção Banco de Dados para uma nova instância de Marketo Engage.
title: NOVO BANCO DE DADOS DE ÁREA
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: 1966bc6f-9384-4c51-b3aa-57d5e52781f1
source-git-commit: 14ccfe39059b9c900a5e5e00b082146bb500d79d
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 10%

---

# NOVA ÁREA: Lista de Verificação do Banco de Dados {#new-area-database-checklist}

Saiba como implementar as etapas necessárias para a seção Banco de dados na nova instância do Marketo Engage. Siga os guias &quot;Implementar uma nova instância&quot; e acompanhe as tarefas em andamento para ajudar você a configurar sua instância para obter eficiência a longo prazo.

## Listas inteligentes do sistema {#system-smart-lists}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Todas as pessoas</td>
    <td><li>Determine a implementação de uma sincronização 1:1 com o CRM ou a aplicação de filtros para limitar quem se move de um sistema para outro e quando.</li> 
    <li>Revise o número total de pessoas e pessoas comercializáveis em seu <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html" target="_blank" rel="noopener noreferrer">banco de dados</a>.</li></td>
  </tr>
  <tr>
    <td>Lista de bloqueios</td>
    <td><li>Definir critérios de inclui na lista de bloqueios. Considere adicionar domínios do concorrente a <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank" rel="noopener noreferrer">➡ incluir na lista de bloqueios</a> para impedir que recebam emails de marketing e operacionais.</li></td>
  </tr>
  <tr>
    <td>Campanha de marketing suspensa</td>
    <td><li>Definir <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html#marketing-suspended" target="_blank" rel="noopener noreferrer">Marketing suspenso</a> critérios.</li></td>
  </tr>
  <tr>
    <td>Endereços de e-mail com mensagens devolvidas </td>
    <td><li>Defina seus critérios para Endereços de email devolvidos.</li>
    <li>Revise as pessoas na categoria Email inválido e se seus emails precisam ser <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank" rel="noopener noreferrer">redefinir manualmente</a>.</li></td>
  </tr>
  <tr>
    <td>Possíveis duplicatas</td>
    <td><li>Revise Pessoas na lista Duplicatas possíveis.</li> 
    <li>Defina sua estratégia de gerenciamento de duplicatas para determinar <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank" rel="noopener noreferrer">mesclando pessoas manualmente</a> ou não.</li>  
    <li>Se você tiver uma integração com o CRM, defina um processo e contabilize para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html#effect-in-salesforce" target="_blank" rel="noopener noreferrer">o efeito da mesclagem de leads no CRM</a>.</li></td>
  </tr>
  <tr>
    <td>Nenhum programa de aquisição</td>
    <td><li>Estabeleça campanhas em seus modelos de programas que definem o Programa de aquisição, especialmente se estiver usando formulários globais.</li></td>
  </tr>
  <tr>
    <td>Pessoas com inscrição cancelada</td>
    <td><li>Revise seus critérios para <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html" target="_blank" rel="noopener noreferrer">Pessoas Não Inscritas</a>.</li></td>
  </tr>
</tbody>
</table>

## Agrupar listas inteligentes {#group-smart-lists}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Agrupar listas inteligentes</td>
    <td><li>Esteja ciente de criar listas inteligentes de grupo para que não haja listas duplicadas.</li>
    <li>Rastreie as listas mestras aqui no banco de dados.</li></td>
  </tr>
</tbody>
</table>

## Segmentação {#segmentation}

<table>
<thead>
  <tr>
    <th>Área</th>
    <th>Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentação</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html" target="_blank" rel="noopener noreferrer">Criar segmentações</a> com base nas necessidades da sua empresa. Cada assinatura é limitada a 20 segmentações e 100 segmentos em cada segmentação.</li></td>
  </tr>
</tbody>
</table>
