---
solution: Marketo Engage
product: marketo engage
title: Fragmentos parametrizados
description: Saiba como personalizar fragmentos tornando alguns de seus campos editáveis.
feature: Email Editor
role: User
level: Beginner, Intermediate
hide: true
hidefromtoc: true
source-git-commit: f50fe3ff6ce2d9e98fa98cc72fd756844d55660c
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 0%

---

# Fragmentos parametrizados {#parameterized-fragments}

Quando os fragmentos são usados em um email ou modelo de email, eles são bloqueados por padrão devido à herança. Isso significa que quaisquer alterações feitas em um fragmento são propagadas automaticamente para todos os ativos em que o fragmento é usado. Com fragmentos personalizáveis, campos específicos em um fragmento podem ser definidos como editáveis quando o fragmento é adicionado a um email ou modelo de email. Por exemplo, suponha que você tenha um fragmento com um banner, texto e botão. Você pode designar determinados campos, como imagem ou URL de destino do botão, como editáveis. Isso permite que os usuários modifiquem esses elementos quando incorporam o fragmento ao seu modelo de email/email, fornecendo uma experiência personalizada sem afetar o fragmento original.

Ao utilizar fragmentos parametrizados, você pode gerenciar e personalizar seu conteúdo com eficiência sem criar blocos de conteúdo totalmente novos ou interromper a herança do fragmento original. Isso garante que as alterações feitas no nível do fragmento ainda sejam propagadas, permitindo a personalização necessária no nível do template de email/email.

Os fragmentos visuais e de expressão podem ser marcados como personalizáveis. Para obter instruções detalhadas sobre como proceder com cada tipo de fragmento, consulte as seções abaixo.

CAPTURA DE TELA

—EDIÇÃO INTERROMPIDA AQUI—

## Adicionar campos editáveis em fragmentos visuais {#visual}

Para tornar partes de um fragmento visual editáveis, siga estas etapas:

>[!NOTE]
>
>Campos editáveis podem ser adicionados aos componentes **imagem**, **texto** e **botão**. Para componentes do **HTML**, os campos editáveis são adicionados usando o editor de personalização, semelhante aos fragmentos de expressão. [Saiba como adicionar campo editável em componentes do HTML e fragmentos de expressão](#expression)

1. Abra a tela de edição de conteúdo do fragmento.

1. Selecione o componente no fragmento onde deseja configurar campos editáveis.

1. O painel de propriedades do componente é aberto no lado direito. Selecione a guia **Campos editáveis** e alterne a opção **Habilitar edição**.

1. Todos os campos que podem ser editados para o componente selecionado são listados no painel. Os campos disponíveis para edição dependem do tipo de componente selecionado.

   No exemplo abaixo, permitimos a edição do URL do botão &quot;Clique aqui&quot;.

CAPTURA DE TELA

1. Clique em **Visão geral** para verificar todos os campos editáveis e seus valores padrão.

   Neste exemplo, o campo URL do botão é exibido com o valor padrão definido no componente. Esse valor será personalizável pelos usuários depois de adicionarem o fragmento ao conteúdo.

CAPTURA DE TELA

1. Quando estiver pronto, salve as alterações para atualizar o fragmento.

1. Depois de adicionar o fragmento em um email, os usuários poderão personalizar todos os campos editáveis configurados no fragmento. [Saiba como personalizar campos editáveis em um fragmento visual](../email/use-visual-fragments.md#customize-fields)

## Adicionar campos editáveis em componentes do HTML e fragmentos de expressão {#expression}

Para tornar editáveis partes de um componente do HTML ou de um fragmento de expressão, é necessário usar uma sintaxe específica no editor de expressão. Isso envolve declarar uma **variável** com um valor padrão que os usuários podem substituir após adicionar o fragmento ao seu conteúdo.

Por exemplo, suponha que você queira criar um fragmento para adicionar aos emails e permitir que os usuários personalizem uma cor específica usada em locais diferentes, como quadros ou cores de fundo dos botões. Ao criar o fragmento, é necessário declarar uma variável com uma **ID exclusiva**, por exemplo, &quot;cor&quot;, e chamá-la nos locais desejados no conteúdo do fragmento onde deseja aplicar essa cor. Ao adicionar o fragmento ao conteúdo, os usuários poderão personalizar a cor usada sempre que a variável for referenciada.

Para componentes do HTML, somente elementos específicos podem se tornar campos editáveis. Expanda a seção abaixo para obter mais informações.

+++Elementos editáveis em componentes do HTML:

Os elementos abaixo podem se tornar campos editáveis em um componente do HTML:

* Uma parte do texto
* Um URL completo para link ou imagem (não funciona com parte de um URL)
* Propriedade CSS inteira (não funciona com a propriedade parcial)

Por exemplo, no código abaixo, cada elemento destacado em vermelho pode se tornar uma propriedade:

![](assets/fragment-html.png){width="70%"}

+++
