---
description: Notas de versão - julho de 2024 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Julho de 2024
feature: Release Information
exl-id: ff63af41-2d33-40f8-abca-3fd9493e7916
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 22%

---

# Notas de versão: julho de 2024 {#release-notes-july-24}

Abaixo você encontrará todos os recursos incluídos na versão de 24 de julho. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 26 de julho de 2024**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
     <tr>
   <td><strong>Painel de Envolvimento para Webinars interativos</strong>: obtenha uma exibição de desempenho de webinário agregado, bem como uma exibição abrangente do engajamento para cada participante durante o webinário, para que você possa decidir quais leads devem ser direcionados por meio das ferramentas de orquestração da Marketo Engage.</td>
    <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/engagement-dashboard.md" target="_blank">Painel de engajamento</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Gerenciamento de Salas para Webinars Interativos</strong>: acesse salas individuais criadas (e faça modificações, se necessário), bem como acesse o conteúdo e a gravação (e limpe-as, se necessário, para otimizar o armazenamento).</td>
    <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/room-management.md" target="_blank">Gerenciamento de salas</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Personalização de webinários para webinários interativos</strong>: forneça uma experiência de marca uniforme e aprovada pela organização usando uma interface de sala comum, telas intermediárias (como telas de fundo de entrada de participantes), bem como telas de fundo de vídeo personalizadas, para que a estratégia do webinário possa se alinhar mais facilmente à estratégia da marca.</td>
    <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/customization.md" target="_blank">Personalização de webinários interativos</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Alteração na API REST do Marketo</strong>: estamos introduzindo uma pequena alteração na <a href="https://developers.marketo.com/rest-api/user-management/">API de Gerenciamento de Usuários</a>. Agora os pontos de extremidade <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Procurar Usuários</a> e <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Excluir Usuário</a> oferecem suporte a <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Gerenciamento de Conta de Destino</a> usuários.</td>
   <td>Lançado</td>
   <td>n/d</td>
  </tr>
 </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Novo site de documentação do desenvolvedor**: como parte de nosso esforço contínuo para aprimorar a experiência do usuário do Marketo Engage, migraremos toda a documentação do desenvolvedor para a Adobe Experience League e o site da Adobe Developer em julho de 2024. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Descontinuação de recursos sociais**: na quarta-feira, 31 de julho de 2024, o Marketo Engage iniciará a desativação dos seguintes recursos sociais no produto:

   * Pesquisas
   * Botão de redes sociais
   * Oferta de recomendação
   * Compartilhamento de vídeo
   * Sorteios

Os usuários não poderão mais criar, clonar ou incorporar esses recursos do Social no Marketo Engage. Os ativos sociais existentes continuarão a funcionar até 31 de janeiro de 2025. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Descontinuação do Token de Acesso no Parâmetro de Consulta**: o suporte à autenticação usando tokens de acesso em um parâmetro de consulta de uma chamada da API REST do Marketo Engage será removido em uma versão futura (data específica a ser definida). As integrações existentes devem migrar para o uso do cabeçalho de Autorização [descrito aqui](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. O novo desenvolvimento deve usar somente o cabeçalho de Autorização para autenticação com o Marketo Engage.

* **Reautenticação do LinkedIn necessária**: o LinkedIn está atualizando as APIs de marketing usadas pelas integrações do Marketo Engage LinkedIn. Essas alterações exigirão reautenticação de todos os serviços do LinkedIn LaunchPoint no menu **Admin** > **LaunchPoint** entre 26 de julho e 15 de dezembro de 2024 para evitar a interrupção do serviço. Você pode encontrar instruções sobre como fazer isso [aqui para a Geração de Clientes Potenciais Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} e [aqui para Públicos Correspondentes](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. O serviço de formulário de geração de lead tem um tipo de &quot;Geração de lead do LinkedIn&quot; e o serviço de Público-alvo correspondente tem um tipo de &quot;Públicos-alvo correspondentes do LinkedIn&quot;. Para obter mais informações, visite as [Perguntas frequentes sobre migração](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
