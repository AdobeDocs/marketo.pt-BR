---
description: Sincronização de mensagens de chamada e principal de chamada - Documentação do Marketo - Documentação do produto
title: Sincronizando Mensagens de Chamada e Chave de Chamada
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 9%

---

# Sincronizando Mensagens de Chamada e Chave de Chamada {#syncing-call-and-call-key-messages}

Os Objetos de Mensagem de Chave de Chamada e Chamada no [!DNL Veeva] CRM são sincronizados por padrão no Marketo Engage. O Marketo sincroniza dados que têm até 6 meses, com base na Data de criação da chamada.

>[!NOTE]
>
>O Marketo retém dados de chamada de até seis meses a partir da data da Chamada.

**Quais são os acionadores/filtros relacionados à Chamada e à Mensagem da Chave de Chamada?**

Gatilhos:

* Adicionado à chamada
* Removido da Chamada
* Adicionado à mensagem da chave de chamada
* Removido da mensagem da chave de chamada
* Chamada atualizada
* Mensagem da chave de chamada atualizada

Filtros:

* Tem Chamada
* Tem Mensagem de Chamada Principal

Os seguintes campos nas mensagens Call e Call Key são sincronizados e podem ser usados como restrições e acionadores.

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
      <td>Procure a conta à qual a chamada está associada.</td>
      <td>Account_vod_c</td>
      <td>Pesquisar (Conta)</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>Tipo de chamada</td>
      <td>Tipo de chamada que é mantido pelo sistema com base no tipo e no conteúdo da chamada. Este campo é usado para fins de relatório. Os valores válidos são: Somente detalhe, Detalhe com amostra, Detalhe do grupo, Detalhe do grupo com amostra, Somente amostra. Esses valores não devem ser alterados, mas as traduções dessas listas de opções podem ser alteradas. Os participantes têm o mesmo tipo de chamada que a chamada de cabeçalho. Para uma Chamada em grupo com três profissionais, todos os quatro registros têm o tipo de chamada "Detalhes do grupo"</td>
      <td>Call_Type_vod_c</td>
      <td>Lista de seleção</td>
    </tr>
    <tr>
     <td>Chamada</td>
      <td>Contato</td>
      <td>Procure o contato (se houver) ao qual a chamada está associada.</td>
      <td>Contact_vod_c</td>
      <td>Lookup(Contato)</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>Data</td>
      <td>A data da chamada quando ela foi salva ou enviada pela primeira vez. Esse campo é definido por meio de um acionador para a data atual se nenhum dos campos date ou datetime for fornecido.</td>
      <td>Call_Date_vod_c</td>
      <td>Data</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>É Chamada Pai?</td>
      <td>Campo de Fórmula para determinar se o registro de Chamada é o Registro de Chamada Pai ou de Participante. 1 indica que o registro é a Chamada pai. 0 indica que é uma Chamada de Participante.</td>
      <td>Is_Parent_Call_vod_c</td>
      <td>Fórmula (Número)</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>Status</td>
      <td>Status da chamada — Planejado, Salvo ou Enviado. Use a bancada de tradução para alterar os valores de exibição. Os acionadores na chamada observam esse campo para ver se a chamada está bloqueada (enviada). Esse valor é definido para o usuário quando o botão Salvar ou Enviar é pressionado.</td>
      <td>Status_vod_c</td>
      <td>Lista de seleção</td>
    </tr>
    <tr>
      <td>Chamada</td>
      <td>Tipo de registro</td>
      <td> </td>
      <td>IDdoTipodeRegistro</td>
      <td>Tipo de registro</td>
    </tr>
    <tr>
      <td>Chamar mensagem principal</td>
      <td>Chamada</td>
      <td>Pesquisa a chamada. Cada mensagem principal está associada a uma chamada.</td>
      <td>Call2_vod_c</td>
      <td>Master-Detail(Chamada)</td>
    </tr>
    <tr>
      <td>Chamar mensagem principal</td>
      <td>Categoria</td>
      <td>Registra a categoria da mensagem. Usado principalmente para relatórios.</td>
      <td>Category_vod_c</td>
      <td>Lista de seleção</td>
    </tr>
    <tr>
      <td>Chamar mensagem principal</td>
      <td>Nome da Apresentação do CLM</td>
      <td>Nome da Apresentação do CLM carimbada</td>
      <td>Clm_Presentation_Name_vod_c</td>
      <td>Texto (80)</td>
    </tr>
    <tr>
      <td>Chamar mensagem principal</td>
      <td>Nome da mensagem principal</td>
      <td>Nome da mensagem principal carimbada</td>
      <td>Key_Message_Name_vod_c</td>
      <td>Texto (80)</td>
    </tr>
    <tr>
      <td>Chamar mensagem principal</td>
      <td>Nome do produto</td>
      <td> </td>
      <td>Nome_do_Produto_c</td>
      <td>Fórmula (Texto)</td>
    </tr>
    <tr>
      <td>Chamar mensagem principal</td>
      <td>Reação</a>
      </td>
      <td>Escolha a lista de reação à mensagem. Edite a lista de opções para alterar os valores da reação.</td>
      <td>Reação_vod_c</td>
      <td>Lista de seleção</td>
    </tr>
  </tbody>
</table>
