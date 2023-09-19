---
description: Lista de verificação do banco de dados da instância herdada - Documentação do Marketo - Documentação do produto
title: Lista de Verificação do Banco de Dados da Instância Herdada
hide: true
hidefromtoc: true
source-git-commit: 0d6507c251e2b7567483af8d75158f6bc6a1ca49
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 7%

---

# Instância Herdada: Lista de Verificação do Banco de Dados {#inherited-instance-database-checklist}

Entenda o número total de pessoas, pessoas comercializáveis e as principais fontes de aquisição de pessoas na sua assinatura.

## Listas inteligentes do sistema {#system-smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th> 
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Todas as pessoas</td> 
   <td><li>Quantas pessoas existem na <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">banco de dados</a>?</li>
<li>Se o banco de dados estiver quase cheio, a política da empresa recomenda expandir o tamanho do banco de dados ou limpar os dados históricos?</li>
<li>Seu banco de dados geral é no mínimo 85% comercializável? 
<br/>     Se o seu estiver abaixo desse limite, verifique as outras listas inteligentes do sistema (Inclui na lista de bloqueios, Marketing suspenso, Duplicatas, Cancelar inscrição) com mais escrutínio.</li></td>
  </tr>
  <tr> 
   <td>Pessoas que cancelaram a inscrição</td> 
   <td><li>Quais são seus critérios para <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">pessoas não inscritas</a>? Há muitas pessoas não inscritas?</li>
<li>Os métodos de cancelamento de inscrição estão alinhados aos requisitos de privacidade de dados?</li>
<li>Sua preferência de cancelamento de inscrição está atualizada? Por quanto tempo os registros permaneceram no banco de dados como não comercializáveis?</li></td>
  </tr>
  <tr> 
   <td>Marketing suspenso</td> 
   <td><li>Quais são seus critérios para <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">Marketing suspenso</a>? Há pessoas demais com suspensão de marketing?</li>
<li>Por quanto tempo os registros permaneceram no status Marketing Suspenso?</li>
<p>Exemplo de caso de uso de suspensão de marketing: registros de pessoas que estão ativamente envolvidas com vendas em oportunidades de estágio avançado para as quais você deseja suprimir comunicações de marketing.</td>
  </tr>
   <tr> 
   <td>Lista de bloqueios</td> 
   <td><li>Quais são seus critérios para <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">➡ registros de incluir na lista de bloqueios</a>? Incluir na lista de bloqueios Há pessoas demais que são revoltadas?</li></td>
  </tr>
  <tr> 
   <td>Endereços de email com mensagens rejeitadas</td> 
   <td><li>Você tem um monte de <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">pessoas que rejeitaram</a> no banco de dados?
   <br/>     Em caso afirmativo, considere investigar o motivo.</li></td></li></td>
  </tr>
  <tr> 
   <td>Possíveis duplicatas</td> 
   <td><li>Quantas <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">registros possivelmente duplicados</a> existem?
   <br/>     Considere excluí-los ou mesclá-los.</li></td>
  </tr>
   <tr> 
   <td>Nenhum programa de aquisição</td> 
   <td><li>Quantas pessoas não têm um <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">programa de aquisição</a>?
   <br/>     Se há muito, considere investigar o porquê.</li></td>
  </tr>
 </tbody> 
</table>

## Listas inteligentes {#smart-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th> 
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Listas inteligentes</td> 
   <td><li>Quantas <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">Smart Lists</a> existem? Como eles são usados nessa instância?</li>
   <p><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: Na seção Banco de Dados, as Smart Lists de Grupo são geradas pelo usuário e as Smart Lists de Sistema são listas default criadas por Marketo Engage.
<li>As listas estão organizadas em uma estrutura de pastas coesa? 
<br/>     Se você tiver listas órfãs, considere organizar sua árvore para que os ativos sejam fáceis de encontrar.</li>
<p><img src="assets/tip-icon.png" alt="ícone de dica">DICA: <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">Arquivamento</a> As Smart Lists desnecessárias ajudarão na organização e no desempenho.</td>
  </tr>
 </tbody> 
</table>

## Listas estáticas {#static-lists}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th> 
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Listas estáticas</td> 
   <td><li>Quantas <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">Listas Estáticas</a> existem? Como eles são usados nessa instância?</li>
   <p><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: Na seção Banco de Dados, Listas de Grupos são Listas Estáticas.</td>
  </tr>
 </tbody> 
</table>

## Segmentações {#segmentations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:20%">Área</th> 
   <th>Revisar foco</th>
  </tr> 
  <tr> 
   <td>Segmentações</td> 
   <td><li>Qual <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">segmentações</a> existem? Como eles estão sendo usados?</li>
<li>Há muitas pessoas em <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">segmentos padrão</a>?</li>
<li>Há uma segmentação para o público comercializável? 
<br/>     Caso contrário, considere a criação de um.</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[► Auditoria de uma instância herdada: Administrador](/help/marketo/getting-started/inheriting-a-marketo-instance/admin-section-checklist.md)

[Auditoria de uma instância herdada: Atividades de marketing ►](/help/marketo/getting-started/inheriting-a-marketo-instance/marketing-activities-checklist.md)
