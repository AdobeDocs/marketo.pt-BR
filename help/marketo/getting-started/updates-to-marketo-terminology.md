---
unique-page-id: 11387674
description: Atualizações para a terminologia do Marketing - Documentos do Marketing - Documentação do produto
title: Atualizações na terminologia do Marketing Cloud
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---


# Atualizações na terminologia do Marketing Cloud {#updates-to-marketo-terminology}

Estamos fazendo algumas mudanças na nossa plataforma, que afetarão o que algumas coisas são chamadas. Se você tiver uma nova instância do Marketo em março de 2016, ou se a sua empresa for renovada após julho de 2016, talvez já esteja vendo a nova terminologia.

Embora você possa ver uma terminologia diferente na documentação do Marketo, tenha certeza de que todos os artigos serão atualizados em breve para refletir essas alterações. Todas as instruções são iguais.

Então, o que mudou?

## O cliente potencial é agora pessoa {#lead-is-now-person}

A maior mudança é a renomeação de Lead/Leads para Pessoa/Pessoas.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antigo</strong></td> 
   <td><strong>Novo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img width="295" src="assets/leads.png" data-linked-resource-id="11387678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img width="295" src="assets/people.png" data-linked-resource-id="11387679" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Em alguns casos, a palavra &quot;Chumbo&quot; é simplesmente removida.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antigo</strong></td> 
   <td><strong>Novo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-database.png" data-linked-resource-id="11387676" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <p><img src="assets/database.png" data-linked-resource-id="11387677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"></p> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Chumbo e Pessoa **são a mesma coisa**.

## Tokens {#tokens}

Tokens com a palavra chumbo neles não **estão mudando**. Pedimos desculpas por qualquer confusão. entretanto, alterar todos os tokens para corresponder à nova terminologia quebraria um monte de tokens em uso no momento. Então você ainda verá tokens como &quot;`{{lead.First Name}}`&quot;. Não há tokens específicos da pessoa.

>[!NOTE]
>
>Existe ** um token chamado &quot;Person Notes&quot;, no entanto esse token sempre esteve lá. Normalmente, é usado para um campo de descrição em seu CRM, se for que é.

## Gerenciamento de campos {#field-management}

Os campos que continham o termo Lead foram substituídos por Pessoa ou a palavra Lead foi removida. No entanto, uma exceção notável é o campo &quot;Proprietário do cliente potencial&quot;. Agora é conhecido como &quot;Proprietário de vendas&quot;.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antigo</strong></td> 
   <td><strong>Novo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-owner.png" data-linked-resource-id="11387757" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/sales-owner.png" data-linked-resource-id="11387758" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Para obter uma lista completa dos nomes dos campos afetados, visite este artigo [de](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens)suporte.

## A personalização em tempo real (RTP) agora é personalização da Web {#real-time-personalization-rtp-is-now-web-personalization}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Antigo</strong></td> 
   <td><strong>Novo</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/rtp.png" data-linked-resource-id="11387692" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/web.png" data-linked-resource-id="11387693" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Além da alteração de nome, agora ela consiste em quatro aplicativos separados:

| ** Personalização [da Web](http://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP)** | Possui mosaicos próprios em tela inicial |
|---|---|
| ** Marketing [Web baseado em](http://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing)conta** | Acessível via mosaico de personalização da Web |
| ** [Redirecionamento](http://docs.marketo.com/display/DOCS/Website+Retargeting)personalizado** | Acessível via mosaico de personalização da Web |
| ** Conteúdo [preditivo](http://docs.marketo.com/display/DOCS/Predictive+Content)** | Possui mosaicos próprios em tela inicial |

>[!NOTE]
>
>Os blocos visíveis na tela inicial refletirão os módulos comprados.

Obrigado pela sua paciência durante esta atualização.
