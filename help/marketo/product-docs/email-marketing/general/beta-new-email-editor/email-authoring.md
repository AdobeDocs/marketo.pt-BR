---
description: Criação de email - Documentação do Marketo - Documentação do produto
title: Criação de email
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: 1f899044d0eb872d4b91fa341cb8b28e1556a045
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 1%

---

# Criação de email {#email-authoring}

Saiba como criar, personalizar e visualizar emails no novo Marketo Engage Email Designer.

>[!IMPORTANT]
>
>Este artigo é destinado apenas aos membros do New Marketo Engage Email Editor beta. Por favor, não difunda.

## Criar um email {#create-an-email}

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

1. No email que acabou de criar, clique em **Adicionar conteúdo de email**.

   ![](assets/choose-your-content-type-1.png)

1. A página _Criar seu email_ é carregada. Você pode escolher entre algumas opções:

* [Criar do zero](#design-from-scratch) usando o editor visual de email

* [Importe seu próprio HTML](#import-html) por meio de um arquivo HTML ou zip

* [Selecione um modelo existente](#choose-a-template) (uma de nossas amostras ou uma que você já salvou)

### Criar do zero {#design-from-scratch}

Ao começar do zero no editor de email, use as opções abaixo para definir seu conteúdo.

1. Na página _Criar seu email_, selecione **Design do zero**.

1. Adicione [estrutura e conteúdo](#add-structure-and-content) ao seu email.

1. Adicionar [imagens](#add-assets).

1. [Personalize](#personalize-content) seu conteúdo.

1. Examine os links e [edite o rastreamento](#edit-url-tracking).

### Importar HTML {#import-html}

Você pode importar conteúdo de HTML existente para criar seu email. O conteúdo pode ser:

* Um arquivo HTML com uma folha de estilos incorporada

* Um arquivo .zip que inclui um arquivo HTML, a folha de estilos (.css) e as imagens

>[!NOTE]
>
>Não há restrições na estrutura do arquivo .zip. No entanto, as referências devem ser relativas e se encaixar na estrutura de árvore da pasta .zip.

1. Na página Criar seu modelo, selecione **Importar HTML**.

1. Arraste e solte o arquivo de HTML ou .zip desejado (ou selecione um arquivo do seu computador) e clique em **Importar**.

   ![](assets/authoring-import-your-html-1.png)

>[!NOTE]
>
>Quando o conteúdo em HTML for carregado, o conteúdo estará no modo Compatibilidade. Nesse modo, você só pode personalizar seu texto, adicionar links ou adicionar ativos ao seu conteúdo.

Você pode fazer as alterações desejadas no conteúdo importado usando as [ferramentas do editor visual de email](#add-structure-and-content).

### Escolher um modelo {#choose-a-template}

Há dois tipos de modelos para escolher.

* **Modelos de exemplo**: o Marketo Engage oferece quatro modelos de email predefinidos.

* **Modelos salvos**: são modelos criados do zero usando o menu Modelos ou um email que você criou e optou por salvar como modelo.

>[!BEGINTABS]

>[!TAB Modelos de exemplo]

Escolha um dos modelos prontos para uso para um head start no design do modelo de email.

1. A guia Modelos de amostra é aberta por padrão.

1. Selecione o template que deseja usar.

   ![](assets/authoring-sample-templates-1.png)

1. Clique em **Usar este modelo**.

   ![](assets/authoring-sample-templates-2.png)

1. Edite o conteúdo conforme desejado usando o designer de conteúdo visual.

>[!TAB Modelos salvos]

1. Clique na guia **Modelos salvos** e selecione o modelo desejado.

   ![](assets/authoring-saved-templates-1.png)

1. Clique em **Usar este modelo**.

   ![](assets/authoring-saved-templates-2.png)

1. Edite o conteúdo conforme desejado usando o designer de conteúdo visual.

>[!ENDTABS]

## Adicionar estrutura e conteúdo {#add-structure-and-content}

1. Para começar a criar ou modificar conteúdo, arraste e solte um item de Estruturas na tela. Edite suas configurações no painel à direita.

   >[!TIP]
   >
   >Selecione o componente de coluna n:n para definir o número de colunas de sua escolha (entre três e 10). Você também pode definir a largura de cada coluna movendo as setas abaixo dela.

   ![](assets/authoring-add-structure-and-content-1.png)

   >[!NOTE]
   >
   >Cada tamanho de coluna não pode ser menor que 10% da largura total do componente de estrutura. Somente colunas vazias podem ser removidas.

1. Na seção Conteúdo, arraste sobre os itens desejados e solte-os em um ou mais componentes da estrutura.

   ![](assets/authoring-add-structure-and-content-2.png)

1. Cada componente pode ser personalizado por meio das guias Configurações ou Estilo. Altere a fonte, o estilo do texto, a margem e muito mais.

### Adicionar o Assets {#add-assets}

```
ADD ASSETS OR ADD IMAGES? WHAT OTHER ASSETS CAN YOU ADD?
```

```
Access assets stored in the Assets library. IMAGES AND FILES ONLY? - For now, only from Marketo Images and Files section!!!
```

1. Para acessar suas imagens, clique no ícone Seletor de ativos.

   CAPTURA DE TELA

1. Arraste e solte a imagem desejada em um componente de estrutura.

   CAPTURA DE TELA

   >[!NOTE]
   >
   >Para substituir uma imagem existente, selecione-a e clique em **Selecionar um ativo** na guia Configurações à direita.

Clique em Ativar conteúdo de condição para adicionar conteúdo dinâmico e adaptar o conteúdo aos perfis direcionados com base em regras condicionais.



Se necessário, você pode personalizar ainda mais seu email clicando em Alternar para o editor de código no menu avançado. Isso permite editar o código fonte do email, por exemplo, para adicionar tags de rastreamento ou HTML personalizadas.

CUIDADO
Você não pode reverter para o designer visual neste email depois de alternar para o editor de código.

Quando o conteúdo estiver pronto, clique no botão Simular conteúdo para verificar a renderização. Você pode escolher a visualização de desktop ou móvel.

Quando estiver pronto, clique em Salvar

### Camadas, configurações e estilos {#layers-settings-styles}

```
ARE THEY CALLED LAYERS OR COMPONENTS - NILESH WILL CHECK
```

Abra a árvore de navegação para acessar estruturas específicas e suas colunas/componentes para uma edição mais granular. Para acessar o, clique no ícone da Árvore de navegação.

![](assets/authoring-layers-settings-styles-1.png)

O exemplo abaixo descreve as etapas para ajustar o preenchimento e o alinhamento vertical dentro de um componente de estrutura composto por colunas.

1. Selecione a coluna no componente de estrutura diretamente na tela ou usando a _Árvore de navegação_ exibida à esquerda.

1. Na barra de ferramentas da coluna, clique na ferramenta _[!UICONTROL Selecionar uma coluna]_ e escolha a que deseja editar.

   Também é possível selecioná-la na árvore de estrutura. Os parâmetros editáveis para essa coluna são exibidos nas guias _[!UICONTROL Configurações]_ e _[!UICONTROL Estilos]_ à direita.

   ![](assets/authoring-layers-settings-styles-2.png)

1. Para editar as propriedades da coluna, clique na guia _[!UICONTROL Estilos]_ à direita e altere-os de acordo com suas necessidades:

   * Para **[!UICONTROL Plano de fundo]**, altere a cor do plano de fundo conforme necessário.

     Desmarque a caixa de seleção para um plano de fundo transparente. Habilite a configuração **[!UICONTROL Imagem de plano de fundo]** para usar uma imagem como plano de fundo em vez de uma cor sólida.

   * Para o **[!UICONTROL Alinhamento]**, selecione o ícone _Superior_, _Meio_ ou _Inferior_.
   * Para **[!UICONTROL Preenchimento]**, defina o preenchimento para todos os lados.

     Selecione **[!UICONTROL Preenchimento diferente para cada lado]** se desejar ajustar o preenchimento. Clique no ícone _Bloquear_ para interromper a sincronização.

   * Expanda a seção **[!UICONTROL Avançado]** para definir estilos embutidos para a coluna.

   ![](assets/authoring-layers-settings-styles-3.png)

1. Repita essas etapas conforme necessário para ajustar o alinhamento e o preenchimento das outras colunas no componente.

1. Salve as alterações.

### Personalizar conteúdo {#personalize-content}

Os tokens funcionam no novo editor da mesma forma que no antigo, mas o ícone é diferente. O exemplo abaixo descreve a adição de um token de nome com texto de fallback.

1. Selecione o componente de texto. Coloque o cursor onde deseja que o token apareça e clique no ícone **Adicionar personalização**.

   ![](assets/authoring-personalize-content-1.png)

1. Clique no [tipo de token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} desejado.

   ![](assets/authoring-personalize-content-2.png)

1. Encontre o token desejado e clique no ícone **...** (se você clicar no ícone +, será adicionado um token sem texto de fallback).

   ![](assets/authoring-personalize-content-3.png)

   >[!NOTE]
   >
   >&quot;Texto de fallback&quot; é o novo termo do editor para o valor padrão. Exemplo: ``{{lead.First Name:default=Friend}}``. É recomendado caso não haja valor para a pessoa no campo escolhido.

1. Defina o texto de fallback e clique em **Adicionar**.

   ![](assets/authoring-personalize-content-4.png)

1. Clique em **Salvar**.

### Editar rastreamento de URL {#edit-url-tracking}

Às vezes, você não quer ativar o URL de rastreamento do Marketo em um link em um email. Isso é útil quando a página de destino não suporta parâmetros de URL e pode resultar em um link quebrado.

1. Clique no ícone Links para exibir todos os URLs do email.

   ![](assets/authoring-edit-url-tracking-1.png)

1. Clique no ícone de lápis para editar o rastreamento dos links desejados.

1. Clique no menu suspenso **Tipo de rastreamento** e faça sua seleção.

   ![](assets/authoring-edit-url-tracking-2.png)

   ```
   LABEL? - just what URL shows as (ex: my site)
   
   TAGS? - NILESH WILL CHECK ON HOW THEY WORK
   ```

   <table><tbody>
     <tr>
       <td><b>Rastrear sem mkt_tok</b></td>
       <td>definição</td>
     </tr>
     <tr>
       <td><b>Rastrear com mkt_tok</b></td>
       <td>definição</td>
     </tr>
     <tr>
       <td><b>Não rastrear</b></td>
       <td>definição</td>
     </tr>
   </tbody>
   </table>

1. Clique em **Salvar** quando terminar.

## Verificar alertas {#check-alerts}

À medida que você cria seu conteúdo, os alertas são exibidos no canto superior direito da tela quando as configurações principais estão ausentes.

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

## Testar seu email {#test-your-email}

Quando o conteúdo da mensagem é definido, você pode usar perfis de teste para pré-visualizá-la, enviar provas e controlar a forma como ela é renderizada em clientes populares de desktop, dispositivos móveis e baseados na Web. Se você inseriu conteúdo personalizado, é possível verificar como ele é exibido na mensagem usando os dados do perfil de teste.

Para visualizar seu conteúdo de email, clique em **Simular conteúdo** e adicione um perfil de teste para verificar sua mensagem usando os dados do perfil de teste.

![](assets/test-your-email-1.png)

## Referenciar um email {#reference-an-email}

Após criar um email no novo editor, você pode referenciá-lo em Campanhas inteligentes e/ou Listas inteligentes como faria com qualquer outro email.

* Faça referência a ele em uma Smart List [seguindo as etapas habituais](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md).

* Referencie-o em uma Campanha Inteligente por [seguindo as etapas habituais](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

>[!NOTE]
>
>Somente os emails salvos podem ser referenciados. Não há status de &quot;aprovado&quot; no novo editor de email.

>[!MORELIKETHIS]
>
>[Modelos de email](/help/marketo/product-docs/email-marketing/general/beta-new-email-editor/email-templates.md){target="_blank"}: saiba como criar, projetar e acessar um modelo de email no novo editor.
