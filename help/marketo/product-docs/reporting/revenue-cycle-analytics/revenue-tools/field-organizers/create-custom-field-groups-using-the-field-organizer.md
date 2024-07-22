---
unique-page-id: 10094404
description: Criar grupos de campos personalizados usando o Organizador de campos - Documentação do Marketo - Documentação do produto
title: Criar grupos de campos personalizados usando o Organizador de campos
exl-id: 0425a446-2c92-4a2a-85c4-e05c22118035
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 2%

---

# Criar grupos de campos personalizados usando o Organizador de campos {#create-custom-field-groups-using-the-field-organizer}

Antes de poder habilitar grupos de campos personalizados para relatórios na Área Análise de Desempenho de Modelo (Clientes Potenciais) do Explorador do Ciclo de Receita, você deve categorizar campos padrão ou personalizados em grupos para relatórios por meio do Organizador de Campos no Marketo Lead Management. Isso se aplica somente aos atributos do cliente potencial e da empresa.
Quando você seleciona um campo padrão ou personalizado no menu suspenso Campo na caixa de diálogo Novo organizador de campos, o sistema mapeia o tipo de dados do Marketo Lead Management associado ao campo que você deseja agrupar com um dos três editores disponíveis no Organizador de campos: sequência, número inteiro ou data.

| Tipo de dados de gerenciamento de clientes potenciais da Marketo | Tipo de Dados do Editor do Organizador de Campos |
|---|---|
| Sequência de caracteres | Sequência de caracteres |
| Email | Sequência de caracteres |
| Inteiro | Inteiro |
| Texto | Sequência de caracteres |
| URL | Sequência de caracteres |
| Referência | Não suportado |
| Moeda | Inteiro |
| DateTime | Data |
| Booleano | Não suportado |
| Telefone | Sequência de caracteres |
| Data | Data |
| Flutuante | Inteiro |
| Calculado | Não suportado |

As próximas três seções descrevem como criar um grupo de campos personalizado para um tipo de sequência, inteiro ou data.

## Criar grupo de campos personalizado - Editor de cadeia de caracteres {#create-custom-field-group-string-editor}

1. Clique em **Banco de Dados de Cliente Potencial**.

   ![](assets/one.png)

1. Clique em **Novo** e selecione **Novo Organizador de Campos**.

   ![](assets/two.png)

1. Clique em **Campo** e selecione um campo padrão ou personalizado com um tipo de dados que mapeie para o editor de cadeia de caracteres (consulte a tabela na seção anterior). O país é usado aqui.

   ![](assets/three.png)

1. Clique em **Criar**.

   ![](assets/four.png)

   O novo grupo personalizado é exibido na árvore do banco de dados de clientes potenciais representada como Nome do campo > Grupo de nomes de campo (exemplo: País > Grupo do país).

   ![](assets/4.5.png)

1. Clique no ícone de lápis para personalizar o nome. Por exemplo, você pode renomear &quot;Grupo de países&quot; como &quot;Continente&quot;. Digite o novo nome desejado e clique fora da caixa para salvar automaticamente.

   ![](assets/five.png)

1. Por padrão, todos os valores de dados são colocados no subgrupo &quot;Outros&quot;. Para categorizar os valores de dados, clique em **Adicionar Grupo** para criar um subgrupo e nomeá-lo.

   >[!NOTE]
   >
   >Você pode adicionar até dez subgrupos para categorizar os valores de dados. A cada subgrupo criado é atribuído um número de ID.

   Neste exemplo, grupos foram criados para a maioria dos continentes.

   ![](assets/six.png)

   >[!NOTE]
   >
   >Para excluir um subgrupo, basta clicar no X vermelho ao lado do nome do subgrupo. Se houver valores de dados no grupo, eles serão movidos para o grupo padrão Outros.

1. Destaque um ou mais valores de dados na tela e arraste e solte os valores de dados no subgrupo apropriado.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Para remover um valor de dados de um subgrupo, reatribua o valor de dados ao grupo padrão de Outros.

1. Use a opção de filtro no canto superior esquerdo, logo acima da tela, para selecionar e exibir os valores de dados em um ou mais subgrupos. Os valores de dados com base na seleção do filtro são exibidos na tela.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Depois que os grupos forem definidos, você poderá ativar o grupo de campos personalizados para geração de relatórios na Análise de desempenho de modelo (clientes potenciais) por meio da guia Análise do ciclo de receita no Gerenciamento de clientes potenciais da Marketo.

## Criar grupo de campos personalizado - Editor de número inteiro {#create-custom-field-group-integer-editor}

1. Clique em **Banco de Dados de Cliente Potencial**.

   ![](assets/one.png)

1. Clique em **Novo** e selecione **Novo Organizador de Campos**.

   ![](assets/two.png)

1. Clique em **Campo** e selecione um campo padrão ou personalizado com um tipo de dados que mapeie para o editor de cadeia de caracteres (consulte a tabela na seção anterior). A receita anual é usada aqui.

   ![](assets/nine.png)

1. Clique em **Criar**.

   ![](assets/9.5.png)

   O novo grupo personalizado é exibido na árvore do banco de dados de clientes potenciais representada como Nome do campo > Grupo de nomes de campo (exemplo: Receita anual > Grupo de receita anual).

   ![](assets/9.6.png)

1. Clique no nome do grupo personalizado padrão acima do editor de números inteiros para personalizar o nome. Por exemplo, você pode renomear &quot;Grupo de receitas anuais&quot; para &quot;Receita anual por tamanho&quot;. Clique em **Salvar**.

   ![](assets/eleven.png)

   O editor de número inteiro permite criar vários subgrupos para definir cada subgrupo por tamanho. Neste exemplo, três grupos serão criados para pequenas empresas, Medium e empresas.

1. Para adicionar o primeiro grupo, digite um nome no campo **Nome do Grupo** (exemplo: Pequeno) e digite um valor máximo no campo **Intervalo do Grupo** (exemplo: 200000). Clique em **Adicionar Grupo**.

   ![](assets/twelve.png)

   Uma entrada de grupo vazia é exibida abaixo do grupo que acabou de ser inserido. O exemplo abaixo mostra uma entrada para pequenas empresas, Medium e empresas.

   >[!NOTE]
   >
   >Você pode adicionar até dez subgrupos para categorizar os valores de dados. Cada entrada de Intervalo de grupo é criada com base na entrada anterior. Se você deixar a última entrada de Intervalo de grupo em branco para o último subgrupo personalizado criado, um valor máximo de dados não será definido.

1. Clique na guia Resumo para salvar e revisar as configurações.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Para excluir um subgrupo, clique no X vermelho ao lado do nome do subgrupo.

1. Na página Resumo, verifique as configurações.

   ![](assets/13.5.png)

   >[!NOTE]
   >
   >Depois que os grupos forem definidos, você poderá ativar o grupo de campos personalizados para geração de relatórios na Análise de desempenho de modelo (clientes potenciais) por meio da guia Análise do ciclo de receita no Gerenciamento de clientes potenciais da Marketo.

## Criar grupo de campos personalizado - Editor de datas {#create-custom-field-group-date-editor}

1. Clique em **Banco de Dados de Cliente Potencial**.

   ![](assets/one.png)

1. Clique em **Novo** e selecione **Novo Organizador de Campos**.

   ![](assets/two.png)

1. Clique em **Campo** e selecione um campo padrão ou personalizado com um tipo de dados que mapeie para o editor de cadeia de caracteres (consulte a tabela na seção anterior). A data de aquisição é usada aqui.

   ![](assets/fourteen.png)

1. Clique em **Criar**.

   ![](assets/14.5.png)

   O novo grupo personalizado é exibido na árvore do Banco de dados de clientes potenciais representada como Nome do campo > Grupo de nomes de campo (exemplo: Data de aquisição > Grupo de datas de aquisição).

   ![](assets/14.6.png)

1. Clique no nome do grupo personalizado padrão acima do editor de datas para personalizar o nome. Por exemplo, você pode renomear &quot;Grupo de datas de aquisição&quot; como &quot;Categorias de datas de aquisição&quot;. Clique em **Salvar**.

   ![](assets/fifteen.png)

   O editor de datas permite criar vários subgrupos e definir cada subgrupo por data. Neste exemplo, três grupos serão criados: Q1-15 Leads, Q2-15 Leads e Q3-15 Leads.

1. Para adicionar seu primeiro grupo, insira um nome no campo **Nome do Grupo** (exemplo: Q1-15 Leads) e insira uma data no campo de data que representa a data em que o lead foi adquirido ou anterior (exemplo: 31/3/2015 para o último dia de Q1-15). Clique em **Adicionar Grupo**.

   ![](assets/sixteen.png)

   >[!NOTE]
   >
   >Você pode adicionar até dez subgrupos para categorizar os valores de dados. Cada entrada de Intervalo de grupo é criada com base na entrada anterior. Se você deixar a última entrada de Faixa de Grupos em branco para o último subgrupo personalizado criado, um valor de data final não será definido.

   O exemplo abaixo mostra uma entrada para os leads do primeiro trimestre de 2015 até o terceiro trimestre.

   ![](assets/16.5.png)

   E é isso! Bom trabalho.
