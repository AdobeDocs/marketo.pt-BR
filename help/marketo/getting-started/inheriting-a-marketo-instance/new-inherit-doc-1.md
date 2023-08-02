---
description: Herdar documento 1 - Documentação do Marketo - Documentação do produto
title: Herdar Doc 1
hide: true
hidefromtoc: true
source-git-commit: 93be928e540fd50d92bef4ead3ea23519de18cce
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 10%

---

# Herdar Doc 1 {#inherit-doc-1}

A auditoria de uma instância herdada pode parecer uma

Você herdou uma instância de Marketo Engage existente de outro administrador? Em caso afirmativo, este artigo é para você.

>[!TIP]
>
>Se você for um novo usuário de Marketo Engage e não estiver familiarizado com muitos dos termos, verifique a [Glossário do Marketo](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Usuários e funções {#users-and-roles}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Usuários</td> 
   <td><li>Há quantos usuários?</li>
<li>Há usuários que devem ser expirados?</li>
<li>Sua empresa tem políticas para excluir usuários?</li> 
<li>Quantos usuários têm permissões de administrador?</li>
<li>Algum desses usuários deve ser alterado para outras funções?</li> 
<li>Quem são os usuários da API nessa instância?</li></td>
   <td>3.1</td>
  </tr>
  <tr> 
   <td>Funções</td> 
   <td><li>Quantas funções existem?</li>  
<li>Que permissões/acesso cada função tem? Algum deve ser ajustado?</li>
<li>Há quantos usuários por função?</li>
<li>Com que frequência os usuários fazem logon?</li>
<li>Cada usuário da API tem sua própria função de usuário? Caso contrário, considere implementar isso para facilitar a solução de problemas.</li> 
<li>As suas funções e permissões de usuário estão alinhadas às suas políticas corporativas de privacidade de dados?</li></td>
   <td>3.2</td>
  </tr>
  <tr> 
   <td>Documentação interna</td> 
   <td><li>Os usuários e as funções estão claramente definidos em sua organização?</li>
<li>Qual é o seu processo para adicionar um novo usuário/administrador?</li></td>
   <td>3.3</td>
  </tr>
  <tr> 
   <td>Sandbox (se aplicável)</td> 
   <td><li>Você tem uma instância de sandbox? Em caso afirmativo, revise as categorias acima para sua sandbox.</li>
<li>A Importação de programa está vinculada à sua sandbox?</li></td>
   <td>3.4</td>
  </tr>
 </tbody> 
</table>

## Trila de auditoria {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Trila de auditoria</td> 
   <td><li>Quem está trabalhando na instância?</li></td>
   <td>3.1</td>
  </tr>
 </tbody> 
</table>

## Espaços de trabalho e partições {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Espaços de trabalho e partições</td> 
   <td><li>Quantos espaços de trabalho e/ou partições você tem?</li>
<li>Qual é o objetivo principal de cada espaço de trabalho e partição?</li>
<li>Eles precisam ser auditados ou alterados?</li>
<li>Qual é a relação entre seus espaços de trabalho e partições?</li>
<li>Quantos usuários têm acesso a cada espaço de trabalho?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Documentação interna</td> 
   <td><li>Como os espaços de trabalho e as partições são definidos?</li>
<li>Qual é o seu processo para adicionar espaços de trabalho à sua instância ou adicionar usuários a um espaço de trabalho?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Campanhas inteligentes {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Configurações da campanha inteligente</td> 
   <td><li>Você tem uma restrição no tamanho da Campanha inteligente?</li>
<li>Caso contrário, considere adicionar um. Recomendamos limitar os limites da campanha inteligente para 25% do banco de dados para evitar comunicação excessiva ou processar todo o banco de dados em workflows. Isso não apenas protege a marca, mas ajuda a proteger o desempenho da instância.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Limites de comunicação {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Limites de comunicação</td> 
   <td><li>Há limites em vigor? Sua empresa tem políticas em que os limites de comunicação podem ser necessários?</li>
<li>A Adobe recomenda limitar sua comunicação a 1 por dia e 3 por 7 dias, com emails não operacionais bloqueados.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Tags {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Tags</td> 
   <td><li>Quantas tags há? Quantas tags estão em uso? É necessário adicionar alguma?</li>
<li>As tags são necessárias em seus programas?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Canais</td> 
   <td><li>Há quantos canais? Quantas estão em uso?</li>
<li>Todos os status dos programas de canal são apropriados? Eles mostram progressão dentro do programa?</li>
<li>Seus canais estão relacionados a tipos de programas específicos?</li>
<li>Quais status são considerados bem-sucedidos para cada canal? Eles se alinham às suas metas de marketing?</li>
<li>O canal Operacional está sendo usado adequadamente?</li>
<li>Para o Advanced Report Builder (Revenue Cycle Explorer\RCE), o comportamento da análise do seu canal está definido para ser alinhado às práticas do seu programa que incorporam o custo do período?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Calendário de marketing (se aplicável)</td> 
   <td><li>Há quantos tipos de entrada de calendário? Elas ainda são relevantes?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Gerenciamento de bancos de dados {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>Gerenciamento de campos</td> 
   <td><li>Há quantos campos? Clique em "Exportar nomes de campo" para revisar uma lista de campos, campos personalizados e seus nomes de API.</li>
<li>Quantos campos personalizados há?</li>
<li>Quantos campos estão sendo usados? Selecione "Exportar usado por" no menu suspenso Ações de campo para revisar ativos relacionados de um campo.</li>
<li>Quantos são sincronizados entre o Marketo Engage e o seu CRM?</li>
<li>Os campos do CRM estão sincronizados com os objetos apropriados?</li>
<li>Há um conjunto de exibições personalizado para detalhes da pessoa? Deveria haver?</li>
<li>Você tem uma convenção de nomenclatura para seus campos com base na origem? Caso contrário, considere implementar isso.</li>
<li>Há campos bloqueados? Certifique-se de entender por que eles estão.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Atividades personalizadas</td> 
   <td><li>Há atividades personalizadas?</li>
<li>Em caso afirmativo, clique nessas atividades para entender quais atividades não estão relacionadas a um formulário, email ou página de aterrissagem do Marketo.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>objetos  personalizados</td> 
   <td><li>Quantos objetos personalizados há? Como eles são sincronizados ao seu CRM?</li>
<li>Como esses objetos personalizados estão sendo utilizados pelos seus programas e consultas de lista?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Integrações {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>CRM</td> 
   <td><li>A qual CRM você está sincronizando? Salesforce? MS Dynamics? Veeva?</li>
<li>A sincronização personalizada ou bidirecional? (KG: corrigir gramática e verificar importância)</li>
<li>[Somente Salesforce] Sua instância tem Filtros de sincronização personalizados implementados? Entre em contato com o Suporte da Marketo para identificar Filtros de sincronização personalizados ou solicitar que uma regra de sincronização personalizada seja implementada.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight (se aplicável)</td> 
   <td><li>Tem o <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">Pacote MSI instalado</a>?</li>
<li>Você <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">atualizado para a versão mais recente do Sales Insight</a>?</li>
<li>Você concluiu a configuração do Sales Insight?</li>
<li>Você <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">acesso concedido aos usuários</a> com base no número de vagas que você comprou?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Baú do tesouro {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Diversos {#miscellaneous}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar foco</th>
   <th>Coluna 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
