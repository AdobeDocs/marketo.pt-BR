---
description: NUR-YYYY-MM-Simple Nurture - Documentação do Marketo - Documentação do produto
title: NUR-AAAA-MM-Enfermagem Simples
feature: Programs
exl-id: aed11d75-3190-46ea-8b0b-c1494645901d
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 15%

---

# NUR-AAAA-MM-Enfermagem Simples {#nur-yyyy-mm-simple-nurture}

Este é um exemplo de programas de enfermagem simples, utilizando o programa de envolvimento Marketo Engage, com conteúdo cadenciado para gotejar ao longo do tempo para seu banco de dados, enquanto utiliza fluxos para orientar registros por meio de jornadas com base no comportamento.

Para obter mais assistência estratégica ou ajuda para personalizar um programa, entre em contato com a Equipe de Conta do Adobe ou visite a página [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}.

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
   <td>Nutrição</td> 
   <td>01 - Membro 
<br/>02 - Envolvido - Êxito</td>
   <td>Inclusivo</td>
   <td>Engajamento</td>
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
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modelo de e-mail de início rápido</a></td>
   <td>01 - Email</td>
  </tr>
   <tr> 
   <td>Email</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modelo de e-mail de início rápido</a></td>
   <td>02 - Email</td>
  </tr>
   <tr> 
   <td>Email</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modelo de e-mail de início rápido</a></td>
   <td>03 - Email</td>
  </tr>
  <tr> 
   <td>Relatório local</td> 
   <td> </td>
   <td>Desempenho do e-mail</td>
  </tr>
  <tr> 
   <td>Relatório local</td> 
   <td> </td>
   <td>Desempenho do fluxo de envolvimento</td>
  </tr>
  <tr>
  <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>01 - Adicionar à criação</td>
  </tr>
  <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>02 - Pausar criação</td>
  </tr>
  <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>03 - Retomar Alimentação</td>
  </tr>
  <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>04 - Envolvido (Sucesso do programa)</td>
  </tr>
  <tr> 
   <td>Pasta</td> 
   <td> </td>
   <td>Assets - Abriga todos os ativos criativos
   <br/>(subpastas de Emails)</td>
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

![](assets/nur-yyyy-mm-simple-nurture-1.png)

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

* Considere atualizar os modelos no programa importado para utilizar modelos com a marca atual ou atualize o modelo recém-importado para refletir a marca adicionando um trecho ou as informações apropriadas de logotipo/rodapé.

* Considere atualizar a convenção de nomenclatura deste exemplo de programa para alinhar-se à sua convenção de nomenclatura.

* Certifique-se de ter regras em vigor para pausar e retomar a cadência de criação. Essas Campanhas inteligentes devem ser ativadas ou programadas antes que o Programa de engajamento seja ativado.

>[!NOTE]
>
>Lembre-se de atualizar os Valores do Meu token no modelo de programa e sempre que usar o programa, conforme necessário.

>[!TIP]
>
>Não se esqueça de ativar a campanha &quot;04 - Envolvido (Sucesso do programa)&quot; para rastrear o sucesso! Faça _antes_ de enviar seus emails.
