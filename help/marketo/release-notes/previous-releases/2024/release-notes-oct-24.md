---
description: Notas de versão - outubro de 2024 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Outubro de 2024
feature: Release Information
exl-id: 2e28ae7f-51de-4510-b3e8-79a989f0daf5
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 21%

---

# Notas de versão: outubro de 2024 {#release-notes-oct-24}

Abaixo você encontrará todos os recursos incluídos na versão de outubro de 2024. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 4 de outubro de 2024**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
    <tr>
   <td><strong>Tokenization para Webinars interativos</strong>: agora você pode usar tokens para promover Webinars interativos em emails e Landing Pages sem precisar adicionar manualmente os detalhes do webinário.</td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/promoting-an-interactive-webinar.md#interactive-webinars-tokens" target="_blank">Promover um webinário interativo</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>Contagem da Smart List "Definida para Afetar"</strong>: veja quantas pessoas serão afetadas ao editar as regras de qualificação de uma Campanha Inteligente.</td>
   <td>Enviado</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>Botão Minha conta no painel de navegação</strong>: para quem migrou para o Adobe Identity Management System, um novo botão "Minha conta" no painel de navegação esquerdo permite configurar seu fuso horário e acessar os detalhes da assinatura.</td>
   <td>Enviado</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Melhorias no Relatório de desempenho de email</strong>: várias melhorias foram feitas nas métricas de relatório de email e no rastreamento de atividades, oferecendo insights adicionais e melhorando a precisão.
   <ul>
   <li>Filtrar pessoas excluídas e mescladas das métricas de desempenho de email</li>
   <li>Emails agora classificados como <i>abortados</i> após aguardar três dias para atividade de resposta</li>
   <li>As aberturas de email são contadas como abertas separadamente, para cada Campanha Inteligente</li>
   </td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">Relatório de desempenho de email</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Métricas de lista de pendências de sincronização do Salesforce</strong>: monitore a taxa de transferência de sincronização e as tendências de lista de pendências para planejar e agendar atualizações do CRM para obter uma experiência de sincronização ideal.
   </td>
   <td>Enviado</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Métricas de lista de pendências de sincronização do Salesforce</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Atualização da API de extração em massa**: corrigimos um problema na API de extração em massa envolvendo a opção columnHeaderNames, que permite especificar nomes de cabeçalho de coluna personalizados no arquivo exportado. Anteriormente, os nomes de cabeçalho de coluna contendo caracteres não ASCII podiam ficar corrompidos.

* **Descontinuação do parâmetro access_token da API Rest**: o parâmetro de consulta &quot;access_token&quot; usado para autenticar chamadas de API REST do Marketo está sendo descontinuado e não estará disponível após 31 de março de 2026. Todas as integrações novas e existentes devem autenticar chamadas de API REST usando o cabeçalho &quot;Autorização&quot; [conforme descrito aqui](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication#using-an-access-token).

* **Descontinuação do código QR**: em 4 de outubro de 2024, o recurso de código QR usado em notificações por push e ativos de mensagens no aplicativo será descontinuado. Isso inclui o uso de códigos QR para um novo dispositivo de teste, bem como a criação de novos ativos com códigos QR. Descontinuar os recursos com uso mais baixo permite realocar seus recursos para a manutenção geral do Marketo Engage.

* **Alterações no Munchkin**

   * **Nova Versão**: em 17 de setembro de 2024, o [Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 começará a ser implantado em instâncias do Marketo Engage que têm a configuração &quot;Munchkin Beta&quot; habilitada em **Admin** > **Treasure Chest**. Ele está programado para começar a implantação em todas as outras instâncias em 29 de outubro. Esta versão atualiza a criação do cookie do Munchkin. Não há alterações na funcionalidade.

   * **Caracteres da URL Removidos**: as atividades &quot;Visitas da página da Web&quot; e &quot;Link de cliques&quot; criadas pelo Munchkin JS agora removerão caracteres de controle não codificados por URL de todos os campos de URL. Essa alteração foi projetada para evitar erros relacionados à propagação desses tipos de caracteres em sistemas que não oferecem suporte a eles e não têm um uso válido no Marketo Engage.
