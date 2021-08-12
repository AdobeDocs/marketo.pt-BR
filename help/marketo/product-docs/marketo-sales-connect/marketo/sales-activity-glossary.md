---
description: Glossário de atividades de vendas - Documentos da Marketo - Documentação do produto
title: Glossário de atividades de vendas
hide: true
hidefromtoc: true
source-git-commit: 70f17106efe52ee742c8e31013e533fc36ce9835
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 17%

---

# Glossário de atividades de vendas {#sales-activity-glossary}

Em Sales Connect, quando um vendedor: adiciona um lead a uma cadência de vendas, envia um email ou faz uma chamada uma atividade. Ele será registrado no histórico de atividades do Marketo. Além disso, quando o cliente potencial interage com emails, aberturas, cliques e respostas também são registrados em log.

As atividades abaixo serão registradas no Marketo pelo Sales Connect.

>[!NOTE]
>
>Essas atividades e atributos estão disponíveis para consumo a partir de nossa REST e API em massa.

## Atividades {#activities}

<table>
 <tr>
  <th>Atividade de vendas</th>
  <th>Atributo</th>
 </tr>
 <tr>
  <th rowspan="3">Enviar e-mail de vendas</th>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID do modelo</td>
 </tr>
 <tr>
  <th rowspan="3">Abrir e-mail de vendas</th>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID do modelo</td>
 </tr>
 <tr>
  <th rowspan="4">Email de vendas clicado</th>
  <td>Link</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID do modelo</td>
 </tr>
 <tr>
  <th rowspan="2">Email de Vendas Recebido</th>
  <td>Recebido por</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <th rowspan="4">E-mail de vendas foi devolvido</th>
  <td>Detalhes</td>
 </tr>
 <tr>
  <td>ID do modelo</td>
 </tr>
 <tr>
  <td>E-mail</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <th rowspan="7">Recebida chamada de vendas</th>
  <td>Chamada do Sales feita por</td>
 </tr>
 <tr>
  <td>Status da Chamada de Vendas</td>
 </tr>
 <tr>
  <td>Assunto da Chamada de Vendas</td>
 </tr>
 <tr>
  <td>Nome da campanha de vendas</td>
 </tr>
 <tr>
  <td>URL da campanha de vendas</td>
 </tr>
 <tr>
  <td>Número de Telefone de Vendas Chamado</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <th rowspan="6">Adicionar a campanha de vendas</th>
  <td>Nome da campanha de vendas</td>
 </tr>
 <tr>
  <td>Status da Chamada de Vendas</td>
 </tr>
 <tr>
  <td>URL da campanha de vendas</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID da campanha de vendas</td>
 </tr>
 <tr>
  <th rowspan="6">Remover da Campanha de Vendas</th>
  <td>Nome da campanha de vendas</td>
 </tr>
 <tr>
  <td>Status da Chamada de Vendas</td>
 </tr>
 <tr>
  <td>URL da campanha de vendas</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID da campanha de vendas</td>
 </tr>
</table>

## Descrições {#descriptions}

<table> 
 <tr>
  <th>Atributo</th>
  <th>Descrição</th>
 </tr>
 <tbody> 
  <tr> 
   <td><strong>Enviado por</strong></td>
   <td>Endereço de email da pessoa que enviou o email.</td> 
  </tr> 
  <tr> 
   <td><strong>Fonte</strong></td> 
   <td>Fonte da atividade. Será definido como "Tout" para atividades de Conexão de Vendas.</td> 
  </tr> 
  <tr> 
   <td><strong>ID do modelo</strong></td> 
   <td>Quando a origem for Tout, a ID do modelo será a ID do modelo de conexão de vendas do Marketo. Use-o para direcionar um modelo específico em vez de linha de assunto, que pode existir em vários modelos.
</td> 
  </tr> 
  <tr> 
   <td><strong>Recebido por</strong></td> 
   <td>Endereço de email da pessoa que enviou o email.</td> 
  </tr> 
  <tr> 
   <td><strong>Detalhes</strong></td> 
   <td>Detalhes da mensagem de erro de rejeição.</td> 
  </tr> 
  <tr> 
   <td><strong>E-mail</strong></td> 
   <td>Endereço de email que retornou.</td> 
  </tr> 
 </tbody> 
</table>