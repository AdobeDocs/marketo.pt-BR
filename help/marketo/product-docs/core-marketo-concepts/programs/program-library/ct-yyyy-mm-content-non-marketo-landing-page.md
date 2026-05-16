---
description: Modelo do programa de página de aterrissagem de conteúdo não-Marketo. Use-o para conteúdo em páginas de aterrissagem externas.
title: CT-MM-AAAA-Conteúdo de página de destino não gerenciado pelo Marketo
feature: Programs
exl-id: b7cf8e52-4f3f-44d7-ab4c-ad10fa0badc9
TQID: https://experienceleague.adobe.com/kz-ALgszD2fVEebqSlEmL4hE-0E2rNuCcSpBBfzWgmc
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: ea6641cb-8461-4151-a8a9-9faaa44a928a
topic_v2:
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 427
ht-degree: 16%

---

# CT-MM-AAAA-Conteúdo de página de destino não gerenciado pelo Marketo {#ct-yyyy-mm-content-non-marketo-landing-page}

Este é um exemplo de um programa de conteúdo com um formulário do Marketo Engage para baixar conteúdo em uma página de aterrissagem que não seja da Marketo Engage utilizando um programa padrão do Marketo Engage. Este programa deve funcionar com um formulário do Marketo Engage incorporado no seu site. O link para a oferta/conteúdo pode ser enviado em um email de agradecimento.

Para obter mais assistência estratégica ou ajuda para personalizar um programa, entre em contato com a Equipe de Conta da Adobe ou visite a página [Adobe Professional Services](https://business.adobe.com/br/customers/consulting-services/main.html){target="_blank"}.

## Resumo do canal {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Canal</th>
   <th>Status da associação</th>
   <th>Comportamento das análises</th>
   <th>Tipo de programa</th>
  </tr>
  <tr>
   <td>Conteúdo da Web</td>
   <td>01-Membro
<br/>02-Engajado-Sucesso</td>
   <td>Inclusivo</td>
   <td>Padrão</td>
  </tr>
 </tbody>
</table>

## O programa contém o seguinte Assets {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo</th>
   <th>Nome do modelo</th>
   <th>Nome do ativo</th>
  </tr>
  <tr>
   <td>Email</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modelo de email de início rápido</a></td>
   <td>01-Email-Obrigado</td>
  </tr>
  <tr>
   <td>Formulário</td>
   <td> </td>
   <td>Formulário de registro de conteúdo FM (ativo global no Design Studio)</td>
  </tr>
  <tr>
   <td>Relatório local</td>
   <td> </td>
   <td>Desempenho do e-mail</td>
  </tr>
  <tr>
   <td>Campanha inteligente</td>
   <td> </td>
   <td>00 - Programa de aquisição de captura</td>
  </tr>
  <tr>
   <td>Campanha inteligente</td>
   <td> </td>
   <td>01-Formulário Preenchido</td>
  </tr>
  <tr>
   <td>Campanha inteligente</td>
   <td> </td>
   <td>02-Envolvido (Sucesso do programa)</td>
  </tr>
  <tr>
   <td>Pasta</td>
   <td> </td>
   <td>Assets - hospeda todos os ativos criativos
<br/>(subpastas para emails e Landing Pages)  </td>
  </tr>
  <tr>
   <td>Pasta</td>
   <td> </td>
   <td>Campanhas - hospeda todas as campanhas inteligentes</td>
  </tr>
  <tr>
   <td>Pasta</td>
   <td> </td>
   <td>Relatórios</td>
  </tr>
 </tbody>
</table>

![](assets/ct-yyyy-mm-content-non-marketo-landing-page-1.png)

## Meus tokens incluídos {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo de token</th>
   <th>Nome do token</th>
   <th>Valor</th>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Content-Title}}</code></td>
   <td><code><--My Content Title Here--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Content-Type}}</code></td>
   <td><code><--My Content Type Here--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Content-URL}}</code></td>
   <td>my.ContentURL?without=http://</td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Email-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Email-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr>
   <td>Texto</td>
   <td><code>{{my.Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
 </tbody>
</table>

## Regras de conflito {#conflict-rules}

* **Marcas do programa**
   * Criar marcas nesta assinatura - _Recomendado_
   * Ignorar

* **Modelo de página de aterrissagem com o mesmo nome**
   * Copiar modelo original
   * Usar modelo de destino - _Recomendado_

* **Imagens com o mesmo nome**
   * Manter ambos os arquivos
   * Substituir item nesta assinatura - _Recomendado_

* **Modelos de email com o mesmo nome**
   * Manter ambos os modelos
   * Substituir modelo existente - _Recomendado_

## Práticas recomendadas {#best-practices}

* Após a importação do programa de conteúdo, mova o formulário de um ativo local para um ativo global localizado no Design Studio.
   * Diminuir o número de formulários e utilizar mais ativos globais do Design Studio permite mais escalabilidade no design do programa e na governança administrativa. Ele também oferece flexibilidade para atualizações de conformidade regulares para campos, idioma de aceitação etc.

* Considere atualizar os modelos no programa importado para utilizar modelos com a marca atual ou atualize o modelo recém-importado para refletir a marca adicionando um trecho ou as informações apropriadas de logotipo/rodapé.

* Considere atualizar a convenção de nomenclatura deste exemplo de programa para alinhar-se à sua convenção de nomenclatura.

>[!NOTE]
>
>Lembre-se de atualizar os Valores do Meu token no modelo de programa e sempre que usar o programa, conforme necessário.

>[!TIP]
>
>Ative a campanha &quot;02-Envolvido&quot; para rastrear o sucesso antes que seu formulário seja publicado e os emails sejam enviados.
