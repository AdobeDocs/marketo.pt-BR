---
description: Programa de solicitação da Web WR-YYYY-MM - Documentação do Marketo - Documentação do produto
title: Programa de solicitação da Web WR-YYYY-MM
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 9c9046d6ac889bef4ec8ab7add82fda8e72d73b4
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 18%

---

# Programa de solicitação da Web WR-YYYY-MM {#wr-yyyy-mm-web-request-program}

Este é um exemplo de programa ideal para solicitação de contato, solicitação de orçamento, solicitação de demonstração ou formulários de solicitação de avaliação utilizando um Programa padrão Marketo Engage. Pode ser usado com Páginas de aterrissagem do Marketo ou como um formulário incorporado em páginas de aterrissagem que não sejam da Marketo. Um email de alerta é enviado a uma pessoa especificada no envio do formulário.

Para obter mais assistência estratégica ou ajuda para personalizar um programa, entre em contato com a equipe de conta do Adobe ou visite o [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} página.

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
   <td>Solicitação da Web</td> 
   <td>01 - Envolvido - Sucesso</td>
   <td>Inclusivo</td>
   <td>Padrão</td>
  </tr>
 </tbody> 
</table>

## O programa contém os seguintes ativos {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo</th> 
   <th>Nome do modelo</th>
   <th>Nome do ativo</th>
  </tr>
  <tr> 
   <td>Formulário</td> 
   <td> </td>
   <td>FM-FormulárioSolicitaçãoWeb</td>
  </tr>
  <tr> 
   <td>Email</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modelo de e-mail de início rápido</a></td>
   <td>Alert-WebRequest</td>
  </tr>
  <tr> 
   <td>Página</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Modelo de LP de Início Rápido</a></td>
   <td>01 - LP - Solicitação</td>
  </tr>
  <tr> 
   <td>Página</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Modelo de LP de Início Rápido</a></td>
   <td>02 - LP - Obrigado</td>
  </tr>
  <tr> 
   <td>Relatório local</td> 
   <td> </td>
   <td>Desempenho da página</td>
  </tr>
   <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>Nova pessoa da solicitação da Web</td>
  </tr>
   <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>Nova pessoa do webinário</td>
  </tr>
  <tr> 
   <td>Pasta</td> 
   <td> </td>
   <td>Assets - Ativos criativos 
<br/>(subpastas para Alertas e Landing Pages)</td>
  </tr>
  <tr> 
   <td>Pasta</td> 
   <td> </td>
   <td>Campanhas - Sedia todas as campanhas inteligentes</td>
  </tr>
  <tr> 
   <td>Pasta</td> 
   <td> </td>
   <td>Relatórios</td>
  </tr>
 </tbody> 
</table>

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
   <td><code>{{my.Request-Type}}</code></td>
   <td>Contato</td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.ALERT-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.ALERT-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.ALERT-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL?sem o http://</td>
  </tr>
 </tbody> 
</table>

IMAGEM DO PROGRAMA

## Regras de conflito {#conflict-rules}

* **Marcas de programa**
   * Criar tags nesta assinatura - _Recomendado_
   * Ignorar

* **Modelo de landing page com o mesmo nome**
   * Copiar modelo original
   * Usar modelo de destino - _Recomendado_

* **Imagens com o mesmo nome**
   * Manter ambos os arquivos
   * Substituir item desta inscrição - _Recomendado_

* **Modelos de e-mail com o mesmo nome**
   * Manter ambos os modelos
   * Substituir modelo existente - _Recomendado_

CAPTURA DE TELA DAS REGRAS DE CONFLITO

## Práticas recomendadas {#best-practices}

* Após a importação do programa de webinário, mova o formulário de um ativo local para um ativo global localizado no Design Studio.
   * Diminuir o número de formulários e utilizar mais ativos globais do Design Studio permite mais escalabilidade no design do programa e na governança administrativa. Ele também oferece flexibilidade para atualizações de conformidade regulares para campos, idioma de aceitação etc.

* Considere atualizar os modelos no programa importado para utilizar modelos com a marca atual ou atualize o modelo recém-importado para refletir a marca adicionando um trecho ou as informações apropriadas de logotipo/rodapé.

* Considere atualizar a convenção de nomenclatura deste exemplo de programa para alinhar-se à sua convenção de nomenclatura.

>[!NOTE]
>
>Lembre-se de atualizar os Valores do Meu token no modelo de programa e sempre que usar o programa, conforme necessário.

>[!IMPORTANT]
>
>Meus tokens que referenciam um URL não podem conter o http:// ou https://, caso contrário, o link não funcionará adequadamente no ativo.
