---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: d0cf66fe0c72af8e9d1db09792f73fd6db10abbb
workflow-type: tm+mt
source-wordcount: 477
ht-degree: 22%

---

# Notas de versão: julho de 2026 {#release-notes-july-26}

Abaixo você encontrará todos os recursos incluídos na versão de 26 de julho. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **10 de julho de 2026**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Habilidade do Marketo AI - Conhecimento do produto</strong>: o conhecimento do produto oferece acesso sob demanda ao conhecimento da Marketo sem sair da plataforma. Faça uma pergunta em linguagem simples e a IA do Marketo se baseia na documentação oficial do Adobe para respondê-la.</td>
   <td>Abrir beta</td>
   <td><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">Conhecimento do produto</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Habilidade do Marketo AI - Investigar clientes potenciais</strong>: descubra por que uma pessoa/cliente potencial específico não atingiu um marco (como MQL, qualificação de programa ou uma campanha) e obtenha uma explicação em linguagem simples do que aconteceu.
</td>
   <td>Abrir beta</td>
   <td><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">Investigar clientes em potencial</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Menu Contextual do Email Designer - Assistente de IA</strong>: os recursos do Assistente de IA da Designer de email agora podem ser acessados pelo menu contextual (a barra preta). Por exemplo, quando você seleciona conteúdo de texto, o ícone do Assistente de IA é exibido no menu contextual, permitindo executar ações rápidas a partir desse ponto.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Descontinuação do parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo está sendo descontinuado e não estará disponível após 31 de julho de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Limite de Clientes Potenciais de Mesclagem da API REST**: a partir de 31 de julho de 2026, as chamadas que incluírem mais de 25 IDs no parâmetro leadIds de uma chamada da API de Clientes Potenciais de Mesclagem resultarão em um código de erro 1080 e a chamada será ignorada. As tarefas que exigem a fusão de mais de 25 registros em um devem ser divididas em várias tarefas para garantir o sucesso dessas chamadas.

* **Descontinuação da API do SOAP**: o suporte para a API do Marketo SOAP terminará em 31 de julho de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Limites de Tamanho de Lista Estática para Obter Atividades de Cliente Potencial e Obter Alterações de Cliente Potencial**: a partir de 30 de setembro de 2026, as chamadas para Obter Atividades de Cliente Potencial e Obter Pontos de Extremidade de Alterações de Cliente Potencial que incluem o parâmetro `listId` retornarão um código de erro 1003 se a lista estática de destino contiver 10.000 ou mais clientes potenciais. Consulte o [Guia de Migração](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} para obter mais informações.
