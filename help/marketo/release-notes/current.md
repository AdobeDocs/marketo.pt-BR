---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: 'https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
  - id: af97ce94-35fa-4fa9-b85a-46b752ac4028
    internal-label: Release information
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: c36bbfe0f8ce46dfa6b5c708fa29c5a710cc2358
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 15%
---
# Notas de versão: novembro de 2026 {#release-notes-nov-26}

Abaixo você encontrará todos os recursos incluídos na versão de novembro de 2026. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **6 de novembro de 2026**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>habilidade Planejar campanhas</strong>: o CX Enterprise Coworker para Marketo Engage agora pode transformar um resumo da campanha em um documento completo de configuração de programa do Marketo Engage. O documento inclui a estrutura de pastas, campanhas inteligentes, configurações de email, tokens e uma lista de verificação de controle de qualidade. Isso ajuda as equipes a lançarem campanhas com mais rapidez e padronizarem a configuração do programa. A habilidade pode ser configurada por meio de marcação.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Agentes chamáveis</strong>: crie agentes de IA que são executados como uma etapa de fluxo em suas campanhas inteligentes e atuam em um registro de cliente potencial com base em instruções escritas em linguagem simples. Por exemplo, um agente pode normalizar os dados ou sinalizar possíveis bots de um lead e, em seguida, gravar o resultado nos campos do lead. Isso leva o processamento de clientes potenciais com base em julgamento a suas campanhas sem código personalizado.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Clonar para este programa/pasta</strong>: as operações de clonagem na Marketo Engage agora oferecem consistentemente uma opção "Esta pasta" ou "Este programa" como primeira escolha ao escolher o destino do ativo clonado. Escolher essa opção clona o ativo para o programa ou pasta pai do ativo atual.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <tr>
   <td><strong>Alerta instantâneo na sincronização do CRM</strong>: habilitar ou desabilitar a sincronização nativa do CRM para um ambiente agora aciona uma notificação para os usuários que assinaram o canal de notificação do CRM.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Descontinuação da Captura de Imagens da Web**: para estar em conformidade com as práticas recomendadas modernas de segurança e privacidade, o recurso [Capturar Imagens da Web](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"} será descontinuado a partir da versão de novembro.

* **Restrições de Nome de API para Atributos de Atividade Personalizados**: Os Nomes de API para Atributos de Atividade Personalizados criados por meio da API ou da interface agora podem conter apenas caracteres alfanuméricos e sublinhados, e devem começar com um caractere alfanumérico.

* **Limites de Tamanho de Lista Estática para Obter Atividades de Cliente Potencial e Obter Alterações de Cliente Potencial**: a partir de 30 de setembro de 2026, as chamadas para Obter Atividades de Cliente Potencial ou Obter Pontos de Extremidade de Alterações de Cliente Potencial que incluem o parâmetro `listId` começaram a falhar com um Código de Erro 1003 (indicando que a lista estática de destino tem muitos registros) se as listas de destino contiverem 10.000 ou mais clientes potenciais. Consulte o [Guia de Migração](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obter mais informações.
