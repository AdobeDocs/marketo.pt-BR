---
description: Notas de versão atuais - Documentos do Marketo - Documentação do produto
title: Notas da versão atual
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 62%

---

# Notas de versão: janeiro de 2026 {#release-notes-jan-26}

Abaixo você encontrará todos os recursos incluídos na versão de janeiro de 2026. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

Para ver as notas de versão específicas do Adobe Dynamic Chat, consulte [esta página](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados com uma estrela (![estrela](assets/yellow-star.png)) são complementos pagos. Entre em contato com o(a) representante do Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os seguintes recursos se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **sábado, 30 de janeiro de 2026**, com uma implementação gradual dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Recurso</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr>
   <td><strong>TÍTULO DO RECURSO</strong>: descrição do recurso.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TÍTULO DO RECURSO</strong>: descrição do recurso.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TÍTULO DO RECURSO</strong>: descrição do recurso.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Recursos do Adobe Connect {#adobe-connect-features}

O recurso [Webinars interativos](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/interactive-webinars-overview){target="_blank"} do Marketo Engage é viabilizado pelo Adobe Connect, que enriquece o gerenciamento de pessoas e campanhas com dados de eventos e melhora a qualidade das pessoas. Abaixo estão algumas versões recentes do Adobe Connect que afetam diretamente os usuários dos Webinars interativos.

* **Pod de pesquisa**: o Adobe Connect 12.11 apresenta um novo Pod de pesquisa que permite que os hosts projetem e entreguem formulários de feedback estruturados diretamente em uma sessão em tempo real.

* **Pod de recursos**: o novo Pod de recursos substitui os pods de arquivos e links da Web anteriores, fornecendo uma maneira única e unificada de compartilhar recursos durante as sessões ativas.

* **Experiência aprimorada de interface de sala**: o Adobe Connect 12.11 apresenta uma interface de sala atualizada e mais moderna, baseada na estrutura de design mais recente do Spectrum 2 da Adobe, alinhada com a linguagem visual usada em outros produtos da Adobe, como o Creative Cloud e o Experience Cloud.

Para obter detalhes completos, consulte as [Notas de versão do Adobe Connect 12.11](https://helpx.adobe.com/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"}.

## Anúncios {#announcements}

* **Descontinuação do parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo será descontinuado e não estará disponível após quarta-feira, 31 de março de 2026. Todas as integrações novas e já existentes devem autenticar chamadas da API REST usando o cabeçalho “Authorization”, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API SOAP**: o suporte para a API SOAP do Marketo terminará em quarta-feira, 31 de março de 2026. Os serviços que usam os recursos da API SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Fim da Vida Útil da Identidade do Marketo Engage**:

   * _Descontinuação de restrições de IP_: o suporte para a [restrição de logons do Marketo com base no IP](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. Um novo recurso de controle de acesso baseado em localização para a Identidade da Adobe no Adobe Admin Console será lançado em breve.

   * _Descontinuação do logon único (SSO)_: o suporte para o [SSO da Identidade do Marketo](https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} terminou em 30 de julho de 2025. O recurso permanecerá operacional até que a transição para a Identidade da Adobe seja concluída. O logon único (SSO) para a Identidade da Adobe no Adobe Admin Console deve ser configurado separadamente. Para ver as etapas de configuração, consulte [Configurar identidade e logon único](https://helpx.adobe.com/br/enterprise/using/set-up-identity.html){target="_blank"}.
