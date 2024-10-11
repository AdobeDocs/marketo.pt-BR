---
description: Criar um email - Documentação do Marketo - Documentação do produto
title: Criar um email
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 2d69e52883d141e3976c6d4fc1de6038675af602
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 0%

---

# Criar um email {#create-an-email}

Texto de introdução aqui.

>[!IMPORTANT]
>
>Este artigo é somente para membros do New Marketo Engage Email Editor fechado beta. Por favor, não difunda.

1. Faça logon no Marketo Engage por meio da [Adobe Experience Cloud](https://experiencecloud.adobe.com/){target="_blank"}.

1. Em Meu Marketo, selecione **Design Studio**.

   ![](assets/create-an-email-1.png)

1. Na árvore, selecione **Emails (Novo Editor)**.

   ![](assets/create-an-email-2.png)

1. Clique no botão **Criar email**.

   ![](assets/create-an-email-3.png)

1. Insira um nome de email e uma linha de assunto. Clique em **Criar**.

   ![](assets/create-an-email-4.png)

Pronto. Agora é hora de projetar seu email.

## Escolha seu tipo de conteúdo {#choose-your-content-type}

1. No email que acabou de criar, clique em **+ Adicionar conteúdo de email**.

   CAPTURA DE TELA

1. A página &quot;Criar seu email&quot; é carregada. Você pode escolher entre algumas opções:

* [Criar do zero](#design-from-scratch) usando o Editor de email

* [Importe seu próprio HTML](#import-html) por meio de um arquivo HTML ou zip

* [Selecione um modelo existente](#choose-a-template) (uma de nossas amostras ou uma que você já salvou)

### Criar do zero {#design-from-scratch}

Ao começar do zero no editor de email, use as opções abaixo para definir seu conteúdo.

1. Na página inicial Criar seu modelo, selecione **Criar do zero**.

Adicione estrutura e conteúdo ao email.

Adicione imagens.

Personalize o conteúdo.

Revisar e atualizar links.

### Importar HTML {#import-html}

Você pode importar conteúdo de HTML existente para criar seus modelos de email. O conteúdo pode ser:

* Um arquivo HTML com uma folha de estilos incorporada

* Um arquivo .zip que inclui um arquivo HTML, a folha de estilos (.css) e as imagens

>[!NOTE]
>
>Não há restrições na estrutura do arquivo .zip. No entanto, as referências devem ser relativas e se encaixar na estrutura de árvore da pasta .zip.

1. Na página Criar seu modelo, selecione **Importar HTML**.

   CAPTURA DE TELA

1. Arraste e solte o arquivo de HTML ou .zip desejado e clique em **Importar**.

   CAPTURA DE TELA

>[!NOTE]
>
>Quando o conteúdo em HTML for carregado, o conteúdo estará no modo Compatibilidade. Nesse modo, você só pode personalizar seu texto, adicionar links ou incluir ativos ao seu conteúdo.

Você pode fazer as alterações desejadas no conteúdo importado usando as [ferramentas do editor de email](#add-structure-and-content).

### Escolher um modelo {#choose-a-template}

Há dois tipos de modelos para escolher.

* Modelos de exemplo: o Marketo Engage oferece quatro modelos de email prontos para uso.

* Modelos salvos: são modelos criados do zero usando o menu Modelos ou um email que você criou e optou por salvar como modelo.

>[!BEGINTABS]

>[!TAB Modelos de exemplo]

Escolha um de nossos modelos prontos para uso para iniciar o design do seu email.

1. Na página Criar seu email, selecione **Modelos de exemplo**.

   CAPTURA DE TELA

1. Selecione o modelo desejado.

   CAPTURA DE TELA

1. Uma pré-visualização é exibida. Para confirmar sua seleção, clique em **Usar este modelo**.

   CAPTURA DE TELA

>[!TAB Modelos salvos]

Escolha um dos modelos criados anteriormente.

1. Na página Criar email, selecione Modelos salvos.

   CAPTURA DE TELA

1. Selecione o modelo desejado.

   CAPTURA DE TELA

1. Uma pré-visualização é exibida. Para confirmar sua seleção, clique em **Usar este modelo**.

   CAPTURA DE TELA

>[!ENDTABS]

## Adicionar estrutura e conteúdo {#add-structure-and-content}

1. Para começar a criar ou modificar conteúdo, arraste e solte um item de Estruturas na tela. Edite suas configurações no painel à direita.

   >[!TIP]
   >
   >Selecione o componente de coluna n:n para definir o número de colunas de sua escolha (entre três e 10). Você também pode definir a largura de cada coluna movendo as setas abaixo dela.

   CAPTURA DE TELA

   >[!NOTE]
   >
   >Cada tamanho de coluna não pode ser menor que 10% da largura total do componente de estrutura. Somente colunas vazias podem ser removidas.

1. Na seção Conteúdo, arraste sobre os itens desejados e solte-os em um ou mais componentes da estrutura.

   CAPTURA DE TELA

1. Cada componente pode ser personalizado por meio das guias Configurações ou Estilo. Altere a fonte, o estilo do texto, a margem e muito mais.

CAPTURA DE TELA

### Adicionar o Assets {#add-assets}

No Seletor de ativos, é possível selecionar diretamente os ativos armazenados na biblioteca do Assets. Clique duas vezes na pasta que contém seus ativos. Arraste e solte-os em um componente de estrutura.

Insira campos de personalização para personalizar seu conteúdo de atributos de perfis, associações de público-alvo, atributos contextuais e muito mais.

Clique em Ativar conteúdo de condição para adicionar conteúdo dinâmico e adaptar o conteúdo aos perfis direcionados com base em regras condicionais.

Clique na guia Links no painel esquerdo para exibir todos os URLs do conteúdo que serão rastreados. Você pode modificar o Tipo de rastreamento ou Rótulo e adicionar Tags, se necessário.

Se necessário, você pode personalizar ainda mais seu email clicando em Alternar para o editor de código no menu avançado. Isso permite editar o código fonte do email, por exemplo, para adicionar tags de rastreamento ou HTML personalizadas.

CUIDADO
Você não pode reverter para o designer visual neste email depois de alternar para o editor de código.

Quando o conteúdo estiver pronto, clique no botão Simular conteúdo para verificar a renderização. Você pode escolher a visualização de desktop ou móvel.

Quando estiver pronto, clique em Salvar





## Verificar alertas {#check-alerts}

À medida que você cria seu conteúdo, os alertas são exibidos na interface (canto superior direito da tela) quando as principais configurações estão ausentes.

Há dois tipos de alertas:

**Avisos**

Os avisos se referem às recomendações e práticas recomendadas, como:

* **O link para opção de não participação não está presente no corpo do email**: embora os links para cancelamento de inscrição sejam um requisito, a prática recomendada é adicioná-los ao corpo do email.

>[!NOTE]
>
>Não é necessário adicionar uma opção de cancelamento de inscrição para [Emails Operacionais](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md) (não marketing).

* **A versão de texto do HTML está vazia**: você deve definir uma versão de texto do corpo do email para quando o conteúdo do HTML não puder ser exibido.

* **Um link vazio está presente no corpo do email**: verifique se todos os links no seu email estão corretos.

* **O tamanho do email excedeu o limite de 100 KB**: para uma entrega ideal, verifique se o tamanho do seu email não excede 100 KB.

**Erros**

Os erros impedem que você envie ou teste o email até que sejam resolvidos:

* **Linha de assunto ausente**: é necessária uma linha de assunto de email.

* **A versão do email da mensagem está vazia**: esse erro ocorre quando o conteúdo do email não foi configurado.

## Testar seu email

Quando o conteúdo da mensagem é definido, você pode usar perfis de teste para pré-visualizá-la, enviar provas e controlar a forma como ela é renderizada em clientes populares de desktop, dispositivos móveis e baseados na Web. Se você inseriu conteúdo personalizado, é possível verificar como ele é exibido na mensagem usando os dados do perfil de teste.

Para visualizar seu conteúdo de email, clique em **Simular conteúdo** e adicione um perfil de teste para verificar sua mensagem usando os dados do perfil de teste.

CAPTURA DE TELA

## Referenciar um email {#reference-an-email}

Após criar um email no novo editor, você pode referenciá-lo em Campanhas inteligentes ou Listas inteligentes como faria com qualquer outro email.

* Faça referência a ele em uma Smart List [seguindo as etapas habituais](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md).

* Referencie-o em uma Campanha Inteligente por [seguindo as etapas habituais](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

>[!NOTE]
>
>Somente os emails salvos podem ser referenciados. Não há status de &quot;aprovado&quot; no novo editor de email.
