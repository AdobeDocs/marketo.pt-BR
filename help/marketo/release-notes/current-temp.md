---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: c353425db0dc8b08620feb68092b25c664111a03
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 49%

---

# Notas de versão: janeiro de 2026 {#release-notes-jan-26}

Abaixo você encontrará todos os recursos incluídos na versão de janeiro de 2026. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 30 de janeiro de 2026**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Gerenciar marcas (beta)</strong>: gere conteúdo de email com base nas diretrizes de redação de cópia específicas de sua organização/marca.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Aprimoramento do Email Designer - Assistente de IA</strong>: agora você pode adicionar ativos de marca diretamente ao seu prompt e pedir ao modelo para consultar essa fonte para gerar conteúdo, em vez de adicionar manualmente um ativo de marca como um arquivo.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Visualizações Visuais de Fragmentos</strong>: todos os Fragmentos publicados agora aparecem como miniaturas, tornando muito mais rápido identificar o que você precisa.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Marcadores</strong>: agora é possível criar marcadores de vários níveis ao criar um email no Email Designer.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Aprimoramentos de Conteúdo Condicional</strong>: paridade com o recurso <i>Conteúdo Dinâmico</i> no editor de email antigo.
   <ul>
   <li>O conteúdo condicional agora se aplica à Segmentação em pastas compartilhadas.</li>
   <li>Agora as segmentações são classificadas em ordem alfabética.</li>
   </ul>
   </td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Pastas</strong>: Agora é possível organizar seus ativos criados usando o Email Designer (emails, modelos de email, fragmentos) com pastas.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Recursos do ciclo de lançamento não padrão {#non-standard-release-cycle-features}

Os recursos a seguir foram lançados fora do ciclo de lançamento padrão do Marketo Engage.

### Webinários interativos {#interactive-webinars}

* **Pod de pesquisa**: um novo Pod de pesquisa permite que os hosts projetem e entreguem formulários de feedback estruturados diretamente em uma sessão em tempo real.

* **Pod de recursos**: o novo Pod de recursos substitui os pods de arquivos e links da Web anteriores, fornecendo uma maneira única e unificada de compartilhar recursos durante as sessões ativas.

* **Experiência aprimorada com a interface do quarto**: aproveite uma interface do quarto mais moderna e atualizada, criada com base na estrutura de design mais recente do Spectrum 2 da Adobe, alinhada com a linguagem visual usada em outros produtos da Adobe, como o Creative Cloud e o Experience Cloud.

Visite [esta página](https://helpx.adobe.com/br/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"} para obter detalhes completos.

## Anúncios {#announcements}

* **Migração da comunidade do Marketo concluída**: a nova Comunidade da Adobe Experience League agora está ativa. [Foram feitos vários aprimoramentos](https://experienceleaguecommunities.adobe.com/community-pulse-blog-34/community-update-streamlined-ways-to-engage-and-a-redesigned-homepage-247673?profile.language=pt){target="_blank"} para melhorar ainda mais a sua experiência com a Marketo Community. [Confira](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-26?profile.language=pt){target="_blank"}.

* **Descontinuação do parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo será descontinuado e não estará disponível após quarta-feira, 31 de março de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API SOAP**: o suporte para a API SOAP do Marketo terminará em quarta-feira, 31 de março de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Fim da Vida Útil da Identidade do Marketo Engage**:

   * _Descontinuação de restrições de IP_: o suporte para a [restrição de logons do Marketo com base no IP](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. Um novo recurso de controle de acesso baseado em localização para a Identidade da Adobe no Adobe Admin Console será lançado em breve.

   * _Descontinuação do logon único (SSO)_: o suporte para o [SSO da Identidade do Marketo](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. O logon único (SSO) para a Identidade da Adobe no Adobe Admin Console deve ser configurado separadamente. Para ver as etapas de configuração, consulte [Configurar identidade e logon único](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.
