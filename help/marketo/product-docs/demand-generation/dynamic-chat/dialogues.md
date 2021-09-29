---
description: Diálogos - Documentos do Marketo - Documentação do produto
title: Diálogos
hide: true
hidefromtoc: true
source-git-commit: fe4a4b89ee295d8e351587a5ac858806a83f1305
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 1%

---

# Diálogos {#dialogues}

As caixas de diálogo são conversas de chat individuais. Saiba como personalizá-las visualmente, determinar em quais páginas elas aparecem e decidir o que é dito, bem como quem as vê.

## Criar uma nova caixa de diálogo {#create-a-new-dialogue}

1. Clique em **Diálogos**.

   ![](assets/dialogues-1.png)

1. Clique no botão **Criar novo**.

   ![](assets/dialogues-2.png)

1. Insira um nome (a descrição é opcional), defina o nível de prioridade e clique em **Save**.

   ![](assets/dialogues-3.png)

>[!NOTE]
>
>A prioridade determina qual caixa de diálogo será exibida para um visitante quando ele se qualificar para várias caixas de diálogo simultaneamente.

## Critérios de público-alvo {#audience-criteria}

Semelhante às Smart Lists da Marketo, os atributos de Critérios de público-alvo permitem que você defina seu público-alvo. Você pode direcionar leads conhecidos ou desconhecidos usando atributos inferidos, de cliente potencial ou de empresa (ou uma combinação desses atributos).

**Leads conhecidos**

Há _muitas_ combinações de atributos para escolher. Neste exemplo, estamos direcionando todos os **leads conhecidos** na Califórnia que trabalham em uma empresa com mais de 50 funcionários.

1. Pegue o atributo **Estado de lead** e arraste-o para a direita.

   ![](assets/dialogues-4.png)

1. __ Está definido por padrão. No campo Selecionar valores , digite CA (também é possível clicar no menu suspenso e selecionar na lista).

   ![](assets/dialogues-5.png)

1. Pegue o atributo **Tamanho da empresa** e arraste-o para onde diz _arraste e solte um atributo aqui_.

   ![](assets/dialogues-6.png)

   >[!NOTE]
   >
   >Você também pode escolher um atributo clicando no ícone **+**.

1. Clique na lista suspensa do operador e selecione **Maior que**.

   ![](assets/dialogues-7.png)

1. Digite 50 e clique em outro lugar na tela para salvar.

   ![](assets/dialogues-8.png)

**Leads anônimos**

Há uma maneira fácil de direcionar especificamente leads que ainda não estão em seu banco de dados. Neste exemplo, estamos direcionando todos os **leads anônimos** localizados na área de Nova York.

1. Pegue o atributo **Email de lead** e arraste-o para a direita.

   ![](assets/dialogues-9.png)

1. Clique na lista suspensa do operador e selecione **Is Empty**.

   ![](assets/dialogues-10.png)

1. Pegue o atributo **Estado inferido** e arraste-o para onde diz _arraste e solte um atributo aqui_.

   ![](assets/dialogues-11.png)

   >[!NOTE]
   >
   >Quando alguém visita seu site, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) os cookies e os coloca no sistema. Procuramos o IP deles em um banco de dados especial e inferimos todos os tipos de boas informações.

1. __ Está definido por padrão. No campo Selecionar valores , digite NY (também é possível clicar no menu suspenso e selecionar na lista).

   ![](assets/dialogues-12.png)

## Adicionar grupos {#add-groups}

Você também tem a opção de agrupar atributos, caso queira ter todos os atributos específicos junto com &quot;qualquer&quot; outro.

TERMINAR ISSO

## Destino {#target}

É aqui que você insere as URLs nas quais deseja que uma caixa de diálogo específica seja exibida.

Formatos aceitáveis:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>O uso de um asterisco atua como um curinga abrangente. Assim, `https://*.website.com` colocaria a caixa de diálogo em cada página do site, incluindo subdomínios (por exemplo: `support.website.com`). E `https://website.com/folder/*` colocaria a caixa de diálogo em cada página HTML na pasta subsequente (por exemplo: nesse caso, considere que a pasta é &quot;esportes&quot;, portanto: website.com/sports/baseball.html, website.com/sports/football.html etc.).

## Designer de fluxo {#stream-designer}

O designer de fluxo contém cartões diferentes que podem ser adicionados para moldar a conversa de bate-papo.

<table>
 <tr>
  <td><strong>Mensagem</strong></td>
  <td>Use quando quiser fazer uma declaração sem nenhuma resposta necessária (por exemplo: "Oi! Todos os itens estão 25% de desconto hoje com código SAVE25").
</td>
 </tr>
 <tr>
  <td><strong>Pergunta</strong></td>
  <td>Use quando quiser fazer uma pergunta de múltipla escolha, da qual você fornece as respostas disponíveis (por exemplo: Em que tipo de veículo você está interessado? Respostas = SUV, Compacto, Caminhão, etc.).</td>
 </tr>
 <tr>
  <td><strong>Captura de informações</strong></td>
  <td>Use quando desejar coletar informações. Os três campos a serem escolhidos são Endereço de email, Número de telefone e Texto (o que permite que o visitante grave sua própria mensagem).</td>
 </tr>
 <tr>
  <td><strong>Programador de Compromissos</strong></td>
  <td>Fornece ao visitante um calendário de datas disponíveis para agendar um acompanhamento. A disponibilidade do calendário reflete [o próximo agente na linha](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing).</td>
 </tr>
 <tr>
  <td><strong>Meta</strong></td>
  <td>Este é o único cartão que os visitantes não verão. Cabe a você determinar em qual ponto uma meta é alcançada dentro do chat específico (por exemplo: se coletar o email do visitante for seu objetivo, coloque o cartão Meta após Captura de informações no fluxo).</td>
 </tr>
</table>

**Criar um fluxo**

Há _muitas_ combinações de fluxo para criar. Neste exemplo, vamos fazer uma pergunta sim ou não e preparar algumas respostas.

EXEMPLO

## Relatórios {#reports}

Na guia Reports , visualize os dados dos últimos 90 dias. Cada categoria é definida abaixo.

<table>
 <tr>
  <td><strong>Total acionado</strong></td>
  <td>Aumenta sempre que um visitante se qualifica para/recebe uma caixa de diálogo.
</td>
 </tr>
 <tr>
  <td><strong>Envolvido</strong></td>
  <td>Aumenta sempre que um visitante clica na âncora do chatbot para abrir a caixa de diálogo.</td>
 </tr>
 <tr>
  <td><strong>Concluído</strong></td>
  <td>Aumenta sempre que um visitante atinge o fim de qualquer ramificação em uma caixa de diálogo.</td>
 </tr>
 <tr>
  <td><strong>Clientes potenciais capturados</strong></td>
  <td>Incrementa sempre que um visitante fornece um endereço de email válido em um fluxo de caixa de diálogo.</td>
 </tr>
 <tr>
  <td><strong>Reuniões marcadas</strong></td>
  <td>Aumenta sempre que um visitante agendar um compromisso com êxito por meio do chatbot.</td>
 </tr>
 <tr>
  <td><strong>Metas alcançadas</strong></td>
  <td>Aumenta sempre que um visitante atinge uma meta em qualquer fluxo de caixa de diálogo.</td>
 </tr>
</table>
