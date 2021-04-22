---
unique-page-id: 1147108
description: Importar um programa - Documentos do Marketo - Documentação do produto
title: Importar um programa
exl-id: 15e23e38-a24b-45b3-89a9-ffec85649f4a
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Importar um Programa {#import-a-program}

Um programa pode ser importado de uma assinatura Marketo para outra. Por exemplo, você pode criar um programa em uma sandbox e depois importá-lo para a sua assinatura ativa. Além disso, você pode importar um programa pré-criado da Biblioteca de programas da Marketo.

## Importar um Programa {#import-a-program-1}

1. Vá para **Marketing Activities.**

   ![](assets/ma.png)

1. Clique no menu suspenso **New**. Selecione **Importar Programa**.

   ![](assets/image2014-9-17-12-3a15-3a4.png)

   >[!NOTE]
   >
   >A Importação de Programa só está disponível para usuários que têm funções com a permissão Importar Programa ativada. Saiba mais sobre como [gerenciar funções e permissões de usuário](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >Para conectar uma conta de sandbox à sua assinatura ativa, entre em contato com o [Suporte do Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Selecione um **Subscription** do Marketo e um programa para importar. Clique em **Next**.

   ![](assets/image2014-9-17-12-3a20-3a13.png)

1. Especifique um **Pasta de Campanha** para o programa importado. Clique em **Próximo.**

   ![](assets/image2014-9-17-12-3a20-3a44.png)

   >[!NOTE]
   >
   >Verifique se a opção **Usar conflito padrão** está selecionada. As regras de conflito são necessárias ao importar programas em uma instância que tenha ativos com o mesmo nome.

1. Visualize os detalhes e **Importe** o programa.

   ![](assets/image2014-9-17-12-3a21-3a36.png)

   Uma caixa de diálogo exibe o progresso da importação do programa.

   ![](assets/image2014-9-17-12-3a21-3a51.png)

Você receberá uma confirmação por email após a conclusão da importação.

>[!NOTE]
>
>Você precisará reprogramar campanhas em lote importadas e ativar campanhas de acionador. O sistema desativa automaticamente os cronogramas de campanha e aciona campanhas no programa importado.

## Identificar programas pré-criados na biblioteca do programa Marketo {#identify-pre-built-programs-in-the-marketo-program-library}

A Biblioteca de programas Marketo contém programas pré-criados e testados que você pode importar para sua assinatura. Os programas disponíveis incluem:

1. **Infraestrutura Básica de Drips.** Envia uma série de emails separados por etapas de espera.
1. **Gerenciamento de dados.** Mantém a integridade dos dados usando campanhas inteligentes.
1. **E-mail com página de aterrissagem.** Envia um email inicial com uma oferta, como &quot;baixar este white paper&quot;. Segue com um email de confirmação ou lembrete. Inclui uma landing page com um formulário.
1. **Email com status de progressão.** Envia uma explosão de email com um link rastreável para a pessoa clicar. Atualiza o status de progressão de cada pessoa - Enviado, Aberto, Clicado etc.
1. **Momentos interessantes.** Cria momentos interessantes para sua equipe de vendas para mantê-los em loop.
1. **Landing Page com autorresponder.** Use o conteúdo baixável para obter novas pessoas e estimulá-las. Inclui páginas de aterrissagem e formulários.
1. **Ciclo de vida 2.** Usa pontuação para mover uma pessoa de nova para qualificada de marketing.
1. **Modelo de email móvel.** Um modelo de email responsivo testado com iPhone e Android. Certas versões do Android, MS Outlook, Exchange e aplicativos de terceiros, como o Gmail e o Yahoo! Os aplicativos móveis de email não suportam o CSS necessário para modelos responsivos. Recomendamos que você teste antes de enviar emails.
1. **Sorteio de importação do programa.** Programa de sorteios para quem está tentando a Biblioteca do Programa! Basta aprovar os emails e a landing page e ativar a campanha inteligente. Em seguida, visualize a landing page aprovada, preencha o formulário e você foi inserido!
1. **Campanhas Disponíveis para Vendas.** Oferece aos representantes de vendas uma maneira de executar campanhas inteligentes do Marketo a partir de um painel em seu CRM.
1. **Pontuação - Edição Spark.** Pontuação demográfica e comportamental capturada em um único campo de pontuação. Inclui mais de duas dúzias de campanhas relacionadas à pontuação.
1. **Pontuação - Padrão e Selecionar edições.** Pontuação demográfica e comportamental capturada em campos de pontuação separados. Inclui mais de duas dúzias de campanhas relacionadas à pontuação.
1. **Sincronizar novas pessoas com o CRM.** A campanha que sincroniza novas pessoas com seu sistema de CRM. Ele atribui um status de pessoa de modo que seja reconhecido como não estando pronto para vendas.
1. **Webinar com adaptador de evento.** Um conjunto completo de emails, como convites e lembretes, além de páginas de aterrissagem com formulários e campanhas para mover as pessoas pelo programa. Este programa recebe atualizações sobre registro, participação, etc. de provedores de eventos online, como WebEx.
1. **Webinar sem adaptador de evento.** Igual ao acima, mas com processos manuais de registro, participação, etc.
1. **Programa de Pontuação de Decisões Sirius**. Este programa foi criado para oferecer suporte ao Modelo de Pontuação de Decisões do Sirius padrão, incluindo as regras de pontuação implícitas e explícitas e a atribuição de pessoa matrixada.

>[!CAUTION]
>
>Você deve criar dois campos personalizados (&quot;Pontuação demográfica&quot; e &quot;Pontuação de comportamento&quot;) antes de importar o programa Pontuação - Padrão e Selecionar edições .

## Impacto em ativos externos durante as importações do programa {#impact-on-external-assets-during-program-imports}

Os programas usam ativos externos, como modelos de email, modelos de landing page, imagens, formulários, tokens e tags de programa. Você pode configurar como os modelos de página de aterrissagem e as tags de programa são manipulados e o Marketo gerencia automaticamente o restante.

**Modelos de email:** os modelos de email são importados e criados automaticamente, a menos que exista um com o mesmo nome.

**Modelos de página de aterrissagem:** os modelos de página de aterrissagem são importados para o estúdio de design. Você pode usar regras de conflito para configurar o comportamento quando existir um modelo com o mesmo nome. Usando a regra padrão, um número será anexado a um modelo de página de aterrissagem se existir um com o mesmo nome. Por exemplo, um modelo de página de aterrissagem chamado Modelo padrão 1 será criado se existir um modelo padrão nomeado.

**Imagens:** as imagens usadas pela landing pages são importadas para o estúdio de design, a menos que exista uma com o mesmo nome.

**Tokens:** os tokens que vivem fora de um programa serão convertidos em tokens locais durante o processo de importação.

>[!CAUTION]
>
>O tipo de imagem que meus tokens não são suportados em importações de programa. Se um programa que tem o tipo de imagem que meus tokens são importados, os tokens **no** serão exibidos.

**Tags de programa:** você pode usar regras de conflito para controlar como as tags de programa que não existem na conta de destino serão tratadas. O uso da regra padrão criará as tags de programa, ou você poderá optar por ignorar as tags. **Forms:** formulários externos serão importados automaticamente para o estúdio de design, a menos que exista um com o mesmo nome.

>[!CAUTION]
>
>Ao importar um programa, landing pages/emails que contêm [conteúdo dinâmico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) serão ignorados.
