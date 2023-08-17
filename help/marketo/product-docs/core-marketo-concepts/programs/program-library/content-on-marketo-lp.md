---
description: Conteúdo do Marketo LP - Documentação do Marketo - Documentação do produto
title: Conteúdo no Marketo LP
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 661a41eb0c5c43541a63a36c31837b35f516d827
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 12%

---

# Conteúdo no Marketo LP {#content-on-marketo-lp}

Nome do programa: CT-AAAA-MM-Content on Marketo LP

Este exemplo de referência foi projetado para ser um programa de conteúdo que aproveita uma página de aterrissagem do Marketo com um formulário do Marketo utilizando um programa padrão do Marketo. O formulário é para acessar o conteúdo/oferta. O link para a oferta pode ser exibido na página de agradecimento, enviado em um email de agradecimento ou em ambos. Para obter mais assistência estratégica ou ajuda para personalizar um programa, entre em contato com a equipe de conta do Adobe ou visite o [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) página.

**Resumo do canal**

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
<br/>02-Envolvido-Sucesso</td>
   <td>Inclusivo</td>
   <td>Padrão</td>
  </tr>
 </tbody> 
</table>

**O programa contém os seguintes ativos:**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo</th> 
   <th>Nome do modelo</th>
   <th>Nome do ativo</th>
  </tr> 
  <tr> 
   <td>Email</td> 
   <td>Modelo de e-mail de início rápido</td>
   <td>01-Email-Obrigado</td>
  </tr>
  <tr> 
   <td>Página</td> 
   <td>Modelo de LP de Início Rápido</td>
   <td>01 - LP - Registro</td>
  </tr>
  <tr> 
   <td>Página</td> 
   <td>Modelo de LP de Início Rápido</td>
   <td>02 - LP - Obrigado</td>
  </tr>
  <tr> 
   <td>Formulário</td> 
   <td> </td>
   <td>Formulário de registro de conteúdo</td>
  </tr>
  <tr> 
   <td>Relatório local</td> 
   <td> </td>
   <td>Desempenho do e-mail</td>
  </tr>
  <tr> 
   <td>Relatório local</td> 
   <td> </td>
   <td>Desempenho da página</td>
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
   <td>Assets - Ativos criativos 
<br/>(subpastas para páginas de e-mail e de aterrissagem)  </td>
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

CAPTURA DE TELA - Imagem do programa

**Meus tokens incluídos:**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo de token</th> 
   <th>Nome do token</th>
   <th>Valor</th>
  </tr> 
  <tr> 
   <td>Texto formatado</td> 
   <td><code>{{my.Content-Description}}</code></td>
   <td>Clique duas vezes para obter detalhes  
<br/><code><--My Content Description Here--></code> 
<br/>Edite esta descrição de conteúdo no Nível do programa, na guia Meus tokens. 
<br/>Você aprenderá: 
<li>Marcador 1</li>
<li>Marcador 2</li>
<li>Marcador 3</li></td>
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
   <td><code>{{my. Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.ThankYouPageURL?sem o http://</td>
  </tr>
 </tbody> 
</table>

>[!CAUTION]
>
>Consulte Instruções de Importação do Programa para Regras de Conflito Padrão.

**Regras de conflito padrão recomendadas para importação:**

* Marcas do programa
   * Criar marcas nesta inscrição (Padrão) - Recomendado
   * Ignorar

* Modelo de landing page com o mesmo nome
   * Copiar modelo original (padrão)
   * Usar modelo de destino - Recomendado

* Imagens com o mesmo nome
   * Manter ambos os arquivos (Padrão)
   * Substituir item nesta assinatura - Recomendado

* Modelos de e-mail com o mesmo nome
   * Manter ambos os modelos (Padrão)
   * Substituir modelo existente - Recomendado

CAPTURA DE TELA - Imagem das regras de conflito padrão

**Práticas recomendadas:**

* As práticas recomendadas da Marketo Consulting recomendam que, após a importação do programa de conteúdo, o formulário seja movido de um ativo local para um ativo global localizado no Design Studio do Marketo Engage.
   * Diminuir o número de formulários e utilizar mais ativos globais do Design Studio permite mais escalabilidade no design do programa e na governança administrativa. Ele também oferece flexibilidade em atualizações de conformidade regulares para campos, idioma de aceitação etc.

* Considere atualizar os modelos no programa importado para utilizar modelos com a marca atual ou atualize o modelo recém-importado para refletir a marca adicionando um trecho ou as informações apropriadas sobre o logotipo e o rodapé.

* Considere atualizar a convenção de nomenclatura deste modelo de programa para alinhar-se à sua convenção de nomenclatura, se necessário.

* Não se esqueça de atualizar os Valores de Meu token no modelo de programa e sempre que usar o programa, conforme necessário.

* Para obter mais assistência estratégica ou ajuda para personalizar um programa, entre em contato com a equipe de conta da Adobe ou visite o [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) página.

>[!TIP]
>
>Não se esqueça de ativar a Campanha &quot;02-Engajado&quot; para rastreamento do sucesso! Faça ISSO ANTES que seu formulário esteja ativo e os emails sejam enviados.

>[!NOTE]
>
>Meus tokens que referenciam um URL não podem conter o http:// ou https://, caso contrário, o link não funcionará adequadamente no ativo.
