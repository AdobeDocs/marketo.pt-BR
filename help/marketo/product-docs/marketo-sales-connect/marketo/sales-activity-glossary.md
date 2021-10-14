---
description: Glossário de atividades de vendas - Documentos da Marketo - Documentação do produto
title: Glossário de atividades de vendas
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: 84a285974de3bbcdf33e24befae323d3d82ef239
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 12%

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
  <th rowspan="9">Enviar e-mail de vendas</th>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID do modelo</td>
 </tr>
 <tr>
  <td>URL do modelo de vendas</td>
 </tr>
 <tr>
  <td>URL da campanha de vendas</td>
 </tr>
 <tr>
  <td>Nome do Modelo de Vendas</td>
 </tr>
 <tr>
  <td>Assunto do email</td>
 </tr>
 <tr>
  <td>Nome da campanha de vendas</td>
 </tr>
 <tr>
  <td>ID de pessoa de vendas da Marketo</td>
 </tr>
 <tr>
  <th rowspan="9">Abrir e-mail de vendas</th>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID do modelo</td>
 </tr>
 <tr>
  <td>URL do modelo de vendas</td>
 </tr>
 <tr>
  <td>URL da campanha de vendas</td>
 </tr>
 <tr>
  <td>Nome do Modelo de Vendas</td>
 </tr>
 <tr>
  <td>Assunto do email</td>
 </tr>
 <tr>
  <td>Nome da campanha de vendas</td>
 </tr>
 <tr>
  <td>ID de pessoa de vendas da Marketo</td>
 </tr>
 <tr>
  <th rowspan="10">Email de vendas clicado</th>
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
  <td>URL do modelo de vendas</td>
 </tr>
 <tr>
  <td>URL da campanha de vendas</td>
 </tr>
 <tr>
  <td>Nome do Modelo de Vendas</td>
 </tr>
 <tr>
  <td>Assunto do email</td>
 </tr>
 <tr>
  <td>Nome da campanha de vendas</td>
 </tr>
 <tr>
  <td>ID de pessoa de vendas da Marketo</td>
 </tr>
<tr>
  <th rowspan="3">Email de Vendas Recebido</th>
  <td>Recebido por</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID de pessoa de vendas da Marketo</td>
 </tr>
 <tr>
  <th rowspan="11">Recebida chamada de vendas</th>
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
  <td>Duração da chamada de vendas</td>
 </tr>
 <tr>
  <td>URL da gravação da chamada do Sales</td>
 </tr>
  <tr>
  <td>Chamada do Sales atendida por</td>
 </tr>
 <tr>
  <td>ID de pessoa de vendas da Marketo</td>
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
   <td><strong>Detalhes</strong></td> 
   <td>Detalhes da mensagem de erro de rejeição.</td> 
  </tr> 
  <tr> 
   <td><strong>E-mail</strong></td> 
   <td>Endereço de email que retornou.</td> 
  </tr> 
  <tr> 
   <td><strong>Link</strong></td> 
   <td>URL que foi clicado.</td> 
  </tr> 
  <tr> 
   <td><strong>ID de pessoa de vendas da Marketo</strong></td> 
   <td>ID exclusiva para registro de pessoa no Sales Connect.</td> 
  </tr> 
  <tr> 
   <td><strong>Recebido por</strong></td> 
   <td>Endereço de email da pessoa que enviou o email.</td> 
  </tr>
  <tr> 
   <td><strong>Chamada do Sales atendida por</strong></td> 
   <td>Nome da pessoa que atendeu a chamada.</td> 
  </tr>
  <tr> 
   <td><strong>Duração da chamada de vendas</strong></td> 
   <td>Duração da chamada em segundos.</td> 
  </tr>
  <tr> 
   <td><strong>Chamada do Sales feita por</strong></td> 
   <td>Endereço de email da pessoa que efetuou a chamada.</td> 
  </tr>
  <tr> 
   <td><strong>URL da gravação da chamada do Sales</strong></td> 
   <td>URL da gravação de chamada.</td> 
  </tr>
  <tr> 
   <td><strong>Status da Chamada de Vendas</strong></td> 
   <td>Salva o status final da chamada, que inclui: concluído, sem resposta, cancelado, com falha.</td> 
  </tr>
  <tr> 
   <td><strong>Assunto da Chamada de Vendas</strong></td> 
   <td>Resultado da chamada selecionado por um usuário de vendas no discador.</td> 
  </tr>
  <tr> 
   <td><strong>ID da campanha de vendas</strong></td> 
   <td>ID exclusiva para o ativo de campanha de vendas no Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>Nome da campanha de vendas</strong></td> 
   <td>Nome da campanha de vendas.</td> 
  </tr>
  <tr> 
   <td><strong>URL da campanha de vendas</strong></td> 
   <td>URL de Conexão de Vendas para Campanha de Vendas.</td> 
  </tr>
  <tr> 
   <td><strong>Assunto do Email de Vendas</strong></td> 
   <td>Linha de assunto do email.</td> 
  </tr>
  <tr> 
   <td><strong>Número de Telefone de Vendas Chamado</strong></td> 
   <td>Número de telefone chamado por Vendas.</td> 
  </tr>
  <tr> 
   <td><strong>Nome do Modelo de Vendas</strong></td> 
   <td>Nome do modelo de email no Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>URL do modelo de vendas</strong></td> 
   <td>URL de Conexão de Vendas para modelo de email.</td> 
  </tr>
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
 </tbody> 
</table>
