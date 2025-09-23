---
unique-page-id: 4720232
description: Criar uma nova lista de contas - Documentação do Marketo - Documentação do produto
title: Criar uma nova lista de contas
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 12%

---

# Criar uma nova lista de contas {#create-a-new-account-list}

Crie e faça upload de uma lista de nomes de domínio e organização para selecionar essas contas principais com campanhas personalizadas.

>[!NOTE]
>
>Este artigo aplica-se somente aos clientes herdados da Web ABM. Se você adquiriu o Web ABM após setembro de 2016, siga as etapas em [este artigo](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList).

## Criar uma nova lista de contas {#create-a-new-account-list-1}

1. Ir para **[!UICONTROL Listas de Contas]**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. Selecione **[!UICONTROL Criar Novo]**.

   ![](assets/create-new-account-list-hand.jpg)

1. Selecione **[!UICONTROL Procurar]** e carregue seu arquivo CSV (verifique se o arquivo csv atende aos critérios). Adicionar um **[!UICONTROL Nome da Lista]** e uma **[!UICONTROL Descrição]**. Clique em **[!UICONTROL Salvar]**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**Qual é o formato do arquivo CSV?**
   >
   >Verifique se o arquivo CSV da conta nomeada atende aos seguintes requisitos:
   >
   >* Salvo como formato CSV
   >* Não excede 10MB
   >* Somente 4 colunas com o cabeçalho Coluna A: Nome, Coluna B: Domínio, Coluna C: País, Coluna D: Estado dos EUA.
   >* A aprovação do arquivo carregado pode levar até 2 dias úteis.
   >* Se não receber uma notificação de aprovação por e-mail, confira o estado do arquivo na página Contas nomeadas.
   >* O número total de registros/linhas acumulados para todas as listas carregadas começa em 10K, com o maior pacote totalizando 100K.

   >[!NOTE]
   >
   >**Exemplo do arquivo CSV**
   >
   >* Linha 1 Coluna A valor = Organização
   >* Linha 1 Coluna B valor = Domínio
   >* Linha 1 Coluna C valor = País
   >* Linha 1 Valor da coluna D = Estado dos EUA
   >* Um dos valores da coluna é obrigatório. No entanto, fornecer nomes de Organização e Domínio melhora as taxas de correspondência da Lista de contas.
   >* País e Estado são valores opcionais.
   >
   >   * Para o nome do país, use o nome completo do país ou o código de abreviação. Ex. Estados Unidos ou EUA.
   >   * Para um Estado dos EUA, use o código de abreviação de 2 letras, ou seja, CA. Somente os estados dos EUA são reconhecidos.
   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## Editar uma lista de contas {#edit-an-account-list}

Na página **Listas de Contas**, clique no ícone **Editar** na lista.

![](assets/create-new-account-list-edit.jpg)

Selecione **[!UICONTROL Procurar...]** e carregue seu novo arquivo CSV. Este arquivo substituirá o arquivo original. Clique em **[!UICONTROL Salvar]**. O novo arquivo carregado estará em um estado pendente até ser aprovado pelo Suporte da Marketo, quando em um estado pendente o arquivo original permanecerá ativo.

![](assets/set-account-list-edit-hands.jpg)

O arquivo CSV substituirá o arquivo existente. A lista existente permanecerá ativa até que o processamento do novo arquivo seja concluído.

## Excluir uma lista de contas nomeadas {#delete-a-named-account-list}

1. Na página **[!UICONTROL Listas de contas]**, clique no ícone Excluir da lista que deseja excluir.

   ![](assets/create-new-account-list-delete.jpg)

1. Será exibida uma mensagem para confirmar se você deseja excluir a lista. Clique em **[!UICONTROL OK]**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[Criar um segmento usando uma lista de contas](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
