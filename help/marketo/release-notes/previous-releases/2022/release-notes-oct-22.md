---
description: Notas de versão - outubro de 2022 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Outubro de 2022
exl-id: 1494b8b9-049c-4969-ab95-a4be41d886b0
feature: Release Information
TQID: https://experienceleague.adobe.com/8d05i8J-yT1oEfPeF8Wn3Ir2Yy9SG6bswhaTA-oRwIw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2: id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 619
ht-degree: 21%

---

# Notas de versão: outubro de 2022 {#release-notes-oct-22}

Abaixo você encontrará todos os recursos incluídos na versão de outubro de 2022. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 14 de outubro de 2022**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique abaixo cada recurso para obter seu status.

### Ambiente de dados de marketing {#marketing-data-environment}

</br>

* **Sincronização de Campo Personalizado de Membro do Programa**: capacidade de sincronizar bidirecionalmente campos extensíveis capturados para um membro do programa (por exemplo, preferências de participante durante o registro do evento, como alimentação, sessões, controles etc.) com campos de membro do Campaign no Salesforce.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Sincronizar campos personalizados de membros de programas</a></td>
  </tr>
  </tbody>
</table>

* **Integração do Adobe Privacy Service**: harmonize com o Privacy Service para automatizar a conformidade com as regulamentações de privacidade de dados em todos os produtos da Experience Cloud. Atualmente, esse serviço está disponível somente para clientes do Marketo Engage que integraram o Adobe Identity Management System.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### Experiência da próxima geração {#modern-ux}

</br>

* **Screens atualizado na Experiência da Próxima Geração**: estamos fornecendo telas adicionais e atualizadas na experiência da próxima geração, que oferecem um design atualizado e aprimoramentos de usabilidade acessíveis via switch de alternância:

   * Detalhes do modelo de página de destino
   * Lista de modelos de email

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">Botão de alternância</a></td>
  </tr>
  </tbody>
</table>

* **Aprimorado Usado pela guia em Detalhes do modelo de email**: na nova experiência do, você verá informações adicionais relacionadas aos ativos que usam o modelo de email, incluindo Status do ativo, Última modificação e Última modificação por. Também é possível pesquisar, classificar e filtrar a lista de usados por ativos.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

* **Modais de filtro de ativo de relatório**: novo design para modelos de configuração de relatório exibindo uma nova árvore de ativos no menu de configuração e um filtro para Data de criação e modificação.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

### Aprimoramentos na API {#api-enhancements}

</br>

* **Importação de Cliente Potencial em Massa: associação de Vendedor**: paridade com a API REST de Cliente Potencial para poder associar clientes potenciais a Vendedores durante o processo de importação de cliente potencial em massa, reduzindo a complexidade e o número de chamadas de API necessárias.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">Importação de leads em massa</a></td>
  </tr>
  </tbody>
</table>

### Sales Insight {#sales-insight}

</br>

![(estrela)](assets/yellow-star.png)

* **Integração do Sales Insight com o Dynamic Chat**: o Painel de Insights agora inclui atividades do Dynamic Chat na Grade Inteligente junto com um resumo semanal e cartões de detalhes.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Integração ao Dynamic Chat</a></td>
  </tr>
  </tbody>
</table>

## Recursos da versão Agile

Os seguintes recursos seguem um formato Agile e são lançados em várias datas antes ou depois da data de lançamento padrão. Verifique abaixo cada recurso para obter seu status.

* **Fluxos de Caixa de Diálogo de Organização Automática para Dynamic Chat**: Melhore sua tela de Caixa de Diálogo lotada organizando tudo na tela em um formato limpo e fácil de ler com o pressionamento de um botão por meio da Organização Automática.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">Ícones de Designer de fluxo</a></td>
  </tr>
  </tbody>
</table>

* **Links de Reunião para Dynamic Chat**: opção para incluir automaticamente um link de Equipes ou Reunião para Google e Outlook em cada convite de calendário enviado aos visitantes.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">Calendário</a></td>
  </tr>
  </tbody>
</table>

* **Suporte a tipos de dados adicionais para o Dynamic Chat**: três novos tipos de dados (booleano, inteiro, flutuante) permitem que você aproveite mais campos existentes do Marketo Engage no Dynamic Chat para coisas como direcionamento com base em pontuações ou fazer perguntas aos visitantes sim/não.

<table>
  <tr>
   <td><b>Status</b></td>
   <td><b>Atualizações de documentação</b></td>
  </tr>
  <tr>
   <td>Lançado</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

## Anúncios {#announcements}

* **Forms 1.0**: a descontinuação do Forms 1.0 será concluída com a versão de outubro. Os ativos do Forms 1.0 não poderão mais enviar dados para o Marketo Engage e retornarão erros se forem tentados.

* **No-Script Forms**: o Forms não funcionará mais quando o Javascript estiver desabilitado no navegador. O envio do formulário exigirá que o Javascript esteja habilitado.
