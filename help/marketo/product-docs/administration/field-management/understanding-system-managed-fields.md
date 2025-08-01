---
unique-page-id: 5472615
description: Noções básicas sobre campos gerenciados pelo sistema - Documentação do Marketo - Documentação do produto
title: Noções básicas sobre campos gerenciados pelo sistema
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 16%

---

# Noções básicas sobre campos gerenciados pelo sistema {#understanding-system-managed-fields}

Você pode ter notado que a [página de detalhes da pessoa](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} tem uma série de campos não editáveis criados pela Marketo. Esses dados vêm de várias fontes e há inúmeros valores que podem ser exibidos.

## Tipos de campos {#field-types}

<table><thead>
  <tr>
    <th>Nome do campo</th>
    <th>Definição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Tipo de fonte original</td>
    <td>O local em que uma pessoa ou visitante do site foi descoberto pela primeira vez (Exemplo: Importação de lista, Visita de página da Web)</td>
  </tr>
  <tr>
    <td>Informações da fonte original</td>
    <td>Informações específicas sobre esse local (Exemplo: Nome da lista, URL da página da Web)</td>
  </tr>
  <tr>
    <td>Mecanismo de pesquisa original</td>
    <td>Se aplicável, o mecanismo de pesquisa que encaminhou a pessoa para a origem de entrada original</td>
  </tr>
  <tr>
    <td>Frase de pesquisa original</td>
    <td>Se aplicável, o termo de pesquisa usado que indicou a pessoa à fonte de entrada original</td>
  </tr>
  <tr>
    <td>Responsável pela indicação original</td>
    <td>URL que hospedava a fonte de entrada original</td>
  </tr>
  <tr>
    <td>Tipo de fonte de registro</td>
    <td>O local em que uma atividade se tornou uma pessoa pela primeira vez (Exemplo: Importação de lista, Visita de página da Web)</td>
  </tr>
  <tr>
    <td>Informações da fonte de registro</td>
    <td>Informações específicas sobre esse local (Exemplo: Nome da lista, URL da página da Web)</td>
  </tr>
  <tr>
    <td>IP anônimo</td>
    <td>Indica o endereço IP de uma pessoa</td>
  </tr>
  <tr>
    <td>Empresa indicada</td>
    <td>A melhor estimativa da Marketo (com base no IP) da empresa da pessoa</td>
  </tr>
  <tr>
    <td>Cidade indicada</td>
    <td>A melhor estimativa da Marketo (com base no IP) da cidade da pessoa</td>
  </tr>
  <tr>
    <td>Estado/região indicado</td>
    <td>A melhor estimativa da Marketo (com base no IP) do estado ou região da pessoa</td>
  </tr>
  <tr>
    <td>Código postal indicado</td>
    <td>Melhor estimativa da Marketo (com base no IP) do código postal da pessoa</td>
  </tr>
  <tr>
    <td>País indicado</td>
    <td>A melhor estimativa da Marketo (com base no IP) do país da pessoa</td>
  </tr>
  <tr>
    <td>Área metropolitana indicada</td>
    <td>A melhor estimativa da Marketo (com base no IP) da área metropolitana da pessoa</td>
  </tr>
  <tr>
    <td>Código de área telefônica indicado</td>
    <td>A melhor estimativa da Marketo (com base no IP) do código de área da pessoa</td>
  </tr>
</tbody></table>

## Valores possíveis para o tipo de Source original e de registro {#possible-values-for-original-and-registration-source-type}

Abaixo estão alguns valores possíveis e o que eles significam.

<table><thead>
  <tr>
    <th>Tipo de fonte original</th>
    <th>Definição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>A pessoa foi descoberta da sincronização do Salesforce</td>
  </tr>
  <tr>
    <td>Visitas à página da Web</td>
    <td>A pessoa foi descoberta de uma página da Web</td>
  </tr>
  <tr>
    <td>Preenchimento de formulário da Web</td>
    <td>A pessoa foi descoberta depois de preencher um formulário</td>
  </tr>
  <tr>
    <td>Importação de lista</td>
    <td>A pessoa foi descoberta em uma importação de lista</td>
  </tr>
  <tr>
    <td>Nova pessoa</td>
    <td>A pessoa foi inserida manualmente no banco de dados</td>
  </tr>
  <tr>
    <td>Clique em links da Web</td>
    <td>A pessoa foi descoberta depois de clicar em um link</td>
  </tr>
  <tr>
    <td>E-mail de vendas</td>
    <td>Uma pessoa recebeu um email por meio do Suplemento de email do Sales Insight</td>
  </tr>
  <tr>
    <td>Pessoa</td>
    <td>A pessoa foi sincronizada do Salesforce como uma pessoa</td>
  </tr>
  <tr>
    <td>Contato</td>
    <td>A pessoa foi sincronizada do Webhook como um contato</td>
  </tr>
  <tr>
    <td>API Munchkin</td>
    <td>A pessoa foi descoberta pela API do Munchkin do Marketo Engage</td>
  </tr>
  <tr>
    <td>Aplicativo social</td>
    <td>A pessoa foi descoberta por um widget de redes sociais</td>
  </tr>
  <tr>
    <td>API de serviço Web</td>
    <td>A pessoa foi descoberta por uma API de serviço Web</td>
  </tr>
  <tr>
    <td>Parceiro de evento</td>
    <td>A pessoa foi descoberta por meio de um serviço de webinário sincronizado</td>
  </tr>
  <tr>
    <td>Associar lead</td>
    <td>Pessoa que foi mesclada por meio de chamada à API Associar lead</td>
  </tr>
</tbody></table>

<table><thead>
  <tr>
    <th>Tipo de fonte de registro</th>
    <th>Definição</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Importação de lista</td>
    <td>Tornou-se uma pessoa por meio de uma importação de lista</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>Tornou-se uma pessoa por meio da sincronização do Salesforce</td>
  </tr>
  <tr>
    <td>Preenchimento de formulário da Web</td>
    <td>Tornou-se uma pessoa após preencher um formulário</td>
  </tr>
  <tr>
    <td>E-mail de vendas</td>
    <td>Uma pessoa recebeu um email por meio do Suplemento de email do Sales Insight</td>
  </tr>
  <tr>
    <td>API de serviço Web</td>
    <td>A pessoa foi criada por meio da API SOAP/REST</td>
  </tr>
  <tr>
    <td>Nova pessoa</td>
    <td>A pessoa foi inserida manualmente no banco de dados</td>
  </tr>
  <tr>
    <td>API Munchkin</td>
    <td>Tornou-se uma pessoa por meio da API Munchkin do Marketo</td>
  </tr>
  <tr>
    <td>Aplicativo social</td>
    <td>Tornou-se uma pessoa através de um widget social</td>
  </tr>
  <tr>
    <td>Parceiro de evento</td>
    <td>Tornou-se uma pessoa por meio de um serviço de webinário vinculado</td>
  </tr>
</tbody>
</table>
