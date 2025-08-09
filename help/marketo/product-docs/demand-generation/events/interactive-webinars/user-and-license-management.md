---
description: Gerenciamento de usuários e licenças - Documentação do Marketo - Documentação do produto
title: Gerenciamento de usuários e licenças
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: fe167b4a70a23f129d56ed20ac6c1ed1130049ef
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 2%

---

# Gerenciamento de usuários e licenças {#user-and-license-management}

Saiba como adicionar e remover usuários, além de visualizar suas licenças atuais.

## Adicionar um usuário {#add-a-user}

1. Vá para a área **Administrador**.

   ![](assets/user-and-license-management-1.png)

1. Clique em **Webinars interativos**.

   ![](assets/user-and-license-management-2.png)

1. Clique em **Adicionar/Remover Usuários**.

   ![](assets/user-and-license-management-3.png)

1. Clique na lista suspensa Usuários Disponíveis, selecione o(s) usuário(s) que deseja adicionar e clique em **OK**.

   ![](assets/user-and-license-management-4.png)

## Remover um usuário {#remove-a-user}

1. Vá para a área **Administrador**.

   ![](assets/user-and-license-management-5.png)

1. Clique em **Webinars interativos**.

   ![](assets/user-and-license-management-6.png)

1. Clique em **Adicionar/Remover Usuários**.

   ![](assets/user-and-license-management-7.png)

1. Realce o(s) usuário(s) que deseja remover e pressione a tecla Delete. Clique em **OK** quando terminar.

   ![](assets/user-and-license-management-8.png)

## Uso da licença {#license-usage}

Webinars interativos oferecem licenças específicas para criar eventos viabilizados pelo Adobe Connect. Toda vez que uma licença é adicionada, uma nova caixa de uso de licença será exibida. Os administradores do Marketo podem visualizar (não editar) as licenças seguindo as etapas abaixo. Entre em contato com a Equipe de conta da Adobe (seu Gerente de conta) para obter licenças adicionais.

1. Vá para a área **Administrador**.

   ![](assets/user-and-license-management-9.png)

1. Clique em **Webinars interativos**.

   ![](assets/user-and-license-management-10.png)

1. Role para baixo até o(s) cartão(ões) de Uso de licença.

   ![](assets/user-and-license-management-11.png)

<table>
  <tr>
   <td width="20%"><b>Data de início</b></td>
   <td width="80%">Data de início da licença.</td>
  </tr>
  <tr>
   <td width="20%"><b>Data de validade</b></td>
   <td width="80%">Data de expiração da licença.</td>
  </tr>
  <tr>
   <td width="20%"><b>Tipo</b></td>
   <td width="80%">O tipo de licença adquirida. Há três tipos disponíveis: Licença de eventos compartilhados, Licença de salas compartilhadas, Licença de armazenamento adicional.</td>
  </tr>
  <tr>
   <td width="20%"><b>Capacidade do evento</b></td>
   <td width="80%">O número máximo de participantes que podem ser acomodados em um evento.</td>
  </tr>
  <tr>
   <td width="20%"><b>Total de eventos</b></td>
   <td width="80%">O número total de eventos que foram provisionados com esta licença.</td>
  </tr>
  <tr>
   <td width="20%"><b>Eventos consumidos</b></td>
   <td width="80%">Todos os eventos concluídos e agendados no momento. <a href="#things-to-note">saiba mais</a></td>
  </tr>
  <tr>
   <td width="20%"><b>Capacidade de armazenamento</b></td>
   <td width="80%">Quantidade de armazenamento disponível para armazenar gravações, material de apoio, imagens principais, documentação e outros ativos.</td>
  </tr>
  </tbody>
</table>

### Itens a Observar {#things-to-note}

* Toda vez que um evento é criado, ele é contado como &quot;consumido&quot; de sua respectiva licença (a menos que seja uma Licença de sala compartilhada). Será dada preferência à &quot;Licença de evento compartilhado&quot; se houver a &quot;Licença de evento compartilhado&quot; e a &quot;Licença de quarto compartilhado&quot; com a mesma capacidade. Se o evento não tiver sido entregue e o Programa de evento for excluído antes do horário agendado, a contagem de eventos será reposta. Se o evento não for entregue e o Programa de evento não for excluído antes do horário programado, o evento não será reposto.

* O tipo &quot;Licença de Armazenamento Adicional&quot; apenas fornece armazenamento, portanto, o valor em cada campo _além de_ Capacidade de Armazenamento será listado simplesmente como &quot;-&quot;.

* O tipo &quot;Licença de quarto compartilhado&quot; tem eventos ilimitados e &quot;Licença de armazenamento adicional&quot; apenas fornece armazenamento, portanto, o campo Total de eventos para essas licenças será listado simplesmente como &quot;-&quot;.

* Depois que uma licença for esgotada, seu bloco permanecerá na tela Webinars interativos na seção de Administrador com &quot;Total de eventos&quot; e &quot;Eventos consumidos&quot; tendo o mesmo valor. Somente quando a licença expirar ela será removida da tela.

## Acesso de usuário {#user-access}

Os Webinars interativos têm a funcionalidade de regular o uso, dando permissões aos usuários do Marketo Engage para criar e fornecer Webinars interativos. No entanto, um usuário do Webinar interativo (ou não usuário) ainda poderia ter acesso de leitura/edição aos programas de eventos de Webinars interativos criados por outros usuários.

Os usuários do Marketo que receberam permissões de Webinars interativos e são proprietários de um Programa de evento de Webinars interativos específico poderiam executar todas as funções do Webinar interativo relacionadas a esse programa. Isso inclui: criar, acessar, modificar, clonar, mover e excluir esse programa. No entanto, uma vez que esse usuário não é mais um usuário de webinário interativo, o proprietário do programa poderá acessar e mover o programa, mas não executar outras funções.

Os usuários do Marketo que receberam permissões de Webinars interativos e que são _não_ proprietários de um Programa de evento de Webinars interativos específico poderiam executar funções limitadas nesses programas. Os usuários não administradores do Marketo poderão acessar e clonar o programa, mas não poderão executar outras funções se tiverem permissões para Webinars interativos. No entanto, os usuários Administradores do Marketo _poderão_ executar todas as funções, como acessar, modificar, clonar, mover e excluir esse programa (desde que tenham permissões para Webinars interativos). Quando essa permissão for revogada para usuários administradores e não administradores do Marketo, eles poderão acessar somente o Programa de evento de webinário interativo e não poderão executar outras funções.

A restrição de funções acionáveis seria indicada por um botão de ação esmaecido e uma mensagem de mouse. Alguns exemplos dos botões de ação esmaecidos são &quot;Projetar o webinário&quot; ou &quot;Inserir o webinário&quot;. Para funções não acionáveis, será fornecida uma mensagem destacando as restrições. Veja o exemplo abaixo:

![](assets/user-and-license-management-12.png)
