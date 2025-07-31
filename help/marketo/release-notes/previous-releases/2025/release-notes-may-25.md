---
description: Notas de versão - maio de 2025 - Documentação do Marketo - Documentação do produto
title: Notas de versão – Maio de 2025
feature: Release Information
exl-id: 99cd1d54-0a80-40fa-9d0c-1cb437be90f0
source-git-commit: 4a575c96100921c69c09996c649db979ac22cd4d
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 3%

---

# Notas de versão: maio de 2025 {#release-notes-may-25}

Abaixo você encontrará todos os recursos incluídos na versão de maio de 2025. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

As Notas de Versão específicas do Adobe Dynamic Chat [podem ser encontradas aqui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante da Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **23 de maio de 2025**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto"> 
 <tbody>
 <tr> 
   <th style="width:65%">Recurso</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr> 
   <td><strong>Controle de acesso com base em função para Email Designer Assets</strong>: um novo aprimoramento do sistema de controle de acesso com base em função (RBAC) fornece permissões mais granulares e gerenciamento de usuário aprimorado para ativos alimentados pelo novo Email Designer.</td> 
   <td>Remetido</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">Permissões granulares para o novo Designer de email (publicação do blog)</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Clonagem de emails criados no Designer de email</strong>: agora você pode clonar um email existente criado com o novo Designer de email.</td> 
   <td>Remetido</td>
   <td>n/d</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Tokens de acionador para qualquer atributo</strong>: lista expandida de tokens de acionador para oferecer suporte ao uso de dados de qualquer atributo de atividade em campos do Smart Campaign.</td> 
   <td>Remetido</td>
   <td>n/d</td>
  </tr>
 </tbody> 
</table>
<br/>

## Anúncios {#announcements}

* **Atualização da Integração de Conversão Offline do Facebook**: em 29 de maio de 2025, a [integração de Conversão Offline do Facebook](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"} para o Marketo Engage será migrada para a nova [API de Conversões Meta](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"}, devido à descontinuação da [API de Conversões Offline](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"} do Meta, de acordo com o controle de versão da API de Gráfico. Para obter mais informações, consulte o Guia de meta para [enviar eventos offline via API de conversões](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} (CAPI para offline).

* **Novo Recurso do Analytics - Beta Público**: [O Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anteriormente conhecido como Revenue Explorer e Advanced Report Builder) começou a ser implantado para todos os usuários atuais do Revenue Cycle Explorer em meados de abril. Essa nova ferramenta oferece uma interface flexível de relatórios e visualização para dados do Marketo Engage, fornecendo detalhes detalhados sobre progressão, desempenho e muito mais. Ele oferece interatividade e visualização mais avançadas, desempenho mais rápido e uma experiência do usuário mais contínua e intuitiva.

Para acessar esse recurso, é necessário ter adquirido o complemento Advanced BI Analytics. Entre em contato com a equipe de conta da Adobe (seu gerente de conta) para obter mais detalhes.

* **Descontinuação do Parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo está sendo descontinuado e não estará disponível após 31 de outubro de 2025. Todas as integrações novas e existentes devem autenticar chamadas de API REST usando o cabeçalho &quot;Autorização&quot;, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API do SOAP**: o suporte para a API do Marketo SOAP terminará em 31 de outubro de 2025. Os serviços que usam os recursos da API do SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
