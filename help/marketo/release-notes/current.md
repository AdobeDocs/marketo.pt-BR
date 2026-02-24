---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 466f4b43124a2cb0894c4b8ce605521be1c4b4cd
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 58%

---

# Notas de versão: fevereiro de 2026 {#release-notes-jan-26}

Abaixo você encontrará todos os recursos incluídos na versão de fevereiro de 2026. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 20 de fevereiro de 2026**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>Email Designer - Ações de Pasta</strong>: paridade com o editor de email antigo.
   <ul>
   <li>Compartilhar e arquivar ações de pastas para ativos do Designer de email.</li>
   <li>Compartilhe pastas entre espaços de trabalho, clique com o botão direito do mouse em uma pasta para criar um novo ativo e mover ativos por meio de arrastar e soltar.</li>
   </ul>
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
   <td><strong>Email Designer - API</strong>: agora você pode usar chamadas de API para o Email Designer.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Gerenciar marcas (beta)</strong>: gere conteúdo de email com base nas diretrizes de redação de cópia específicas de sua organização/marca.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
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
   <td><strong>Email Designer - Geração de imagem do assistente de IA</strong>: agora, além do Firefly, você pode usar modelos do Nano Banana para gerar imagens com o Assistente de IA para conteúdo de email.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Descontinuação do parâmetro “access_token” da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo será descontinuado e não estará disponível após 31 de março de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API SOAP**: o suporte para a API SOAP do Marketo terminará em 31 de março de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
