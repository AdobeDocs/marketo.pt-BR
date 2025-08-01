---
unique-page-id: 11387674
description: Atualizações na Terminologia do Marketo - Documentação do Marketo - Documentação do produto
hide: true
hidefromtoc: true
title: Atualizações na Terminologia do Marketo
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 2%

---

# Atualizações na Terminologia do Marketo {#updates-to-marketo-terminology}

Estamos fazendo algumas alterações em nossa plataforma, que afetarão o que algumas coisas são chamadas. Se você tiver uma nova instância do Marketo a partir de março de 2016, ou se sua empresa foi renovada após julho de 2016, você pode estar vendo a nova terminologia agora.

Embora você possa ver terminologias diferentes na documentação do Marketo, tenha certeza de que cada artigo será atualizado em breve para refletir essas alterações. Todas as instruções são iguais.

Então, o que mudou?

## O cliente em potencial agora é pessoa {#lead-is-now-person}

A maior mudança é a renomeação de lead/leads para pessoa/pessoas.

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

O cliente em potencial e a Pessoa **são a mesma coisa**.

## Tokens {#tokens}

Os tokens com a palavra lead neles **não são alterados**. Lamentamos qualquer confusão; no entanto, alterar todos os tokens para corresponder à nova terminologia quebraria muitos tokens em uso no momento. Portanto, você ainda verá tokens como &quot;`{{lead.First Name}}`&quot;. Não há tokens específicos para pessoas.

>[!NOTE]
>
>Existe *um* token chamado &quot;Notas de pessoa&quot;, no entanto esse token sempre esteve lá. Normalmente, é usado para um campo de descrição no CRM, se for o caso.

## Gerenciamento de campos {#field-management}

Os campos que continham o termo Cliente Potencial foram substituídos por Pessoa ou a palavra Cliente Potencial foi descartada. Uma exceção notável, no entanto, é o campo &quot;Lead Owner&quot;. Agora ele é conhecido como &quot;Proprietário de vendas&quot;.

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
>Para obter uma lista completa dos nomes de campos afetados, consulte este [Artigo de suporte](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}.

## O Real-Time Personalization (RTP) agora é o Web Personalization {#real-time-personalization-rtp-is-now-web-personalization}

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

| **[Web Personalization](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target="_blank"}** | Tem seu próprio bloco na tela inicial |
|---|---|
| **[Marketing pela Web baseado em conta](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | Acessível por meio do bloco do Web Personalization |
| **[Redirecionamento personalizado](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | Acessível por meio do bloco do Web Personalization |
| **[Conteúdo preditivo](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | Tem seu próprio bloco na tela inicial |

>[!NOTE]
>
>Os blocos visíveis na tela inicial refletirão os módulos comprados.

Agradecemos sua paciência durante esta atualização.
