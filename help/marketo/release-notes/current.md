---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 015ece7d2ad38f6e0c957298bce432316e8d9efa
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 44%

---

# Notas de versão: agosto de 2025 {#release-notes-aug-25}

Abaixo você encontrará todos os recursos incluídos na versão de agosto de 2025. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 22 de agosto de 2025**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Relatórios</strong>: os relatórios de Desempenho de email e Desempenho de link de email agora mostram dados de emails criados usando o novo Email Designer.</td>
   <td>Enviado</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de email - Remoção de preenchimento automático</strong>: a opção de preenchimento automático no editor de personalização de token apontava para objetos incorretos e foi removida. Não há planos para reimplementá-lo neste momento.</td>
   <td>Enviado</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Otimização da Visualização de Email</strong>: alguns usuários experimentavam tempos de carregamento mais lentos ao tentar visualizar seus emails na página de detalhes do email/modelo/fragmento de email. Essa experiência foi otimizada para tempos de carregamento até 60% mais rápidos.</td>
   <td>Enviado</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Correções de Modelos</strong>: alguns modelos prontos para uso tinham problemas de renderização (por exemplo, não renderização correta em determinados navegadores/modo escuro, imagens desalinhadas, botões do CTA no local errado e alguns outros). Tudo isso foi corrigido nesta versão.</td>
   <td>Enviado</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Correção de Bloqueio de Conteúdo do Designer - </strong>: anteriormente, se um modelo de email fosse criado com bloqueio de conteúdo e o modelo fosse usado para criar um email, o bloqueio de conteúdo persistiria mesmo quando o email fosse redefinido ou o "design de alteração" fosse selecionado. Esse problema foi corrigido nesta versão.</td>
   <td>Enviado</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Permissão para editar limites do Smart Campaign</strong>: agora os administradores podem restringir a capacidade de modificar limites do Smart Campaign somente para usuários com permissões.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Fim da vida útil da Marketo Engage Identity**: em agosto de 2025, a Adobe começou a cancelar o suporte à Marketo Engage Identity (fazendo logon via `login.marketo.com`). Para evitar a interrupção do acesso ao Marketo Engage, você deve fazer a transição para a [Identidade da Adobe](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} até no máximo 30 de setembro de 2025.

   * _Descontinuação de Restrições de IP_: O suporte para [Restrição de Logons do Marketo com Base no IP](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. Um novo recurso de controle de acesso baseado em localização para a Adobe Identity na Adobe Admin Console será adicionado em breve.

   * _Descontinuação do SSO (Logon Único)_: o suporte para o [SSO da Identidade Marketo](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. O logon único (SSO) para a Identidade da Adobe no Adobe Admin Console deve ser configurado separadamente. Para ver as etapas de configuração, consulte [Configurar identidade e logon único](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

* **Descontinuação do recurso _Encaminhar para um Amigo_**: em 29 de setembro de 2025, o recurso _Encaminhar para um Amigo_ nos emails do Marketo Engage 2.0 (o editor de email herdado) será completamente descontinuado para todas as assinaturas. Isso afeta os links &quot;Encaminhar para um amigo&quot; e &quot;Encaminhar para um amigo&quot; em emails que já foram ou serão enviados usando o token. [Saiba mais](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Descontinuação do parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo será descontinuado e não estará disponível após 31 de outubro de 2025. Todas as integrações novas e existentes devem autenticar chamadas da API REST usando o cabeçalho &#39;Authorization&#39;, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API SOAP**: o suporte para a API SOAP do Marketo terminará em 31 de outubro de 2025. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
