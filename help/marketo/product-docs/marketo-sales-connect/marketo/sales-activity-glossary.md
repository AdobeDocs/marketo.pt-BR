---
description: Glossário de atividades de vendas - Documentação do Marketo - Documentação do produto
title: Glossário da atividade de vendas
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: 3e0836fd9f40436564c7b2d8bb58a7f771e49c33
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 17%

---

# Glossário da atividade de vendas {#sales-activity-glossary}

No Sales Connect, quando um vendedor: adiciona um lead a uma cadência de vendas, envia um email a ele ou faz uma chamada para uma atividade, ele será registrado no histórico de atividades do Marketo. Além disso, quando o lead interagir com emails, aberturas, cliques e respostas também são registrados.

As atividades abaixo serão registradas no Marketo a partir do Sales Connect.

>[!NOTE]
>
>Essas atividades e atributos estão disponíveis para serem consumidos em nossa REST e API em massa.

## Atividades {#activities}

<table>
 <tr>
  <th>Atividade de Vendas</th>
  <th>Atributo</th>
 </tr>
 <tr>
  <th rowspan="9">Enviar e-mail de vendas</th>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Origem</td>
 </tr>
 <tr>
  <td>ID do modelo</td>
 </tr>
 <tr>
  <td>URL do Modelo de Vendas</td>
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
  <td>ID do vendedor da Marketo</td>
 </tr>
 <tr>
  <th rowspan="9">Abrir e-mail de vendas</th>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Origem</td>
 </tr>
 <tr>
  <td>ID do modelo</td>
 </tr>
 <tr>
  <td>URL do Modelo de Vendas</td>
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
  <td>ID do vendedor da Marketo</td>
 </tr>
 <tr>
  <th rowspan="10">Email de vendas clicado</th>
  <td>Link</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Origem</td>
 </tr>
 <tr>
  <td>ID do modelo</td>
 </tr>
 <tr>
  <td>URL do Modelo de Vendas</td>
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
  <td>ID do vendedor da Marketo</td>
 </tr>
<tr>
  <th rowspan="3">Respondido para o e-mail de vendas</th>
  <td>Recebido por</td>
 </tr>
 <tr>
  <td>Origem</td>
 </tr>
 <tr>
  <td>ID do vendedor da Marketo</td>
 </tr>
 <tr>
  <th rowspan="11">Recebida chamada de vendas</th>
  <td>Chamada do Sales feita por</td>
 </tr>
 <tr>
  <td>Status da chamada de vendas</td>
 </tr>
 <tr>
  <td>Assunto da chamada de vendas</td>
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
  <td>Origem</td>
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
  <td>ID do vendedor da Marketo</td>
 </tr>
 <tr>
  <th rowspan="6">Adicionar a campanha de vendas</th>
  <td>Nome da campanha de vendas</td>
 </tr>
 <tr>
  <td>Status da chamada de vendas</td>
 </tr>
 <tr>
  <td>URL da campanha de vendas</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Origem</td>
 </tr>
 <tr>
  <td>ID da campanha de vendas</td>
 </tr>
 <tr>
  <th rowspan="6">Remover da campanha de vendas</th>
  <td>Nome da campanha de vendas</td>
 </tr>
 <tr>
  <td>Status da chamada de vendas</td>
 </tr>
 <tr>
  <td>URL da campanha de vendas</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>Origem</td>
 </tr>
 <tr>
  <td>ID da campanha de vendas</td>
 </tr>
 <tr>
  <th rowspan="5">Rejeição de email de vendas</th>
  <td>Detalhes</td>
 </tr>
 <tr>
  <td>Email</td>
 </tr>
 <tr>
  <td>Enviado por</td>
 </tr>
 <tr>
  <td>ID do vendedor da Marketo</td>
 </tr>
 <tr>
  <td>ID do modelo</td>
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
   <td>Detalhe da mensagem de erro rejeitada.</td> 
  </tr> 
  <tr> 
   <td><strong>Email</strong></td> 
   <td>Endereço de email rejeitado.</td> 
  </tr> 
  <tr> 
   <td><strong>Link</strong></td> 
   <td>URL que foi clicado.</td> 
  </tr> 
  <tr> 
   <td><strong>ID do vendedor da Marketo</strong></td> 
   <td>Identificador exclusivo para registro de pessoa no Sales Connect.</td> 
  </tr> 
  <tr> 
   <td><strong>Recebido por</strong></td> 
   <td>Endereço de email da pessoa que enviou o email.</td> 
  </tr>
  <tr> 
   <td><strong>Chamada do Sales atendida por</strong></td> 
   <td>Nome da pessoa que atendeu à chamada.</td> 
  </tr>
  <tr> 
   <td><strong>Duração da chamada de vendas</strong></td> 
   <td>Duração da chamada em segundos.</td> 
  </tr>
  <tr> 
   <td><strong>Chamada do Sales feita por</strong></td> 
   <td>Endereço de email do vendedor que fez a chamada.</td> 
  </tr>
  <tr> 
   <td><strong>URL da gravação da chamada do Sales</strong></td> 
   <td>URL da gravação de chamada.</td> 
  </tr>
  <tr> 
   <td><strong>Status da chamada de vendas</strong></td> 
   <td>Salvará o status final da chamada do que inclui: concluído, sem resposta, cancelado, com falha.</td> 
  </tr>
  <tr> 
   <td><strong>Assunto da chamada de vendas</strong></td> 
   <td>Resultado da chamada selecionado por um usuário de vendas no discador.</td> 
  </tr>
  <tr> 
   <td><strong>ID da campanha de vendas</strong></td> 
   <td>Identificador exclusivo do ativo Campanha de Vendas no Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>Nome da campanha de vendas</strong></td> 
   <td>Nome da campanha de vendas.</td> 
  </tr>
  <tr> 
   <td><strong>URL da campanha de vendas</strong></td> 
   <td>URL do Sales Connect para a Campanha de Vendas.</td> 
  </tr>
  <tr> 
   <td><strong>Assunto do e-mail de vendas</strong></td> 
   <td>Linha de assunto do email seguida de uma ID exclusiva (por exemplo: Minha linha de assunto (MSC-12345678)</td> 
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
   <td><strong>URL do Modelo de Vendas</strong></td> 
   <td>URL do Sales Connect para o modelo de email.</td> 
  </tr>
  <tr> 
   <td><strong>Enviado por</strong></td>
   <td>Endereço de email da pessoa que enviou o email.</td> 
  </tr> 
  <tr> 
   <td><strong>Origem</strong></td> 
   <td>Origem da atividade. Será definido como "Tout" para as atividades do Sales Connect anteriores à versão de outubro de 2021. Será "Aplicativo de vendas" para atividades do Sales Connect após a versão de outubro de 2021.</td>
  </tr> 
  <tr> 
   <td><strong>ID do modelo</strong></td> 
   <td>Quando a origem for Tout, a ID do Modelo será a ID do Modelo do Marketo Sales Connect. Use essa opção para direcionar um modelo específico em vez da linha de assunto, que pode existir em vários modelos.
</td> 
  </tr> 
 </tbody> 
</table>
