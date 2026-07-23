---
description: Notas de versão - março de 2026 - Documentação do Marketo - Documentação do produto
title: Notas de versão - março de 2026
feature: Release Information
source-git-commit: e8663ada66948bc30ff7ad90b26f6ba75d670ae8
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 21%

---

# Notas de versão: março de 2026 {#release-notes-mar-26}

Abaixo você encontrará todos os recursos incluídos na versão de março de 2026. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **27 de março de 2026**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Gerenciar marcas (beta)</strong>: gere conteúdo de email com base nas diretrizes de redação de cópia específicas de sua organização/marca.</td>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/manage-brands.md" target="_blank">Criar e gerenciar marcas</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Componentes editáveis do HTML em fragmentos</strong>: dentro de fragmentos visuais, campos editáveis são suportados em componentes de imagem, texto e botão por meio do painel de propriedades do componente. Para componentes HTML, os campos editáveis são configurados de forma diferente, usando uma sintaxe baseada em variáveis dentro do código-fonte do próprio componente HTML.
   </td>
   <td>Lançado</i></td>
   <td><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/email-marketing/email-designer/customizable-fragments#editable-html" target="_blank">Componentes editáveis do HTML em fragmentos</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Ações Rápidas</strong>: <i>Paridade com o antigo editor de email</i>. As ações rápidas agora estão disponíveis para todos os ativos de email do Designer (emails, modelos de email, fragmentos). As ações rápidas compatíveis incluem: Duplicar, Excluir, Mover, Criar/Editar rascunho.
   </td>
   <td>Lançado</i></td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Correção de Renderização do Email Designer - Outlook</strong>: essa atualização corrige problemas de renderização, especialmente no MS Outlook. O Modo HTML avançado permite fazer pequenas edições de HTML/CSS ou adicionar tags de script ao modelo de email.
   </td>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/advanced-html-mode.md" target="_blank">Editar modelos de email com o editor avançado do HTML</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Verificador de pontuação da marca</strong>: avalie a qualidade do conteúdo geral para identificar possíveis problemas de legibilidade, coesão do conteúdo e eficácia, independentemente das diretrizes da sua marca.</td>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/brand-score.md" target="_blank">Pontuação da marca</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Notificações por push</strong>: os URIs de redirecionamento configurados nas mensagens de notificação por push agora oferecem suporte a tokens do Marketo Engage (aplicável somente a <i>URLs de aplicativos de inicialização</i>).
   </td>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md#redirect-uris">URIs de redirecionamento</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Descontinuação do recurso de SEO**: na terça-feira, 31 de março de 2026, o Marketo Engage descontinuará o recurso de Otimização do Mecanismo de Pesquisa (SEO). Se você não usa o SEO ativamente, não precisa fazer nada. Se você tiver usado o SEO recentemente, terá a opção de exportar seus dados. [Saiba mais](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617?profile.language=pt){target="_blank"}.

* **Limite de Clientes Potenciais de Mesclagem da API REST**: a partir de 31 de julho de 2026, as chamadas que incluírem mais de 25 IDs no parâmetro leadIds de uma chamada da API de Clientes Potenciais de Mesclagem resultarão em um código de erro 1080 e a chamada será ignorada. As tarefas que exigem a fusão de mais de 25 registros em um devem ser divididas em várias tarefas para garantir o sucesso dessas chamadas.

* **Descontinuação do Parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo está sendo descontinuado e não estará disponível após 31 de agosto de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API do SOAP**: o suporte para a API do Marketo SOAP terminará em 31 de julho de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
