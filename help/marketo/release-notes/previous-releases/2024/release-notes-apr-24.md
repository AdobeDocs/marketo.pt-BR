---
description: Notas de versão - abril de 2024 - Documentação do Marketo - Documentação do produto
title: Notas de versão – Abril de 2024
feature: Release Information
exl-id: d87474f8-fc47-407b-bc97-e343b56c1f8f
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 31%

---

# Notas de versão: abril de 2024 {#release-notes-apr-24}

Abaixo você encontrará todos os recursos incluídos na versão de abril de 2024. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 26 de abril de 2024**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
     <tr>
   <td><strong>Aprimoramentos nos webinários interativos</strong>: agora você pode fornecer aos hosts e apresentadores a capacidade de adicionar um título de webinário, renomear uma sala e sincronizar manualmente os dados de envolvimento após a entrega do evento.</td>
   <td>Lançado</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">Criar um webinário interativo</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">Sincronização manual</a></li></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Aprimoramentos da Trilha de Auditoria</strong>:
   Agora novos tipos de ações podem ser capturados na Trilha de auditoria para alterações feitas no Gerenciamento de campo, alterações feitas nos Usuários e Funções e a contagem de pessoas exportadas de listas e Smart Lists.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Novas Permissões de Usuários e Funções</strong>: novas permissões estão disponíveis, fornecendo aos usuários acesso mais granular ao Marketo Engage. Controle partes do Administrador não previamente restritas, como Nova experiência e Públicos preditivos, divida permissões para conceder acesso à Trilha de auditoria de ativos e à Trilha de auditoria de administradores separadamente e utilize novas permissões de criação e movimentação para ativos e pastas, a fim de impedir que usuários somente leitura façam alterações.
   <p>Embora as novas permissões apareçam em sua instância do Marketo Engage a partir de 26 de abril, elas estão passivas por enquanto e se tornarão acessíveis posteriormente neste trimestre.
   <li>Acessar o Adobe Experience Manager</li>
   <li>Acessar o mapeamento de organização da Adobe</li>
   <li>Acessar trilha de auditoria do administrador</li>
   <li>Acessar trilha de auditoria do ativo</li>
   <li>Acessar nova experiência</li>
   <li>Acessar públicos preditivos</li>
   <li>Criar relatório</li>
   <li>Criar lista</li>
   <li>Exportar atividade da campanha</li>
   </td>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">Descrições de permissões de função</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Atualização da API de atividades**: no dia 26 de abril, adicionamos vários novos atributos às atividades baseadas na Web e por email que são retornados quando você recupera atividades usando a [API REST do Marketo](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities){target="_blank"}. As atividades listadas abaixo agora incluirão atributos de navegador, plataforma, dispositivo e agente do usuário. Chame o ponto de extremidade [Obter Tipos de Atividade](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/getAllActivityTypesUsingGET){target="_blank"} para analisar os detalhes do atributo de cada atividade.

**Atividades baseadas na Web**

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:30%">Atividade</th>
   <th style="width:70%">Atributos recém-adicionados</th>
   </tr>
  <tr>
   <td>Visit Webpage</td>
   <td>Navegador, plataforma, dispositivo</td>
  </tr>
   <tr>
   <td>Preenchimento de formulário</td>
   <td>Navegador, plataforma, dispositivo</td>
  </tr>
  <tr>
   <td>Clicar em link</td>
   <td>Navegador, plataforma, dispositivo</td>
  </tr>
 </tbody>
</table>

**Atividades baseadas em email**

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:30%">Atividade</th>
   <th style="width:70%">Atributos recém-adicionados</th>
  </tr>
   <tr>
   <td>Enviar email</td>
   <td>Navegador, Plataforma, Dispositivo, Agente do Usuário</td>
  </tr>
   </tr>
  <tr>
   <td>E-mail enviado</td>
   <td>Navegador, Plataforma, Dispositivo, Agente do Usuário</td>
  </tr>
   <tr>
   <td>E-mail foi devolvido</td>
   <td>Navegador, Plataforma, Dispositivo, Agente do Usuário</td>
  </tr>
  <tr>
   <td>Cancelamento de inscrição do email</td>
   <td>Navegador, plataforma, dispositivo</td>
  </tr>
  <tr>
   <td>Abertura de email</td>
   <td>Navegador</td>
  </tr>
   <tr>
   <td>Cliques no email</td>
   <td>Navegador</td>
  </tr>
  <tr>
   <td>E-mail foi devolvido temporariamente</td>
   <td>Navegador, Plataforma, Dispositivo, Agente do Usuário</td>
  </tr>
 </tbody>
</table>
