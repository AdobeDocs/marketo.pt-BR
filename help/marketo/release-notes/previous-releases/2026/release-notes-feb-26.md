---
description: Notas de versão - fevereiro de 2026 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Fevereiro de 2026
feature: Release Information
exl-id: 679d2fca-99ba-4321-ad0d-a297b7f193fc
source-git-commit: 937c4a43066f957ddbeab9363174bc04e9a7d718
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 41%

---

# Notas de versão: fevereiro de 2026 {#release-notes-feb-26}

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
   <td>Lançado</td>
   <td><a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/email-marketing/email-designer/ai-assistant#create-content-for-a-specific-section">Crie conteúdo para uma seção específica do seu email</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Anúncios {#announcements}

* **Descontinuação do recurso de SEO**: na terça-feira, 31 de março de 2026, o Marketo Engage descontinuará o recurso de Otimização do Mecanismo de Pesquisa (SEO). Se você não usa o SEO ativamente, não precisa fazer nada. Se você tiver usado o SEO recentemente, terá a opção de exportar seus dados. [Saiba mais](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617?profile.language=pt){target="_blank"}.

* **Limite de Clientes Potenciais de Mesclagem da API REST**: a partir de 31 de março de 2026, as chamadas que incluírem mais de 25 IDs no parâmetro leadIds de uma chamada da API de Clientes Potenciais de Mesclagem resultarão em um código de erro 1080 e a chamada será ignorada. As tarefas que exigem a fusão de mais de 25 registros em um devem ser divididas em várias tarefas para garantir o sucesso dessas chamadas.

* **Descontinuação do parâmetro “access_token” da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo será descontinuado e não estará disponível após sábado, 31 de julho de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API SOAP**: o suporte para a API SOAP do Marketo terminará em sábado, 31 de julho de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
