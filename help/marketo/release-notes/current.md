---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 60%

---

# Notas de versão: setembro de 2025 {#release-notes-sep-25}

Abaixo você encontrará todos os recursos incluídos na versão de setembro de 2025. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 19 de setembro de 2025**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Retenção de atividade do webinário sob demanda</strong>: os usuários de webinários interativos agora têm dados do Painel de webinários sob demanda disponíveis por mais de 30 dias (anteriormente, eram apenas até 30 dias a partir do dia do webinário).</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Fluxo de trabalho do Email Designer - Collaboration de Conteúdo</strong>: Agora você pode comentar e colaborar com outros usuários do Marketo em um ativo de email. Os membros da equipe de tags (usuários do Marketo que têm as permissões de ativo apropriadas) e receberão uma notificação por email ou por pulso.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Permissões do Assistente de IA</strong>: os administradores do Marketo podem fornecer a usuários específicos acesso aos recursos do GenAI.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Modo Escuro</strong>: agora você pode utilizar o Modo Escuro, que permite que clientes e aplicativos de email de suporte exibam emails com planos de fundo mais escuros e cores mais claras para texto, botões e outros elementos da interface do usuário.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Correções de redirecionamento</strong>: alguns usuários estavam com problemas de redirecionamento de URLs para emails criados com o novo Designer (por exemplo, colar diretamente as URLs ou marcar ativos de email nem sempre funcionava). Esse problema foi resolvido. Além disso, os links para ativos de email de <b>Modelos de email</b> &gt; <b>Detalhes</b> &gt; <b>Usados por</b> redirecionarão para o ativo de email correspondente.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Alternando de volta para o script do Velocity no novo Designer de email**: a Adobe Marketo Engage lançou um recurso chamado _Conteúdo condicional_ para o novo Designer de email em junho passado. O recurso era alimentado por scripts Handlebar em vez de scripts Velocity, em um esforço para fornecer um pouco mais de flexibilidade em seu conteúdo dinâmico. Mas quando descobrimos que isso estava fazendo com que alguns tokens fossem resolvidos incorretamente, decidimos desativá-los temporariamente. [Saiba mais](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Fim da vida útil da Identidade do Marketo Engage**: em agosto de 2025, a Adobe começou o processo de remoção do suporte à Identidade do Marketo Engage (logon via `login.marketo.com`). Para evitar a interrupção do acesso ao Marketo Engage, você deve fazer a transição para a [Identidade da Adobe](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} até no máximo 30 de setembro de 2025.

   * _Descontinuação de restrições de IP_: o suporte para a [restrição de logons do Marketo com base no IP](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. Um novo recurso de controle de acesso baseado em localização para a Identidade da Adobe no Adobe Admin Console será lançado em breve.

   * _Descontinuação do logon único (SSO)_: o suporte para o [SSO da Identidade do Marketo](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. O logon único (SSO) para a Identidade da Adobe no Adobe Admin Console deve ser configurado separadamente. Para ver as etapas de configuração, consulte [Configurar identidade e logon único](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

* **Descontinuação do recurso _Encaminhar para um amigo_**: em 29 de setembro de 2025, o recurso _Encaminhar para um amigo_ nos emails do Marketo Engage 2.0 (o editor de email legado) será completamente descontinuado para todas as assinaturas. Isso afeta o token “Encaminhar para um amigo” e os links “Encaminhar para um amigo” em emails que já foram ou serão enviados usando o token. [Saiba mais](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Descontinuação do parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo será descontinuado e não estará disponível após 31 de outubro de 2025. Todas as integrações novas e existentes devem autenticar chamadas da API REST usando o cabeçalho &#39;Authorization&#39;, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API SOAP**: o suporte para a API SOAP do Marketo terminará em 31 de outubro de 2025. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
