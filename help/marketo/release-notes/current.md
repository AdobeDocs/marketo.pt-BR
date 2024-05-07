---
description: Notas de versão atuais — Documentação do Marketo — Documentação do produto
title: Notas da versão atual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 0d2416651da183460ad1f60ff5d566cbfc7abd12
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 10%

---

# Notas de versão: abril de 2024 {#release-notes-apr-24}

Abaixo você encontrará todos os recursos incluídos na versão de abril de 2024. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

As notas de versão especificamente para o Adobe Dynamic Chat [pode ser encontrado aqui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **26 de abril de 2024**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Recurso</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
     <tr> 
   <td><strong>Melhorias nos webinários interativos</strong>: agora você pode fornecer aos hosts e apresentadores a capacidade de adicionar um título de webinário, renomear uma sala e sincronizar manualmente os dados de engajamento após a entrega do evento.</td> 
   <td>Remetido</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">Criar um webinário interativo</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">Sincronização manual</a></li></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Aprimoramentos da trilha de auditoria</strong>: agora novos tipos de ações podem ser capturados na Trilha de auditoria para alterações feitas no Gerenciamento de campo, alterações feitas nos Usuários e Funções e a contagem de pessoas exportadas de listas e Smart Lists.</td> 
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Permissões para novos usuários e funções</strong>: novas permissões estão disponíveis, fornecendo aos usuários acesso mais granular ao Marketo Engage. Controle partes do Administrador não previamente restritas, como Nova experiência e Públicos preditivos, divida permissões para conceder acesso à Trilha de auditoria de ativos e à Trilha de auditoria de administradores separadamente e utilize novas permissões de criação e movimentação para ativos e pastas, a fim de impedir que usuários somente leitura façam alterações. 
   <p>Embora as novas permissões apareçam em sua instância do Marketo Engage a partir de 26 de abril, elas estão passivas por enquanto e se tornarão acessíveis posteriormente neste trimestre.
   <li>Acessar o Adobe Experience Manager</li>
   <li>Mapeamento da organização do Adobe de acesso</li>
   <li>Acessar trilha de auditoria do administrador</li>
   <li>Acessar trilha de auditoria do ativo</li>
   <li>Acessar nova experiência</li>
   <li>Acessar públicos preditivos</li>
   <li>Criar relatório</li>
   <li>Criar lista</li>
   <li>Exportar atividade da campanha</li>
   </td> 
   <td>Remetido</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">Descrições de permissões de função</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anúncios {#announcements}

* **Atualização da API de atividades**: No dia 26 de abril, adicionamos vários novos atributos às atividades baseadas na Web e baseadas em email que são retornados quando você recupera atividades usando o [API REST DO MARKETO](https://developers.marketo.com/rest-api/lead-database/activities/){target="_blank"}. The activities listed below will now include Browser, Platform, Device, and User Agent attributes. Call the [Get Activity Types](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Activities/getAllActivityTypesUsingGET){target="_blank"} endpoint para analisar detalhes do atributo de cada atividade.

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
   <td>Enviar e-mail</td> 
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
   <td>Cliques em email</td> 
   <td>Navegador</td>
  </tr>
  <tr> 
   <td>E-mail foi devolvido temporariamente</td> 
   <td>Navegador, Plataforma, Dispositivo, Agente do Usuário</td>
  </tr>
 </tbody> 
</table>
