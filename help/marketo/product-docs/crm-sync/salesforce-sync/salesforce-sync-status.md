---
description: Status de sincronização do Salesforce - Documentos do Marketo - Documentação do produto
title: Status da sincronização do Salesforce
exl-id: 61197808-7812-4e0a-8ac6-4a60af0f7979
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 13%

---

# Status da sincronização do Salesforce {#salesforce-sync-status}

Use o Painel de status de sincronização para exibir as estatísticas de sincronização como parte das etapas de sincronização e seu status de sucesso.

As etapas de sincronização refletem operações de push ou pull por cada tipo de objeto para o esquema de objeto e os próprios dados. As estatísticas abordam novos registros, atualizações, exclusões e contagens de falhas durante a sincronização. Os usuários podem filtrar por data, tipo de operação ou tipo de objeto. O Painel de Status de Sincronização mostra o status dos ciclos de sincronização dos últimos cinco dias.

>[!NOTE]
>
>Permissões de administrador necessárias

## Ver Estado de Sincronização {#view-sync-status}

1. Clique em **Admin**.

   ![](assets/salesforce-sync-status-1.png)

1. Em Integração, clique em Salesforce e, em seguida, na guia Status de sincronização .

   ![](assets/salesforce-sync-status-2.png)

Por padrão, as estatísticas serão classificadas pela mais recente. Você pode classificar por Iniciado em ou Encerrado em — do mais recente ao mais antigo — clicando no ícone de classificação.

![](assets/salesforce-sync-status-3.png)

## Filtrar Status de Sincronização {#filter-sync-status}

1. Para filtrar os dados, clique no ícone de filtro na extremidade direita da página.

   ![](assets/salesforce-sync-status-4.png)

1. Selecione a data e o intervalo de tempo e clique nas listas suspensas para filtrar por Tipo de objeto, Tipo de operação e/ou Tipo de status.

   ![](assets/salesforce-sync-status-5.png)

1. Clique em **Aplicar**.

   ![](assets/salesforce-sync-status-6.png)

**Etapa** opcional: Para exportar erros de sincronização, clique em  **Exportar**. Os dados serão exportados como um CSV.

![](assets/salesforce-sync-status-7.png)

## Sincronizar campos de status {#sync-status-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Campo</th> 
   <th>Descrição</th> 
   <th>Valores de Enum</th> 
  </tr> 
  <tr> 
   <td colspan="1">Iniciado em</td> 
   <td colspan="1">A data/hora de início do ciclo de sincronização (fuso horário do usuário)</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Encerrado em</td> 
   <td colspan="1">A data/hora de término do ciclo de sincronização (fuso horário do usuário)</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Objeto</td> 
   <td colspan="1">Tipo de objeto</td> 
   <td colspan="1">Contato, Pessoa, Tarefa, Oportunidade, Lead, Outros como abaixo</td> 
  </tr>  
  <tr> 
   <td colspan="1">Operação</td> 
   <td colspan="1">Tipo de operação</td> 
   <td colspan="1">Tipos de operação abaixo</td> 
  </tr>  
  <tr> 
   <td colspan="1">Status</td> 
   <td colspan="1">Status do lote</td> 
   <td colspan="1">Êxito, Falha, Incompleto, Em Andamento, Limpo*</td> 
  </tr>
  <tr> 
   <td colspan="1">Novo</td> 
   <td colspan="1">Contagem de novos registros</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Atualizado</td> 
   <td colspan="1">Contagem de registros atualizados</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Excluído</td> 
   <td colspan="1">Contagem de registros excluídos</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Item malsucedido</td> 
   <td colspan="1">Número de registros cuja sincronização falhou</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">Ignorado</td> 
   <td colspan="1">Contagem de registros ignorados porque não houve alterações em campos de interesse para a Sincronização</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

*Dados revertidos para o estado de integridade anterior após a falha da etapa de sincronização.

## Tipo de objeto {#object-type}

<table> 
 <colgroup> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td colspan="1">Conta</td> 
  </tr>  
  <tr> 
   <td colspan="1">Tipo de conta</td> 
  </tr> 
  <tr> 
   <td colspan="1">Objetos personalizados</td> 
  </tr>  
  <tr> 
   <td colspan="1">Campanha</td> 
  </tr>  
  <tr> 
   <td colspan="1">Status de membro de campanha</td> 
  </tr>
  <tr> 
   <td colspan="1">Contato</td> 
  </tr>  
  <tr> 
   <td colspan="1">Modelo de e-mail</td> 
  </tr>  
  <tr> 
   <td colspan="1">Evento</td> 
  </tr> 
  <tr> 
   <td colspan="1">Pessoa (lead)</td> 
  </tr>  
  <tr> 
   <td colspan="1">Oportunidade</td> 
  </tr>  
  <tr> 
   <td colspan="1">Função de contato em oportunidades</td> 
  </tr>  
  <tr> 
   <td colspan="1">Tarefa</td> 
  </tr>  
  <tr> 
   <td colspan="1">Usuário</td> 
  </tr>  
 </tbody> 
</table>

## Operação Tipo {#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Tipo de operação</th> 
   <th>Encontrado em relação a esses objetos</th> 
   <th>Observações</th> 
   <th>Tipo de operação</th>
  </tr> 
  <tr> 
   <td colspan="1">Iniciar link com Programa</td> 
   <td colspan="1">Campanha</td> 
   <td colspan="1">Vincular campanhas a programas</td> 
   <td colspan="1">Atualizar</td>
  </tr>  
  <tr> 
   <td colspan="1">Extrair conversões</td> 
   <td colspan="1">Pessoa (lead)*</td> 
   <td colspan="1">Puxe as ações de conversão do SFDC para o Marketo. Unidades (números) são leads convertendo em Contatos</td> 
   <td colspan="1">Atualização, Item com Falha ou Ignorado</td>
  </tr> 
  <tr> 
   <td colspan="1">Extrair exclusões</td> 
   <td colspan="1">Contato, Pessoa (Lead), Oportunidade, Campanha, Membros da Campanha, Contato da Oportunidade, Objetos Personalizados, Campanhas, Status do Membro da Campanha, Função do Contato da Oportunidade</td> 
   <td colspan="1">Registros excluídos do SFDC que estão sendo sincronizados com o Marketo</td> 
   <td colspan="1">Excluído, com falha de item ou ignorado</td>
  </tr>  
  <tr> 
   <td colspan="1">Extrair atualizações</td> 
   <td colspan="1">Tarefa, Pessoa (Lead), Fila de Pessoa (Lead), Contato, Evento, Oportunidade, Conta, Tipo de Conta, Membros da Campanha, Objetos Personalizados, Campanhas, Status de Membro da Campanha, Eventos, Status de Pessoa, Oportunidade, Função de Contato de Oportunidade</td> 
   <td colspan="1">Atualizações ou Novos registros no SFDC sincronizados com o Marketo, Extrair eventos como atividades</td> 
   <td colspan="1">Novo, Atualizado, Falha no Item ou Ignorado</td>
  </tr>  
  <tr> 
   <td colspan="1">Enviar novo(a)s</td> 
   <td colspan="1">Tarefas, modelos de email</td> 
   <td colspan="1">Tarefas de push (atividades)</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">Enviar atualizações</td> 
   <td colspan="1">Tarefas, Modelos de email, Pessoa, Contato, Campanhas</td> 
   <td colspan="1">Envio de atualizações para o SFDC e também exclui</td> 
   <td colspan="1">Atualização, Item com Falha ou Ignorado</td>
  </tr>  
  <tr> 
   <td colspan="1">Sincronizar esquemas</td> 
   <td colspan="1">Membros Da Campanha, Objetos Personalizados, Campanhas, Status Do Membro Da Campanha, Tarefas, Pessoa, Oportunidade, Função De Contato Da Oportunidade, Usuários</td> 
   <td colspan="1">Sincroniza metadados para diferentes objetos, para decidir quais novos campos serão sincronizados no próximo ciclo</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Sincronizar com programa</td> 
   <td colspan="1">Campanhas</td> 
   <td colspan="1">Sincroniza o programa Marketo com campanhas SFDC</td> 
   <td colspan="1">Novo, Atualizações, Falha ou Ignorado</td>
  </tr> 
  <tr> 
   <td colspan="1">Atualizar atividades</td> 
   <td colspan="1">Tarefas</td> 
   <td colspan="1">Retirar atividades do Salesforce</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Atualizar FKS</td> 
   <td colspan="1">Todos</td> 
   <td colspan="1">Atualizar chave externa de todos os objetos</td> 
   <td colspan="1">N/D</td>
  </tr>  
 </tbody> 
</table>

*A configuração de marca no nível da assinatura decide o rótulo - &quot;Lead&quot; ou &quot;Pessoa&quot; no relatório.
