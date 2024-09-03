---
description: Permissões — Documentação do Marketo — Documentação do produto
title: Permissões
feature: Dynamic Chat
exl-id: 06798ac4-636b-476e-bbb1-498062844406
source-git-commit: 38e1e2d8c2fef7163f77d7774837571008075b5f
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 5%

---

# Permissões {#permissions}

Há cinco perfis padrão com permissões predefinidas que podem ser editadas no Dynamic Chat. Você também pode criar um perfil personalizado com um conjunto personalizado de permissões. Vamos analisar os dois.

## Editar permissões existentes {#edit-existing-permissions}

1. No [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}, clique em **Dynamic Chat**.

   ![](assets/permissions-1.png)

1. Na guia **Perfis de produto**, selecione o perfil que deseja editar. Neste exemplo, estamos escolhendo **Live Agent**.

   ![](assets/permissions-2.png)

1. Clique na guia **Permissões**.

   ![](assets/permissions-3.png)

1. Selecione a área do perfil que deseja editar. Neste exemplo, estamos escolhendo Bate-papo ao Vivo. Clique no ícone de lápis.

   ![](assets/permissions-4.png)

1. Os itens de permissão disponíveis estão listados à esquerda. Você pode optar por adicionar permissões uma por uma ou todas de uma vez. Clique no sinal **+**.

   ![](assets/permissions-5.png)

   >[!NOTE]
   >
   >Ativar a Inclusão automática adicionará todos os itens de permissão à lista incluída. Quando novos itens de permissão se tornarem disponíveis, eles serão incluídos automaticamente para esse perfil de produto.

1. Clique em **Salvar**.

   ![](assets/permissions-6.png)

Agora é possível repetir esse processo para qualquer/todas as outras áreas de Dynamic Chat.

![](assets/permissions-7.png)

## Criar um perfil {#create-a-profile}

1. No [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}, clique em **Dynamic Chat**.

   ![](assets/permissions-8.png)

1. Na guia **Perfis de produto**, clique em **Novo perfil**.

   ![](assets/permissions-9.png)

1. **Nomeie** seu perfil de produto. Como opção, você pode fornecer um nome de exibição e/ou descrição e optar por notificar os usuários quando eles forem adicionados/removidos. Clique em **Salvar** quando terminar.

   ![](assets/permissions-10.png)

1. O novo perfil aparecerá na guia Perfis de produto. Selecione-o.

   ![](assets/permissions-11.png)

1. Agora siga as etapas 3 a 6 da [seção acima](#edit-existing-permissions) para cada área desejada.

## Lista de permissões {#list-of-permissions}

Abaixo você encontrará uma lista de todas as permissões disponíveis para cada área.

<table>
<thead>
  <tr>
    <th style="width:25%">Área de Dynamic Chat</th>
    <th>Permissões</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gerenciamento de Conversas</td>
    <td><li>Exibir caixas de diálogo</li>
    <li>Gerenciar caixas de diálogo (criar, excluir)</li>
    <li>Caixas de diálogo do Publish</li>
    <li>Exibir Fluxos de Conversa</li>
    <li>Gerenciar Fluxos de Conversação (criar, excluir)</li>
    <li>Fluxos de conversa do Publish</li></td>
  </tr>
  <tr>
    <td>Chat ao vivo</td>
    <td><li>Exibir minhas conversas</li>
    <li>Exibir Todas as Conversas</li>
  </tr>
  <tr>
    <td>Reuniões</td>
    <td><li>Gerenciar Todas as Reuniões</li>
  </tr>
  <tr>
    <td>Analytics</td>
    <td><li>Exibir Relatórios de Desempenho Global</li>
    <li>Exibir Relatórios de Bate-papo ao Vivo</li>
    <li>Exibir Relatórios de Reuniões</li>
    <li>Exportar relatórios</li></td>
  </tr>
  <tr>
    <td>Configurações do agente</td>
    <td><li>Gerenciar Disponibilidade do Live Chat</li>
    <li>Conectar seu calendário</li>
    <li>Gerenciar Disponibilidade de Calendário</li></td>
  </tr>
  <tr>
    <td>Configurações de admin</td>
    <td><li>Exibir Round-robin</li>
    <li>Exibir Regras Personalizadas</li>
    <li>Gerenciar regras personalizadas (adicionar, editar, excluir)</li>
    <li>Exibir Lista de Contas <b>*</b></li>
    <li>Gerenciar Contas (adicionar, editar, excluir) <b>*</b></li>
    <li>Gerenciar configurações de Chatbot</li>
    <li>Gerenciar configurações de fluxos de conversa</li>
    <li>Gerenciar privacidade e segurança</li>
    <li>Gerenciar integrações</li>
    <li>Gerenciar agentes</li>
    <li>Exibir Equipes de Agentes <b>*</b></li>
    <li>Gerenciar Equipes de Agentes (adicionar, editar, excluir) <b>*</b></li></td>
  </tr>
</tbody>
</table>

**&#42;** Atualmente disponível apenas para usuários do Dynamic Prime

<p>

## Permissões de perfil padrão {#default-profile-permissions}

Abaixo estão os cinco perfis padrão e as permissões que são ativadas por padrão.

<table>
<thead>
  <tr>
    <th style="width:25%">Perfil</th>
    <th>Permissões padrão</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Usuário de campanha de marketing</td>
    <td><i>Gerenciamento de Conversas</i>
    <li>Exibir caixas de diálogo</li>
    <li>Gerenciar caixas de diálogo (criar, excluir)</li>
    <li>Caixas de diálogo do Publish</li>
    <li>Exibir Fluxos de Conversa</li>
    <li>Gerenciar Fluxos de Conversação (criar, excluir)</li>
    <li>Fluxos de conversa do Publish</li>
    <br>
    <i>Chat ao vivo</i>
    <li>n/d</li>
    <br>
    <i>Reuniões</i>
    <li>n/d</li>
    <br>
    <i>Análises</i>
    <li>Exibir Relatórios de Desempenho Global</li>
    <li>Exibir Relatórios de Bate-papo ao Vivo</li>
    <li>Exibir Relatórios de Reuniões</li>
    <br>
    <i>Configurações do agente</i>
    <li>n/d</li>
    <br>
    <i>Configurações do administrador</i>
    <li>Exibir Round-robin</li>
    <li>Exibir Regras Personalizadas</li>
    <li>Exibir Lista de Contas <b>*</b></li>
    <li>Exibir Equipes de Agentes <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>LiveAgent</b></td>
    <td><i>Gerenciamento de Conversas</i>
    <li>Exibir caixas de diálogo</li>
    <li>Exibir Fluxos de Conversa</li>
    <br>
    <i>Chat ao vivo</i>
    <li>Exibir minhas conversas</li>
    <br>
    <i>Reuniões</i>
    <li>n/d</li>
    <br>
    <i>Análises</i>
    <li>Exibir Relatórios de Desempenho Global</li>
    <li>Exibir Relatórios de Bate-papo ao Vivo</li>
    <li>Exibir Relatórios de Reuniões</li>
    <br>
    <i>Configurações do agente</i>
    <li>Gerenciar Disponibilidade do Live Chat</li>
    <li>Conectar seu calendário</li>
    <li>Gerenciar Disponibilidade de Calendário</li>
    <br>
    <i>Configurações do administrador</i>
    <li>Exibir Round-robin</li>
    <li>Exibir Regras Personalizadas</li>
    <li>Exibir Lista de Contas <b>*</b></li>
    <li>Exibir Equipes de Agentes <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Agente de calendário</b></td>
    <td><i>Gerenciamento de Conversas</i>
    <li>Exibir caixas de diálogo</li>
    <li>Exibir Fluxos de Conversa</li>
    <br>
    <i>Chat ao vivo</i>
    <li>n/d</li>
    <br>
    <i>Reuniões</i>
    <li>n/d</li>
    <br>
    <i>Análises</i>
    <li>Exibir Relatórios de Desempenho Global</li>
    <li>Exibir Relatórios de Bate-papo ao Vivo</li>
    <li>Exibir Relatórios de Reuniões</li>
    <br>
    <i>Configurações do agente</i>
    <li>Conectar seu calendário</li>
    <li>Gerenciar Disponibilidade de Calendário</li>
    <br>
    <i>Configurações do administrador</i>
    <li>Exibir Round-robin</li>
    <li>Exibir Regras Personalizadas</li>
    <li>Exibir Lista de Contas <b>*</b></li>
    <li>Exibir Equipes de Agentes <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Administrador de marketing</b></td>
    <td><i>Gerenciamento de Conversas</i>
    <li>Exibir caixas de diálogo</li>
    <li>Gerenciar caixas de diálogo (criar, excluir)</li>
    <li>Caixas de diálogo do Publish</li>
    <li>Exibir Fluxos de Conversa</li>
    <li>Gerenciar Fluxos de Conversação (criar, excluir)</li>
    <li>Fluxos de conversa do Publish</li>
    <br>
    <i>Chat ao vivo</i>
    <li>n/d</li>
    <br>
    <i>Reuniões</i>
    <li>n/d</li>
    <br>
    <i>Análises</i>
    <li>Exibir Relatórios de Desempenho Global</li>
    <li>Exibir Relatórios de Bate-papo ao Vivo</li>
    <li>Exibir Relatórios de Reuniões</li>
    <li>Exportar relatórios</li>
    <br>
    <i>Configurações do agente</i>
    <li>n/d</li>
    <br>
    <i>Configurações do administrador</i>
    <li>Exibir Round-robin</li>
    <li>Exibir Regras Personalizadas</li>
    <li>Gerenciar regras personalizadas (adicionar, editar, excluir)</li>
    <li>Exibir Lista de Contas <b>*</b></li>
    <li>Gerenciar Contas (adicionar, editar, excluir) <b>*</b></li>
    <li>Gerenciar configurações de Chatbot</li>
    <li>Gerenciar configurações de fluxos de conversa</li>
    <li>Gerenciar privacidade e segurança</li>
    <li>Gerenciar integrações</li>
    <li>Exibir Equipes de Agentes <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Administrador de Vendas</b></td>
    <td><i>Gerenciamento de Conversas</i>
    <li>Exibir caixas de diálogo</li>
    <li>Exibir Fluxos de Conversa</li>
    <br>
    <i>Chat ao vivo</i>
    <li>Exibir minhas conversas</li>
    <li>Exibir Todas as Conversas</li>
    <br>
    <i>Reuniões</i>
    <li>Gerenciar Todas as Reuniões</li>
    <br>
    <i>Análises</i>
    <li>Exibir Relatórios de Desempenho Global</li>
    <li>Exibir Relatórios de Bate-papo ao Vivo</li>
    <li>Exibir Relatórios de Reuniões</li>
    <li>Exportar relatórios</li>
    <br>
    <i>Configurações do agente</i>
    <li>Gerenciar Disponibilidade do Live Chat</li>
    <li>Conectar seu Calendário</li>
    <li>Gerenciar Disponibilidade de Calendário</li>
    <br>
    <i>Configurações do administrador</i>
    <li>Exibir Round-robin</li>
    <li>Exibir Regras Personalizadas</li>
    <li>Gerenciar regras personalizadas (adicionar, editar, excluir)</li>
    <li>Exibir Lista de Contas <b>*</b></li>
    <li>Gerenciar Contas (adicionar, editar, excluir) <b>*</b></li>
    <li>Gerenciar agentes</li>
    <li>Exibir Equipes de Agentes <b>*</b></li>
    <li>Gerenciar Equipes de Agentes <b>*</b></li>
    </td>
  </tr>
</tbody>
</table>

**&#42;** Atualmente disponível apenas para usuários do Dynamic Prime
