---
description: Notas de versão - setembro de 2025 - Documentação do Marketo - Documentação do produto
title: Notas de versão — Setembro de 2025
feature: Release Information
exl-id: fd40d9df-67ba-4fc4-891f-81aebfd07b0a
TQID: https://experienceleague.adobe.com/WfcIv3NWuYLgVCvHGcGmKbE6pDLOJ6FBk0OAX5uNJDE
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 960
ht-degree: 85%

---

# Notas de versão: setembro de 2025 {#release-notes-sep-25}

Abaixo é possível encontrar todos os recursos incluídos na versão de setembro de 2025. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **19 de setembro de 2025**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Retenção de atividade do webinário sob demanda</strong>: os usuários de webinários interativos agora têm dados do Painel de webinários sob demanda disponíveis por mais de 30 dias (anteriormente, era apenas até 30 dias a partir do dia do webinário).</td>
   <td>Lançado</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/event-workflows#manual-sync">Sincronização manual</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de email — Permissões do Assistente de IA</strong>: os administradores do Marketo podem fornecer a usuários específicos acesso aos recursos de GenAI.</td>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/ai-assistant.md#set-up-permissions">Configurar permissões</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de email — modo escuro</strong>: agora é possível utilizar o modo escuro, que permite que clientes de email e aplicativos compatíveis exibam emails com fundos mais escuros e cores mais claras para textos, botões e outros elementos da IU.</td>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md">Modo escuro</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de email — fluxo de trabalho de colaboração de conteúdo</strong>: agora é possível comentar e colaborar com outros usuários do Marketo dentro de um ativo de email. Marque membros da equipe (usuários do Marketo que têm as permissões de ativos apropriadas) e esses membros receberão uma notificação de email ou de pulso.</td>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/email-collaboration.md">Colaboração por email</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de email — Correções de redirecionamento</strong>: alguns usuários estavam tendo problemas de redirecionamento com URLs para emails criados com o novo Designer (por exemplo, colar diretamente os URLs ou marcar ativos de email nem sempre funcionava). Esse problema foi resolvido. Além disso, os links para ativos de email em <b>Modelos de email</b> &gt; <b>Detalhes</b> &gt; <b>Usados por</b> redirecionarão para o ativo de email correspondente.</td>
   <td>Lançado</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Descontinuação da barra dupla na API REST**: em 16 de setembro de 2025, a Adobe fez a transição para uma infraestrutura de hospedagem mais moderna para URLs da API REST que usam tecnologia mais recente, adicionando segurança e escalabilidade. Se sua assinatura tem usado APIs com uma barra dupla (//) no URL, leia [esta publicação da Nation](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} para saber as próximas etapas.

* **Retorno ao Velocity Scripting no novo Designer de email**: o Adobe Marketo Engage lançou um recurso chamado _Conteúdo condicional_ para o novo Designer de email em junho. O recurso era alimentado por scripts Handlebar, em vez de scripts Velocity, em um esforço para fornecer um pouco mais de flexibilidade no conteúdo dinâmico. Mas, quando descobrimos que isso estava causando a resolução incorreta de alguns tokens, decidimos desabilitá-lo temporariamente. [Saiba mais](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Fim da vida útil da Identidade do Marketo Engage**: em agosto de 2025, a Adobe começou o processo de remoção do suporte à Identidade do Marketo Engage (logon via `login.marketo.com`). Para evitar a interrupção do acesso ao Marketo Engage, você deve fazer a transição para a [Identidade da Adobe](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} até no máximo 30 de setembro de 2025.

   * _Descontinuação de restrições de IP_: o suporte para a [restrição de logons do Marketo com base no IP](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. Um novo recurso de controle de acesso baseado em localização para a Identidade da Adobe no Adobe Admin Console será lançado em breve.

   * _Descontinuação do logon único (SSO)_: o suporte para o [SSO da Identidade do Marketo](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. O logon único (SSO) para a Identidade da Adobe no Adobe Admin Console deve ser configurado separadamente. Para ver as etapas de configuração, consulte [Configurar identidade e logon único](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

* **Descontinuação do recurso _Encaminhar para um amigo_**: em 29 de setembro de 2025, o recurso _Encaminhar para um amigo_ nos emails do Marketo Engage 2.0 (o editor de email legado) será completamente descontinuado para todas as assinaturas. Isso afeta o token “Encaminhar para um amigo” e os links “Encaminhar para um amigo” em emails que já foram ou serão enviados usando o token. [Saiba mais](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Descontinuação do parâmetro “access_token” da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo será descontinuado e não estará disponível após 31 de março de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API SOAP**: o suporte para a API SOAP do Marketo terminará em 31 de março de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Substituição do Fluxo de Dados de Atividades de Clientes Potenciais Herdados**: até o final de junho de 2026, os usuários deverão migrar do Fluxo de Dados de Atividades de Clientes Potenciais herdado para o novo Fluxo de Dados de Atividades de Clientes Potenciais (LADS) do Adobe I/O. Essa descontinuação afeta apenas alguns usuários que foram integrados ao fluxo de dados da atividade principal antes de ele ser integrado ao Adobe I/O Events. Se você for um usuário de fluxos de dados mais recente ou já gerenciar o Fluxo de dados da atividade principal por meio de Eventos de E/S, isso não terá impacto em você. Consulte [este artigo](https://developer.adobe.com/events/docs/guides/using/marketo/marketo-lead-activity-data-stream-migration){target="_blank"} para obter detalhes sobre a migração.
