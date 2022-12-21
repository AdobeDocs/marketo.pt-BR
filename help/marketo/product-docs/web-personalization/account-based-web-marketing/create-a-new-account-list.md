---
unique-page-id: 4720232
description: Criar uma nova lista de contas - Documentos do Marketo - Documentação do produto
title: Criar uma nova lista de contas
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 12%

---

# Criar uma nova lista de contas {#create-a-new-account-list}

Crie e faça upload de uma lista de organizações e nomes de domínio para direcionar essas contas principais com campanhas personalizadas.

>[!NOTE]
>
>Este artigo aplica-se somente a clientes Web ABM herdados. Se você adquiriu o Web ABM após setembro de 2016, siga as etapas em [este artigo](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList) em vez disso.

## Criar uma nova lista de contas {#create-a-new-account-list-1}

1. Ir para **Listas de contas**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. Selecionar **Criar novo**.

   ![](assets/create-new-account-list-hand.jpg)

1. Selecionar **Procurar** e fazer upload do arquivo CSV (verifique se o arquivo csv atende aos critérios). Adicione um **Nome** e **Descrição**. Clique em **Salvar**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**Qual é o formato do arquivo CSV?**
   >
   >Verifique se o arquivo CSV da conta nomeada atende aos seguintes requisitos:
   >
   >* Salvo como um formato CSV
   >* Não excede 10 MB
   >* Apenas 4 colunas com o cabeçalho Coluna A: Nome, Coluna B: Domínio, Coluna C: País, Coluna D: Estado dos EUA.
   >* A aprovação do arquivo carregado pode levar até 2 dias úteis.
   >* Se não receber uma notificação de aprovação por e-mail, confira o estado do arquivo na página Contas nomeadas.
   >* O número total de registros/linhas acumulados para todas as listas carregadas começa em 10K, com o maior pacote totalizando 100K.


   >[!NOTE]
   >
   >**Exemplo do arquivo CSV**
   >
   >* Linha 1 Valor da coluna A = Organização
   >* Linha 1 Valor da coluna B = Domínio
   >* Linha 1 Valor da coluna C = País
   >* Linha 1 Valor da coluna D = Estado dos EUA
   >* Um dos valores de coluna é obrigatório. No entanto, fornecer nomes de organização e de domínio melhora as taxas de correspondência da Lista de contas.
   >* País e Estado são valores opcionais.
      >
      >   * Para o nome do país, use o nome completo do país ou o código de abreviação. Ex. Estados Unidos ou EUA.
      >   * Para um Estado dos EUA, use o código de abreviação de 2 letras, ou seja, CA. Somente os estados dos EUA são reconhecidos.

   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## Editar uma lista de contas {#edit-an-account-list}

No **Listas de contas** clique no botão **Editar** na lista.

![](assets/create-new-account-list-edit.jpg)

Selecionar **Procurar** e faça upload do novo arquivo CSV. Este arquivo substituirá o arquivo original. Clique em **Salvar**. O novo arquivo carregado estará em um estado pendente até ser aprovado pelo Suporte da Marketo, quando, em um estado pendente, o arquivo original permanecer ativo.

![](assets/set-account-list-edit-hands.jpg)

O arquivo CSV substituirá o arquivo existente. A lista existente permanecerá ativa até a conclusão do processamento do novo arquivo.

## Excluir uma lista de contas nomeadas {#delete-a-named-account-list}

1. No **Listas de contas** clique no ícone Delete da lista que deseja excluir.

   ![](assets/create-new-account-list-delete.jpg)

1. Uma mensagem é exibida para confirmar se você deseja excluir a lista. Clique em **OK**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[Criar um segmento usando uma lista de contas](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
