---
description: Critérios de público-alvo - Documentos do Marketo - Documentação do produto
title: Critérios de público
exl-id: 9b70b03e-229e-469e-bd65-07aaf2dcbec6
source-git-commit: f71ac0398b3a93d2c46201a696dd41e6ccd89000
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 2%

---

# Critérios de público {#audience-criteria}

Semelhante às Smart Lists da Marketo, os atributos de Critérios de público-alvo permitem que você defina seu público-alvo. Você pode direcionar pessoas conhecidas ou desconhecidas usando atributos inferidos, de pessoa ou da empresa (ou uma combinação desses atributos).

## Prioridade {#priority}

A prioridade determina qual Diálogo um lead recebe, caso se qualifique para mais de um. Ele é estabelecido quando você é o primeiro [criar a caixa de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}. Você pode alterar a prioridade de um Diálogo existente abrindo-o e indo para **Detalhes da caixa de diálogo** na guia Critérios de público-alvo .

![](assets/audience-criteria-1.png)

## Eventos {#events}

![](assets/audience-criteria-2.png)

Os eventos permitem direcionar os visitantes com base na rolagem ou no tempo em que eles ficam em sua página/site. No exemplo abaixo, estamos direcionando visitantes que estão em uma página específica por mais de 20 segundos.

1. Pegue o **Tempo na página** e arraste-o para a direita.

   ![](assets/audience-criteria-3.png)

1. Defina o tempo &quot;Maior que&quot; para 20 segundos.

   ![](assets/audience-criteria-4.png)

1. Adicione o URL da página desejada no [Target](#target) seção.

   ![](assets/audience-criteria-5.png)

## Atributos {#attributes}

![](assets/audience-criteria-6.png)

**Pessoas conhecidas**

Existem _many_ combinações de atributos para escolher. No exemplo abaixo, estamos direcionando tudo **pessoas conhecidas** na Califórnia, que trabalham em uma empresa com mais de 50 funcionários.

1. Pegue o **Estado da pessoa** e arraste-o para a direita.

   ![](assets/audience-criteria-7.png)

1. _Is_ é definido por padrão. No campo Selecionar valores , digite CA (também é possível clicar no menu suspenso e selecionar na lista).

   ![](assets/audience-criteria-8.png)

1. Pegue o **Tamanho da empresa** atribua-o e arraste-o para onde ele diz _arraste e solte um atributo aqui_.

   ![](assets/audience-criteria-9.png)

   >[!NOTE]
   >
   >Você também pode escolher um atributo clicando em **+** ícone .

1. Clique no menu suspenso do operador e selecione **Maior que**.

   ![](assets/audience-criteria-10.png)

1. Digite 50 e clique em outro lugar na tela para salvar.

   ![](assets/audience-criteria-11.png)

E é isso!

**Pessoas anônimas**

Há uma maneira fácil de direcionar especificamente as pessoas que ainda não estão no seu banco de dados. Neste exemplo, estamos direcionando tudo **pessoas anônimas** localizada na área de Nova York.

1. Pegue o **Email da pessoa** e arraste-o para a direita.

   ![](assets/audience-criteria-12.png)

1. Clique no menu suspenso do operador e selecione **Está vazio**.

   ![](assets/audience-criteria-13.png)

1. Pegue o **Estado inferido** atribua-o e arraste-o para onde ele diz _arraste e solte um atributo aqui_.

   ![](assets/audience-criteria-14.png)

   >[!NOTE]
   >
   >Quando alguém visita seu site, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) Os cookies e os coloca no sistema. Procuramos o IP deles em um banco de dados especial e inferimos todos os tipos de informações boas.

1. _Is_ é definido por padrão. No campo Selecionar valores , digite NY (também é possível clicar no menu suspenso e selecionar na lista).

   ![](assets/audience-criteria-15.png)

## Adicionar grupos {#add-groups}

Você também tem a opção de agrupar atributos, caso queira ter todos os atributos específicos junto com &quot;todos ou qualquer&quot; um dos outros. Você pode adicionar vários grupos.

![](assets/audience-criteria-16.png)

![](assets/audience-criteria-17.png)

## Destino {#target}

É aqui que você insere as URLs nas quais deseja que uma caixa de diálogo específica seja exibida. Você também tem a opção de adicionar exclusões.

Formatos aceitáveis:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>O uso de um asterisco atua como um curinga abrangente. So `https://*.website.com` coloca a caixa de diálogo em cada página do site, incluindo subdomínios (por exemplo: `support.website.com`). E `https://website.com/folder/*` colocaria a caixa de diálogo em cada página HTML na pasta subsequente (por exemplo: nesse caso, considere que a pasta é &quot;esportes&quot;, portanto: website.com/sports/baseball.html, website.com/sports/football.html etc.).

**Exclusões**

Use exclusões para garantir que a caixa de diálogo faça isso **not** aparecem em uma página/área específica do site. As exclusões seguem o mesmo formato que as inclusões.

![](assets/audience-criteria-18.png)

>[!MORELIKETHIS]
>
>* [Criar uma caixa de diálogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/create-a-dialogue.md){target=&quot;_blank&quot;}
>* [Designer de fluxo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/stream-designer.md){target=&quot;_blank&quot;}
>* [Relatórios](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues/reports.md){target=&quot;_blank&quot;}

