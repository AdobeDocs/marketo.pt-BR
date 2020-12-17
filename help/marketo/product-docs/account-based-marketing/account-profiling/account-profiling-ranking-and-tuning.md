---
unique-page-id: 15695924
description: Classificação e ajuste do perfil da conta - Documentos do Marketing - Documentação do produto
title: Classificação e Ajuste da Definição de Perfil da Conta
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---


# Classificação e Ajuste de Definição de Perfil de Conta {#account-profiling-ranking-and-tuning}

A criação de perfil de conta identifica seu Perfil de cliente ideal (ICP), classifica empresas no banco de dados com base no ICP e adiciona dados de Indicador ICP a contas promovidas como Contas nomeadas.

## Resultados do Modelo {#model-results}

Os resultados mostram todas as suas contas conhecidas divididas por grau. A é a nota mais alta, D é a mais baixa.

![](assets/results.png)

Embora opcional, recomendamos selecionar a caixa de seleção Promover automaticamente, pois isso economizará muito tempo. Entretanto, se você quiser percorrer cada conta e [adicioná-las manualmente](http://docs.marketo.com/display/DOCS/Discover+Accounts#DiscoverAccounts-DiscoverCRMAccounts), deixe a caixa desmarcada.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Classificação</strong></td> 
   <td> 
    <div>
      Classificação da conta com base no Perfil ideal do cliente. A é o melhor ajuste, D é o menos adequado. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Propensão</strong></td> 
   <td> 
    <div>
      Estimativa do aumento da taxa de conversão em comparação com uma seleção de contas não baseada no ICP. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Contas (%)</strong></td> 
   <td> 
    <div>
      Porcentagem de contas na entrada de modelo que têm esta classificação. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% da base do modelo</strong></td> 
   <td> 
    <div>
      Porcentagem de contas com base em modelo que têm essa classificação. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Ajuste de modelo {#model-tuning}

Na guia Modelo, clique no botão Ajustar modelo.

![](assets/two.png)

Há várias guias para escolher, permitindo personalização detalhada.

![](assets/tuning-page.png)

Categorias do indicador

| **Conformidade** | Certificações, posições de conformidade/contratação. |
|---|---|
| **Operações** | Posições/contratação relacionadas com operações. |
| **HR** | Software de RH ou Folha de Pagamento, posições/contratação relacionadas a RH. |
| **Engenharia** | Tecnologias, quadros, posições relacionadas com engenharia/contratação. |
| **Vendas** | Soluções e software para vendas, posições relacionadas a vendas/contratação. |
| **Propósito** | Indicadores de intenção. |
| **IT** | Soluções de hardware e software, tecnologias, posições/contratações relacionadas à TI. |
| **Finanças** | Software financeiro, posições financeiras/contratação. |
| **Marketing** | Tecnologias de marketing e software, posições relacionadas ao marketing/contratação. |
| **Negócios** | Listas da Forbes ou Inc ou parcerias comerciais. |
| **Experiência do cliente e relações** | Sucesso do cliente e posições/contratação de relações com o cliente. |

Passe o mouse sobre as dicas de ferramenta para obter uma descrição de cada coluna.

![](assets/tool-tip.png)

Clique no menu suspenso Adicionar indicador ICP para inserir outros indicadores no modelo.

![](assets/add-icp.png)

Marcar a caixa Exportar permite que você veja o indicador ICP na página Detalhes da conta nomeada, bem como usar o indicador ICP selecionado como restrições em [filtros de conta nomeados](http://docs.marketo.com/display/DOCS/Account+Filters).

![](assets/export.png)

>[!NOTE]
>
>Os indicadores de ICP são incluídos como restrições em **Membro de Filtros e acionadores da conta nomeada**.

O Indicador de peso é o que controla o nível de importância que cada indicador recebe no seu modelo.

![](assets/weightage.png)

Clique em Atualizar modelo para que essas alterações entrem em vigor.

![](assets/refresh-button.png)

Quando terminar de ajustar seu modelo (depois de atualizá-lo), volte para a guia Resultados do modelo e clique em **Salvar e aplicar fileiras**.

![](assets/ranks.png)

