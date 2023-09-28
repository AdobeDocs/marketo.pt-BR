---
description: Programa de feiras de vendas TS-YYYY-MM-DD-Marketo Docs - Documentação do produto
title: Programa de feiras de vendas em DD/MM/TS-YYYY
feature: Programs
exl-id: 32e4d07e-e9fd-4906-acc4-5f97c09f3c44
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 20%

---

# Programa de feiras de vendas em DD/MM/TS-YYYY {#ts-yyyy-mm-dd-tradeshow-program}

Este é um exemplo de um programa de feiras com convites e emails de acompanhamento utilizando um Programa de Marketo Engage Event.

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
   <td>Evento</td> 
   <td>01-Convidado 
   <br/>02 - Em Lista de Espera
   <br/>03-Registrado
   <br/>Cabine Visitada em 04
   <br/>05-Envolvido no Show - Sucesso
   <br/>06-Envolvido em um Post Show - Sucesso</td>
   <td>Inclusivo</td>
   <td>Evento</td>
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
   <td>Email</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modelo de e-mail de início rápido</a></td>
   <td>01-Email-Obrigado</td>
  </tr>
   <tr> 
   <td>Email</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modelo de e-mail de início rápido</a></td>
   <td>02a- Email - Convite</td>
  </tr>
  <tr>
  <tr> 
   <td>Relatório local</td> 
   <td> </td>
   <td>Desempenho do e-mail</td>
  </tr>
  <tr> 
   <td>Relatório local</td> 
   <td> </td>
   <td>Desempenho do programa</td>
  </tr>
  <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>00 - Programa de aquisição de captura</td>
  </tr>
  <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>01 - Enviar Convite</td>
  </tr>
   <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>02 - Enviar emails de acompanhamento</td>
  </tr>
   <tr> 
   <td>Campanha inteligente</td> 
   <td> </td>
   <td>03 - Envolvido pelo email de acompanhamento (Sucesso)</td>
  </tr>
  <tr> 
   <td>Pasta</td> 
   <td> </td>
   <td>Assets - Ativos criativos 
<br/>(subpastas para páginas de e-mail e de aterrissagem)</td>
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

![](assets/ts-yyyy-mm-dd-tradeshow-program-1.png)

## Meus tokens incluídos {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo de token</th> 
   <th>Nome do token</th>
   <th>Valor</th>
  </tr>
  <tr> 
   <td>Arquivo de calendário</td> 
   <td><code>{{my.AddToCalendar}}</code></td>
   <td>Clique duas vezes para obter detalhes</td>
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
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
   <tr> 
   <td>Texto formatado</td> 
   <td><code>{{my.Event-Booth#}}</code></td>
   <td><code><--My Booth Number--></code></td>
  </tr>
   <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-City}}</code></td>
   <td><code><--My Event City Here--></code></td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-Time}}</code></td>
   <td><code><--My Event Time + TimeZone--></code></td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-Title}}</code></td>
   <td><code><--My Event Title Here--></code></td>
  </tr>
  <tr> 
   <td>Texto</td> 
   <td><code>{{my.Event-Type}}</code></td>
   <td>Evento comercial</td>
  </tr>
 </tbody> 
</table>

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

## Práticas recomendadas {#best-practices}

* Após a importação do programa de webinário, mova o formulário de um ativo local para um ativo global localizado no Design Studio.
   * Diminuir o número de formulários e utilizar mais ativos globais do Design Studio permite mais escalabilidade no design do programa e na governança administrativa. Ele também oferece flexibilidade em atualizações de conformidade regulares para campos, idioma de aceitação etc.

* Considere atualizar os modelos no programa importado para utilizar modelos com a marca atual ou atualize o modelo recém-importado para refletir a marca adicionando um trecho ou as informações apropriadas de logotipo/rodapé.

* Considere atualizar a convenção de nomenclatura deste exemplo de programa para alinhar-se à sua convenção de nomenclatura.

>[!NOTE]
>
>Lembre-se de atualizar os Valores do Meu token no modelo de programa e sempre que usar o programa, conforme necessário.

>[!TIP]
>
>Não se esqueça de ativar a campanha &quot;03 - Engajado pelo e-mail de acompanhamento (sucesso do programa)&quot; para rastrear o sucesso! Faça isso _antes_ seus emails serão enviados.

>[!IMPORTANT]
>
>Meus tokens que referenciam um URL não podem conter o http:// ou https://, caso contrário, o link não funcionará adequadamente no ativo.
