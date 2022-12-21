---
unique-page-id: 11380774
description: Pontuação da conta - Documentos do Marketo - Documentação do produto
title: Pontuação de contas
exl-id: 68fb5f41-f715-4a4d-b4da-9db4dc38d67d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# Pontuação de contas {#account-score}

A Pontuação de conta é uma parte essencial do Gerenciamento de conta do Target. Ajuda a determinar o nível de envolvimento de suas contas.

## O que é Pontuação de conta? {#what-is-account-scoring}

É uma abordagem sistemática criada para ajudar equipes de vendas e marketing a identificar e priorizar as empresas (incluindo prospetos) com maior probabilidade de realizar uma compra.

No mundo complexo de processos de compra de B2B, é raro um único indivíduo tomar uma decisão de compra. Há muitas vezes vários papéis envolvidos, cada um com suas próprias necessidades. A pontuação baseada em conta leva isso em consideração ao agregar as pontuações do lead de vários leads e fornecer uma pontuação em um nível de conta.

## Exemplos comuns {#common-examples}

<table> 
 <tbody>
  <tr>
   <td><strong>Pontuação de engajamento da conta</strong></td> 
   <td>Profundidade de engajamento com base em atividades comportamentais rastreadas em vários canais (por exemplo, email, Web e anúncio) das pessoas em contas de destino específicas.</td>
  </tr>
  <tr>
   <td><strong>Pontuação de interesse do produto da conta</strong></td>
   <td>Pessoas de contas de destino mostrando interesse no conteúdo de um produto específico (por exemplo, baixar um white paper).</td> 
  </tr>
  <tr>
   <td><strong>Pontuação de engajamento na Web da conta</strong></td>
   <td>Pessoas de contas de destino visitando o canal da Web. A mesma pontuação pode ser criada para medir o envolvimento do canal por email, anúncio ou outros canais.</td> 
  </tr>
 </tbody>
</table>

## Como configurar a pontuação da conta {#how-to-configure-account-score}

>[!NOTE]
>
>Para calcular as pontuações da conta, primeiro é necessário criar pontuações de lead. O Marketo TAM agrega automaticamente pontuações de lead às pontuações da conta. Como exemplo, pegaremos dois dos exemplos acima (_Pontuação de interesse do produto da conta_ e _Pontuação de engajamento na Web da conta_).
>
>Primeiro, crie campos de pontuação de lead que capturam detalhes relevantes de cada lead de uma conta de target.\
>Em seguida, atribua essas pontuações de lead às respectivas pontuações da conta:\
>Pontuação de interesse do produto da conta = SUM (Pontuação de interesse do produto líder)\
>Pontuação de engajamento com a Web da conta = SUM (Pontuação de engajamento com a Web principal)

>[!NOTE]
>
>Os usuários podem criar várias pontuações de engajamento de conta e atribuir pontuações de pessoa diferentes a diferentes pontuações de conta.

Depois de configurar a pontuação de lead, siga as etapas abaixo.

1. Clique em **Administrador**.

   ![](assets/one-1.png)

1. Clique em **Gerenciamento de conta do Target**.

   ![](assets/account-score-2.png)

1. Em Campos de pontuação, clique em **Editar**.

   ![](assets/account-score-3.png)

   >[!NOTE]
   >
   >Você pode escolher até **cinco** para calcular a Pontuação da conta.

1. Insira o nome da Pontuação da conta, clique no botão **Selecionar Pontuação de Pessoa** e selecione a pontuação correspondente.

   ![](assets/four.png)

1. Clique em **+Adicionar** para adicionar mais pontuações.

   ![](assets/five.png)

1. Adicione todas as pontuações desejadas. Clique em **Salvar** quando concluído.

   ![](assets/six.png)
