---
unique-page-id: 1147108
description: Importar um Programa - Documentos do Marketing - Documentação do produto
title: Importar um Programa
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---


# Importar um Programa {#import-a-program}

Um programa pode ser importado de uma subscrição de marketing para outra. Por exemplo, você pode criar um programa em uma caixa de proteção e depois importá-lo para sua subscrição ativa. Além disso, você pode importar um programa pré-criado da Biblioteca de Programas do Marketing Cloud.

## Importar um Programa {#import-a-program-1}

1. Vá para **Atividades de marketing.**

   ![](assets/ma.png)

1. Clique no menu suspenso **Novo**. Selecione **Importar Programa**.

   ![](assets/image2014-9-17-12-3a15-3a4.png)

   >[!NOTE]
   >
   >A Importação de programa só está disponível para usuários que têm funções com a permissão Importar Programa ativada. Saiba mais sobre [como gerenciar funções e permissões do usuário](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md).
   >
   >Para conectar uma conta de caixa de proteção à sua subscrição ao vivo, entre em contato com [Suporte de marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Selecione uma Subscrição Marketo **e um programa para importar.** Clique em **Próximo**.

   ![](assets/image2014-9-17-12-3a20-3a13.png)

1. Especifique uma **Pasta de Campanha** para o programa importado. Clique em **Próximo.**

   ![](assets/image2014-9-17-12-3a20-3a44.png)

   >[!NOTE]
   >
   >Certifique-se de que **Utilizar as regras de conflito predefinidas** estejam selecionadas. As regras de conflito são necessárias quando você importa programas para uma instância que tenham ativos com o mesmo nome.

1. Detalhes da pré-visualização e **Importar** o programa.

   ![](assets/image2014-9-17-12-3a21-3a36.png)

   Uma caixa de diálogo exibe o andamento da importação do programa.

   ![](assets/image2014-9-17-12-3a21-3a51.png)

Você receberá uma confirmação por email assim que a importação for concluída.

>[!NOTE]
>
>Você precisará reprogramar campanhas em lote importadas e ativar campanhas de disparo. O sistema desativa automaticamente as programações de campanha e aciona campanhas no programa importado.

## Identificar Programas pré-criados na Biblioteca de Programas do Marketo {#identify-pre-built-programs-in-the-marketo-program-library}

A Biblioteca de Programas do Marketing Cloud contém programas pré-criados e testados que podem ser importados para a sua subscrição. Os programas disponíveis incluem:

1. **Infraestrutura básica de gotejamento.** Envia uma série de emails separados por etapas de espera.
1. **gestão de dados.** Mantém a integridade dos dados usando campanhas inteligentes.
1. **Envie um email com Landing page.** Envia um e-mail inicial com uma oferta, como &quot;baixe este white paper&quot;. Segue um email de confirmação ou lembrete. Inclui uma landing page com um formulário.
1. **Email com status de progressão.** Envia uma explosão de correio com um link rastreável para a pessoa clicar. Atualiza o status de progressão de cada pessoa - Enviado, Aberto, Clicado etc.
1. **Momentos Interessantes.** Cria momentos interessantes para sua equipe de vendas para mantê-los no ciclo.
1. **landing page com o Respondedor automático.** Use conteúdo baixável para obter novas pessoas e estimulá-las. Inclui landings page e formulários.
1. **Ciclo de vida 2.** Usa a pontuação para mover uma pessoa de nova para qualificada de marketing.
1. **Modelo de email móvel.** Um modelo de email responsivo testado em iPhone e Android. Certas versões do Android, MS Outlook, Exchange e aplicativos de terceiros, como o Gmail e o Yahoo! Aplicativos para dispositivos móveis de email não oferecem suporte ao CSS necessário para modelos responsivos. Recomendamos que você teste antes de enviar emails.
1. **Sorteios de importação de programa.** Sorteio programa para aqueles que tentam a Biblioteca de Programas! Basta aprovar os emails e a landing page e ativar a campanha inteligente. Depois, visualização a landing page aprovada, preencha o formulário e você será inserido!
1. **Campanhas Disponíveis para Vendas.** Fornece aos representantes de vendas uma maneira de executar campanhas inteligentes de marketing de um Painel no seu CRM.
1. **Pontuação - Spark Edition.** Pontuação demográfica e comportamental capturada em um único campo de pontuação. Inclui mais de duas dúzias de campanhas relacionadas à pontuação.
1. **Pontuação - Edições padrão e seletivas.** Pontuação demográfica e comportamental capturada em campos de pontuação separados. Inclui mais de duas dúzias de campanhas relacionadas à pontuação.
1. **Sincronizar novas pessoas com o CRM.** A campanha que sincroniza novas pessoas com seu sistema CRM. Ela atribui um status de pessoa de forma que seja reconhecida como não estando pronta para venda.
1. **Webinar com adaptador de Evento.** Um conjunto completo de emails - como convites e lembretes - além de landings page com formulários e campanhas para mover pessoas pelo programa. Este programa recebe atualizações sobre inscrição, presença etc. de provedores de eventos online, como WebEx.
1. **Webinar sem adaptador de Evento.** O mesmo que acima, mas com processos manuais de registro, presença, etc.
1. **Sirius Decide Pontuar Programa**. Este programa foi criado para suportar o Modelo de Pontuação de Decisões Sirius padrão, incluindo as regras de pontuação implícitas e explícitas e a atribuição de pessoa matrixada.

>[!CAUTION]
>
>Você deve criar dois campos personalizados (&quot;Pontuação demográfica&quot; e &quot;Pontuação de comportamento&quot;) antes de importar o programa Pontuação - Padrão e Selecionar edições.

## Impacto em ativos externos durante importações de Programas {#impact-on-external-assets-during-program-imports}

Os programas usam ativos externos como modelos de e-mail, modelos de landing page, imagens, formulários, tokens e tags de programa. Você pode configurar como os modelos de landing page e as tags de programa são manipulados e o Marketo gerencia automaticamente o restante.

**Modelos de e-mail:modelos de** e-mail são importados e criados automaticamente, a menos que exista um com o mesmo nome.

**Modelos de landing page:modelos de** Landing page são importados para o estúdio de design. Você pode usar regras de conflito para configurar o comportamento quando existir um modelo com o mesmo nome. Usando a regra padrão, um número será anexado a um modelo de landing page se houver um com o mesmo nome. Por exemplo, um modelo de landing page chamado Modelo padrão 1 será criado se existir um modelo padrão nomeado.

**Imagens:** as imagens usadas pelo landing page são importadas para o estúdio de design, a menos que exista uma com o mesmo nome.

**Tokens:** Tokens que vivem fora de um programa serão convertidos em tokens locais durante o processo de importação.

>[!CAUTION]
>
>O tipo de imagem que meus tokens não são suportados para importações de programas. Se um programa com o tipo de imagem meus tokens for importado, os tokens **no** aparecerão.

**Tags de programa:** Você pode usar regras de conflito para controlar como as tags de programa que não existem na conta de destino serão tratadas. O uso da regra padrão criará as tags de programa ou você poderá optar por ignorá-las. **Forms:Formulários** externos serão importados automaticamente para o estúdio de design, a menos que exista um com o mesmo nome.

>[!CAUTION]
>
>Ao importar um programa, landings page/emails que contêm [conteúdo dinâmico](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/understanding-dynamic-content.md) serão ignorados.
