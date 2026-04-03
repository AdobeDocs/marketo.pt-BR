---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 1850dd03baba259e99e8cc089b39f35735e63fdf
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 38%

---

# Notas de versão: março de 2026 {#release-notes-mar-26}

Abaixo você encontrará todos os recursos incluídos na versão de março de 2026. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 27 de março de 2026**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

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
   <td><strong>Email Designer - Verificador de qualidade da marca</strong>: avalie a qualidade do conteúdo geral para identificar possíveis problemas de legibilidade, consistência do conteúdo e eficácia, independentemente das diretrizes da sua marca.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Correção de Renderização do Email Designer - Outlook</strong>: essa atualização corrige problemas de renderização, especialmente no MS Outlook. O "modo Expert" permite fazer pequenas edições de HTML/CSS ou adicionar tags de script ao email (a prática recomendada é não fazer outras alterações no HTML do email para manter os elementos visuais como estão).
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
   <td><strong>Gerenciamento de lista de opções</strong>: agora é possível especificar os valores que podem ser usados em campos no Marketo Engage.
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
   <td><strong>Notificações por push</strong>: as URLs de redirecionamento configuradas nas mensagens de notificação por push agora oferecem suporte a tokens do Marketo Engage (aplicável somente a <i>URLs de aplicativos de inicialização</i>).
   </td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Descontinuação do recurso de SEO**: na terça-feira, 31 de março de 2026, o Marketo Engage descontinuará o recurso de Otimização do Mecanismo de Pesquisa (SEO). Se você não usa o SEO ativamente, não precisa fazer nada. Se você tiver usado o SEO recentemente, terá a opção de exportar seus dados. [Saiba mais](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617?profile.language=pt){target="_blank"}.

* **Limite de Clientes Potenciais de Mesclagem da API REST**: a partir de 31 de março de 2026, as chamadas que incluírem mais de 25 IDs no parâmetro leadIds de uma chamada da API de Clientes Potenciais de Mesclagem resultarão em um código de erro 1080 e a chamada será ignorada. As tarefas que exigem a fusão de mais de 25 registros em um devem ser divididas em várias tarefas para garantir o sucesso dessas chamadas.

* **Descontinuação do parâmetro “access_token” da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo será descontinuado e não estará disponível após sábado, 31 de julho de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API SOAP**: o suporte para a API SOAP do Marketo terminará em sábado, 31 de julho de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
