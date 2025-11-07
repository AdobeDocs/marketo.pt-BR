---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: fdd1cc80d215fc7dee484a9e7b9fa640a47c4519
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 99%

---

# Notas de versão: outubro de 2025 {#release-notes-oct-25}

Abaixo você encontrará todos os recursos incluídos na versão de outubro de 2025. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **31 de outubro de 2025**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Designer de email — Importador de modelos (Beta)</strong>: importe modelos de email do editor de email clássico para criar modelos compatíveis com o novo designer de email no Design Studio.</td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/import-template.md" target="_blank">Importação de modelo</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de email – Conteúdo condicional</strong>: recurso de paridade para o novo designer de email, possibilitando a personalização de emails para além de tokens.</td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/conditional-content.md" target="_blank">Conteúdo condicional</a></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de email – Teste A/B</strong>: recurso de paridade para o novo designer de email que permite realizar testes A/B para ver quais tipos de conteúdo obtêm a melhor resposta.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de email – Temas de marca</strong>: agora é possível definir temas de marca no Marketo Engage. As configurações de estilo podem ser reutilizadas e aplicadas em modelos de email e outros ativos de email para manter a consistência da marca.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <td><strong>Designer de email – Conversor de imagem para HTML</strong>: faça upload de um arquivo de imagem PNG/JPEG compatível de um email e ele será convertido automaticamente em HTML para uso no novo designer de email.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer de email – Ação clonar email</strong>: agora é possível clonar um email em outra pasta do programa nas Atividades de marketing e reutilizar rapidamente os emails já existentes.</td>
   <td>Enviado</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Atualização da integração do Salesforce CRM**: uma nova versão da integração nativa do CRM será implantada em sandboxes ativas com o conector nativo habilitado ao longo de sete dias, a partir de 13 de novembro de 2025. Obtenha todos os detalhes [esta publicação da Nation](https://nation.marketo.com/t5/product-blogs/salesforce-crm-integration-upgrade/ba-p/358702){target="_blank"}

* **Descontinuação da barra dupla na API REST**: em 16 de setembro de 2025, a Adobe fez a transição para uma infraestrutura de hospedagem mais moderna para URLs da API REST que usam tecnologia mais recente, adicionando segurança e escalabilidade. Se sua assinatura tem usado APIs com uma barra dupla (//) no URL, leia [esta publicação da Nation](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} para saber as próximas etapas.

* **Retorno ao Velocity Scripting no novo Designer de email**: o Adobe Marketo Engage lançou um recurso chamado _Conteúdo condicional_ para o novo Designer de email em junho. O recurso era alimentado por scripts Handlebar, em vez de scripts Velocity, em um esforço para fornecer um pouco mais de flexibilidade no conteúdo dinâmico. Mas, quando descobrimos que isso estava causando a resolução incorreta de alguns tokens, decidimos desabilitá-lo temporariamente. [Saiba mais](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Fim da vida útil da Identidade do Marketo Engage**: em agosto de 2025, a Adobe começou o processo de remoção do suporte à Identidade do Marketo Engage (logon via `login.marketo.com`). Para evitar a interrupção do acesso ao Marketo Engage, você deve fazer a transição para a [Identidade da Adobe](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} até no máximo 30 de setembro de 2025.

   * _Descontinuação de restrições de IP_: o suporte para a [restrição de logons do Marketo com base no IP](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. Um novo recurso de controle de acesso baseado em localização para a Identidade da Adobe no Adobe Admin Console será lançado em breve.

   * _Descontinuação do logon único (SSO)_: o suporte para o [SSO da Identidade do Marketo](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. O logon único (SSO) para a Identidade da Adobe no Adobe Admin Console deve ser configurado separadamente. Para ver as etapas de configuração, consulte [Configurar identidade e logon único](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.

* **Descontinuação do recurso _Encaminhar para um amigo_**: em 29 de setembro de 2025, o recurso _Encaminhar para um amigo_ nos emails do Marketo Engage 2.0 (o editor de email legado) foi completamente descontinuado para todas as assinaturas. Isso afetou o token “Encaminhar para um amigo” e os links “Encaminhar para um amigo” em emails que já foram enviados ou foram agendados para envio com o token. [Saiba mais](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Descontinuação do parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo será descontinuado e não estará disponível após 31 de janeiro de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API SOAP**: o suporte para a API SOAP do Marketo terminará em 31 de janeiro de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
