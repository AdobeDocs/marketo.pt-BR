---
unique-page-id: 15695924
description: Classificação e ajuste do perfil da conta - Documentação do Marketo - Documentação do produto
title: Classificação e ajuste da criação de perfil da conta
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 2f978d814f4cf2d4d2ca9ead0c1a3e5c15430520
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 3%

---

# Classificação e ajuste da criação de perfil da conta {#account-profiling-ranking-and-tuning}

O Account Profiling identifica o seu perfil de cliente ideal (ICP), classifica as empresas no seu banco de dados com base no ICP e adiciona os dados do indicador ICP às contas promovidas como contas nomeadas.

>[!IMPORTANT]
>
>A partir de 2025, a Criação de perfil da conta não estará mais disponível para novos usuários. Ele continuará a funcionar para os usuários existentes.

## Resultados do modelo {#model-results}

Os resultados mostram todas as suas contas conhecidas detalhadas por nível. A é o grau mais alto, D é o mais baixo.

![](assets/results.png)

Embora seja opcional, recomendamos marcar a caixa de seleção Promover automaticamente, pois economizará muito tempo. No entanto, se você quiser passar por cada conta e [adicioná-las manualmente](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts), basta deixar a caixa desmarcada.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Categoria</strong></td> 
   <td> 
    <div>
      Classificação da conta com base no Perfil de cliente ideal. A é o melhor ajuste, D é o menor ajuste. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Propensão</strong></td> 
   <td> 
    <div>
      Aumento estimado na taxa de conversão em comparação a uma seleção de contas não baseada em ICP. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Contas (%)</strong></td> 
   <td> 
    <div>
      Porcentagem de contas na entrada do modelo que têm essa classificação. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% de Base de Modelo</strong></td> 
   <td> 
    <div>
      Porcentagem de contas na base de modelo que têm essa classificação. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Afinação do modelo {#model-tuning}

Na guia Modelo, clique no botão Ajustar modelo.

![](assets/two.png)

Há várias guias para escolher, permitindo uma personalização detalhada.

![](assets/tuning-page.png)

**Categorias de indicadores**

<table> 
 <tbody> 
  <tr> 
   <td><strong>Conformidade</strong></td> 
   <td> 
    <div>
      Certificações, posições/contratação relacionadas à conformidade. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Operações</strong></td> 
   <td> 
    <div>
      Posições/contratação relacionadas a operações. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>HR</strong></td> 
   <td> 
    <div>
      Software de RH ou Folha de Pagamento, posições/admissão relacionadas a RH.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Engenharia</strong></td> 
   <td> 
    <div>
      Tecnologias, estruturas, cargos relacionados à engenharia/contratação. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Vendas</strong></td> 
   <td> 
    <div>
      Soluções e software para vendas, posições/contratações relacionadas a vendas. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Intenção</strong></td> 
   <td> 
    <div>
      Indicadores de intenção. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      Soluções de hardware e software, tecnologias, posições/contratações relacionadas à TI.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Finanças</strong></td> 
   <td> 
    <div>
      Software financeiro, posições/contratação relacionadas a finanças. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Marketing</strong></td> 
   <td> 
    <div>
      Tecnologias de marketing e software, cargos/contratações relacionados a marketing. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Business</strong></td> 
   <td> 
    <div>
      Listagens da Forbes ou Inc ou parcerias comerciais. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Experiência e relações com o cliente</strong></td> 
   <td> 
    <div>
      Posições/contratações de relações com o cliente e sucesso do cliente.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Passe o mouse sobre as dicas de ferramenta para obter uma descrição de cada coluna.

![](assets/tool-tip.png)

Clique na lista suspensa Adicionar indicador ICP para inserir indicadores adicionais no modelo.

![](assets/add-icp.png)

Marcar a caixa Exportar permite que você veja o indicador ICP na página de detalhes da Conta Nomeada, bem como usar o indicador ICP selecionado como restrições em [filtros de conta nomeados](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>Os indicadores ICP estão incluídos como restrições em **Membro da Conta Nomeada** Filtros e Acionadores.

Indicador Peso é o que controla o nível de importância que cada indicador recebe em seu modelo.

![](assets/weightage.png)

Clique em Refresh Model para que as alterações entrem em vigor.

![](assets/refresh-button.png)

Quando terminar de ajustar o modelo (depois de atualizá-lo), volte para a guia Resultados do Modelo e clique em **Salvar e Aplicar Classificações**.

![](assets/ranks.png)
