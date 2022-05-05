---
description: Sincronização das mensagens das chaves de chamada e chamada - Documentos do Marketo - Documentação do produto
title: Sincronização de mensagens de chave de chamada e de chamada
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 5%

---

# Sincronização de mensagens de chave de chamada e de chamada {#syncing-call-and-call-key-messages}

Objetos de mensagem de chave de chamada e chamada em Veeva CRM são sincronizados por padrão no Marketo Engage. O Marketo sincroniza dados de até 6 meses, com base na data da chamada.

>[!NOTE]
>
>O Marketo retém dados de chamada até seis meses a partir da data da chamada.

**Quais são os acionadores/filtros relacionados à Mensagem de chave de chamada e chamada?**

Gatilhos:

* Adicionado à Chamada
* Removido da Chamada
* Adicionado à Mensagem da Chave de Chamada
* Removido da mensagem de chave de chamada
* Chamada atualizada
* Atualização da mensagem da chave de chamada

Filtros:

* Tem chamada
* Possui mensagem de chave de chamada

Os seguintes campos nas mensagens Chame e Chave de chamada são sincronizados e podem ser usados como restrições e acionadores.

<table>
  <colgroup>
    <col>
    <col>
    <col>
    <col>
    <col>
  </colgroup>
  <thead>
    <tr>
      <th>
        Objeto
      </th>
      <th>
        Rótulo do campo
      </th>
      <th>
        Descrição
      </th>
      <th>
        Nome do campo
      </th>
      <th>
        Tipo de dados
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Chamada</td>
      <td>Contador</td>
      <td>Pesquise a conta à qual a chamada está associada.</td>
      <td>Account_vod_c</td>
      <td>Pesquisa (Conta)</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>Tipo de chamada</td>
      <td>Tipo de chamada que é mantido pelo sistema com base no tipo e no conteúdo da chamada. Esse campo é usado para fins de relatório. Os valores válidos são: Detalhe Somente, Detalhe com Amostra, Detalhe do Grupo, Detalhe do Grupo com Amostra, Somente Amostra. Esses valores não devem ser alterados, mas as traduções dessas listas de opções podem ser alteradas. Os participantes têm o mesmo tipo de chamada que a chamada de cabeçalho. Para uma chamada de Grupo com 3 profissionais, todos os 4 registros têm o tipo de chamada "Detalhe do Grupo"</td>
      <td>Call_Type_vod_c</td>
      <td>Lista de seleção</td>
    </tr>
    <tr>
     <td>Chamada</td>
      <td>Contato</td>
      <td>Pesquise o contato (se houver) ao qual a chamada está associada.</td>
      <td>Contact_vod_c</td>
      <td>Pesquisa(Contato)</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>Data</td>
      <td>A data da chamada quando foi salva ou enviada pela primeira vez. Este campo é definido por meio de um acionador para a data atual se nem a data nem a hora forem fornecidas.</td>
      <td>Call_Date_vod_c</td>
      <td>Data</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>Produtos detalhados</td>
      <td>Um campo de ajuda para exibir a lista de produtos detalhados para uma chamada . Os nomes de produtos devem ser delimitados por espaços duplos e ordem na prioridade da esquerda para a direita. Este campo não controla o processamento e é incluído para tornar as listas e relatórios relacionados mais fáceis de usar.</td>
      <td>Detailed_Products_vod_c</td>
      <td>Área de texto(255)</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>É Chamada Pai?</td>
      <td>Campo de Fórmula para determinar se o registro de Chamada é o registro de Chamada Pai ou de Chamada de Participante. 1 indica que o registro é a Chamada principal. 0 indica que é uma Chamada de participante.</td>
      <td>Is_Parent_Call_vod_c</td>
      <td>Fórmula (Número)</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>Status</td>
      <td>Status da chamada — Planejado, Salvo ou Enviado. Use o Workbench de tradução para alterar os valores de exibição. Os acionadores na chamada observam esse campo para ver se a chamada está bloqueada (enviada). Esse valor é definido para o usuário quando o botão Salvar ou Enviar é pressionado.</td>
      <td>Status_vod_c</td>
      <td>Lista de seleção</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>Tipo de registro</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>Tipo de registro</td>
    </tr>
    <tr>
      <td>Mensagem da chave de chamada</td>
      <td>Chamada</td>
      <td>Pesquise a chamada. Cada mensagem principal é associada a uma chamada .</td>
      <td>Call2_vod_c</td>
      <td>Principal-Detalhe(Chamada)</td>
    </tr>
    <tr>
      <td>Mensagem da chave de chamada</td>
      <td>Categoria</td>
      <td>Registra a categoria de mensagem da mensagem. Usado principalmente para relatórios.</td>
      <td>Category_vod_c</td>
      <td>Lista de seleção</td>
    </tr>
    <tr>
      <td>Mensagem da chave de chamada</td>
      <td>Nome da apresentação do CLM</td>
      <td>Nome da Apresentação CLM com carimbo</td>
      <td>Clm_Presentation_Name_vod_c</td>
      <td>Texto (80)</td>
    </tr>
    <tr>
      <td>Mensagem da chave de chamada</td>
      <td>Nome da mensagem principal</td>
      <td>Nome da mensagem da chave com carimbo</td>
      <td>Key_Message_Name_vod_c</td>
      <td>Texto (80)</td>
    </tr>
    <tr>
      <td>Mensagem da chave de chamada</td>
      <td>Nome do produto</td>
      <td> </td>
      <td>Nome_do_produto_c</td>
      <td>Fórmula (Texto)</td>
    </tr>
    <tr>
      <td>Mensagem da chave de chamada</td>
      <td>Reação</a>
      </td>
      <td>Lista de opções de reação à mensagem. Edite a lista de opções para alterar os valores da reação.</td>
      <td>Reaction_vod_c</td>
      <td>Lista de seleção</td>
    </tr>
  </tbody>
</table>
