---
unique-page-id: 11387674
description: Atualizações à terminologia do Marketo - Documentos do Marketo - Documentação do produto
title: Atualizações para a terminologia do Marketo
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 1%

---

# Atualizações para a terminologia do Marketo {#updates-to-marketo-terminology}

Estamos fazendo algumas mudanças em nossa plataforma, o que afetará o que algumas coisas são chamadas. Se você tiver uma nova instância do Marketo a partir de março de 2016, ou se sua empresa for renovada após julho de 2016, você poderá ver a nova terminologia agora.

Embora você possa ver uma terminologia diferente na documentação da Marketo, tenha certeza de que todos os artigos serão atualizados em breve para refletir essas alterações. Todas as instruções são iguais.

Então, o que mudou?

## O Cliente Potencial é Agora Pessoa {#lead-is-now-person}

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

Em alguns casos, a palavra &quot;lead&quot; é simplesmente removida.

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

Líder e Pessoa **são a mesma coisa**.

## Tokens {#tokens}

Tokens com a palavra chumbo neles **não estão mudando**. Pedimos desculpas por qualquer confusão. entretanto, alterar todos os tokens para corresponder à nova terminologia quebraria muitos tokens em uso no momento. Assim, você ainda verá tokens como &quot;`{{lead.First Name}}`.&quot; Não há tokens específicos da pessoa.

>[!NOTE]
>
>Lá *é* um token chamado &quot;Notas de pessoa&quot;, no entanto, esse token estava sempre lá. Normalmente, é usado para um campo de descrição no seu CRM, se é que é.

## Gerenciamento de campos {#field-management}

Os campos que continham o termo Lead foram substituídos por Pessoa ou a palavra Lead foi removida. No entanto, uma exceção notável é o campo &quot;Proprietário principal&quot;. Agora é conhecido como &quot;Proprietário de vendas&quot;.

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
>Para obter uma lista completa dos nomes de campo afetados, visite este [Artigo de suporte](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target=&quot;_blank&quot;}.

## A Personalização em tempo real (RTP) agora é Personalização da Web {#real-time-personalization-rtp-is-now-web-personalization}

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

| **[Personalização da Web](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target=&quot;_blank&quot;}** | Possui mosaico próprio na tela inicial |
|---|---|
| **[Marketing da Web baseado em conta](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target=&quot;_blank&quot;}** | Acessível via bloco de personalização da Web |
| **[Redirecionamento personalizado](https://docs.marketo.com/display/DOCS/Website+Retargeting){target=&quot;_blank&quot;}** | Acessível via bloco de personalização da Web |
| **[Conteúdo preditivo](https://docs.marketo.com/display/DOCS/Predictive+Content){target=&quot;_blank&quot;}** | Possui mosaico próprio na tela inicial |

>[!NOTE]
>
>Os blocos visíveis na tela inicial refletirão os módulos comprados.

Obrigado por sua paciência durante esta atualização.
