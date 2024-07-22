---
description: Notas de versão atuais — Documentação do Marketo — Documentação do produto
title: Notas da versão atual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: cb69844d8e9e25cae19bc2d4a91c28376f58eadb
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 6%

---

# Notas de versão: julho de 2024 {#release-notes-july-24}

Abaixo você encontrará todos os recursos incluídos na versão de 24 de julho. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

As Notas de versão específicas para o Adobe Dynamic Chat [podem ser encontradas aqui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com o representante da Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **26 de julho de 2024**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Recurso</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
     <tr> 
   <td><strong>Painel de Envolvimento para Webinars interativos</strong>: obtenha uma exibição de desempenho de webinário agregado, bem como uma exibição abrangente do engajamento para cada participante durante o webinário, para que você possa decidir quais leads devem ser direcionados por meio das ferramentas de orquestração de Marketo Engage.</td> 
    <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Gerenciamento de Salas para Webinars Interativos</strong>: acesse salas individuais criadas (e faça modificações, se necessário), bem como acesse o conteúdo e a gravação (e limpe-as, se necessário, para otimizar o armazenamento).</td> 
    <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Personalização de webinários para webinários interativos</strong>: forneça uma experiência de marca uniforme e aprovada pela organização usando uma interface de sala comum, telas intermediárias (como telas de fundo de entrada de participantes), bem como telas de fundo de vídeo personalizadas, para que a estratégia do webinário possa se alinhar mais facilmente à estratégia da marca.</td> 
    <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Alteração na API REST do Marketo</strong>: estamos introduzindo uma pequena alteração na <a href="https://developers.marketo.com/rest-api/user-management/">API de Gerenciamento de Usuários</a>. Agora os pontos de extremidade <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Procurar Usuários</a> e <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Excluir Usuário</a> oferecem suporte a <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Gerenciamento de Conta de Destino</a> usuários.</td> 
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anúncios {#announcements}

* **Novo site de documentação do desenvolvedor**: como parte de nosso esforço contínuo para aprimorar a experiência do usuário do Marketo Engage, migraremos toda a documentação do desenvolvedor para o site da Adobe Experience League e do Adobe Developer em julho de 2024. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Descontinuação do Token de Acesso no Parâmetro de Consulta**: o suporte para autenticação usando tokens de acesso em um parâmetro de consulta de uma chamada à API REST do Marketo Engage será removido em uma versão futura (data específica a ser definida). As integrações existentes devem migrar para o uso do cabeçalho de Autorização [descrito aqui](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. O novo desenvolvimento deve usar somente o cabeçalho de autorização para autenticação com Marketo Engage.

* **Reautenticação do LinkedIn necessária**: a LinkedIn está atualizando suas APIs de marketing usadas pelas integrações do Marketo Engage LinkedIn. Essas alterações exigirão a reautenticação de todos os serviços do LinkedIn LaunchPoint no menu **Admin** > **LaunchPoint** entre 26 de julho e 15 de dezembro de 2024 para evitar a interrupção do serviço. Você pode encontrar instruções sobre como fazer isso [aqui para a Geração de Clientes Potenciais Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} e [aqui para Públicos Correspondentes](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. O serviço de formulário de geração de lead tem um tipo de &quot;Geração de lead da LinkedIn&quot; e o serviço de Público-alvo correspondente tem um tipo de &quot;Públicos-alvo correspondentes da LinkedIn&quot;. Para obter mais informações, consulte as [Perguntas frequentes sobre migração](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
