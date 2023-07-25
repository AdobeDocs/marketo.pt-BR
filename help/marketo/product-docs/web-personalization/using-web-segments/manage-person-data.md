---
unique-page-id: 7504051
description: Gerenciar dados da pessoa - Documentação do Marketo - Documentação do produto
title: Gerenciar dados da pessoa
exl-id: 40f4aac8-c6e5-4cf3-9573-cac2fdf9bcad
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 18%

---

# Gerenciar dados da pessoa {#manage-person-data}

Aproveite os dados de pessoas para personalização na Web selecionando campos de pessoas para usar na segmentação.

1. Ir para **Configurações da conta**.

   ![](assets/image2015-5-7-15-3a17-3a23.png)

1. Ir para **Banco de dados**.

   ![](assets/account-settings-dropdown-database.jpg)

## Adição de um campo Nova pessoa {#adding-a-new-person-field}

1. Selecionar **Campo a ser adicionado** no menu suspenso para adicionar um campo de dados de pessoa à lista.

   ![](assets/add-a-person-field-hand.jpg)

   >[!NOTE]
   >
   >Um novo campo é adicionado em um estado pendente e pode levar até 24 horas para ser ativado.

## Deletando um Campo de Pessoa {#deleting-a-person-field}

1. Clique no ícone de exclusão ( ![—](assets/image2015-3-24-13-3a45-3a56.png)) para remover um campo da lista. Clique em **Sim** para confirmar que deseja excluir o campo.

   ![](assets/web-engagement-settings-delete.jpg)

   >[!NOTE]
   >
   >**Gerenciar campos de Dados da pessoa**
   >
   >* Somente campos de dados de pessoas podem ser incluídos
   >* Você pode adicionar até 30 campos de dados pessoais
   >* A ativação de novos campos pode demorar até 24 horas
   >* A extensão máxima dos tipos de sequências é de 255 caracteres
   >* Campos ocultos serão removidos automaticamente

<table> 
 <tbody> 
  <tr> 
   <th><p>Nome da API REST</p></th> 
   <th><p>Nome da API SOAP</p></th> 
   <th><p>Nome intuitivo</p></th> 
  </tr> 
  <tr> 
   <td><p>departamento</p></td> 
   <td><p>Departamento</p></td> 
   <td><p>Departamento</p></td> 
  </tr> 
  <tr> 
   <td><p>título</p></td> 
   <td><p>Título</p></td> 
   <td><p>Cargo</p></td> 
  </tr> 
  <tr> 
   <td><p>avaliação</p></td> 
   <td><p>Classificação</p></td> 
   <td><p>Classificação</p></td> 
  </tr> 
  <tr> 
   <td><p>leadScore</p></td> 
   <td><p>LeadScore</p></td> 
   <td><p>Pontuação</p></td> 
  </tr> 
  <tr> 
   <td><p>leadStatus</p></td> 
   <td><p>StatusDoCliente Potencial</p></td> 
   <td><p>Status</p></td> 
  </tr> 
  <tr> 
   <td><p>prioridade</p></td> 
   <td><p>Prioridade</p></td> 
   <td><p>Prioridade</p></td> 
  </tr> 
  <tr> 
   <td><p>leadRole</p></td> 
   <td><p>FunçãoDeCliente Potencial</p></td> 
   <td><p>Função</p></td> 
  </tr> 
  <tr> 
   <td><p>cancelado</p></td> 
   <td><p>Inscrição cancelada</p></td> 
   <td><p>Inscrição cancelada</p></td> 
  </tr> 
 </tbody> 
</table>

Os seguintes campos de clientes em potencial são fornecidos prontos para uso para novas contas de Personalização da Web:

>[!MORELIKETHIS]
>
>[Criar um segmento usando dados de pessoas conhecidas](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-known-person-data.md)
