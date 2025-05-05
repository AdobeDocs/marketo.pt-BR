---
description: Notas de versão - Janeiro de 2025 - Documentação do Marketo - Documentação do produto
title: Notas de versão - Janeiro de 2025
feature: Release Information
source-git-commit: 709c5f3c0009763f8ab7778278c6a2fe6db10a08
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 5%

---

# Notas de versão: janeiro de 2025 {#release-notes-jan-25}

Abaixo você encontrará todos os recursos incluídos na versão de janeiro de 2025. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

As Notas de Versão específicas do Adobe Dynamic Chat [podem ser encontradas aqui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante da Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **17 de janeiro de 2025**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Recurso</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
    <tr> 
   <td><strong>Novo Designer de email</strong>: crie emails modernos e eficientes usando o novo Designer de email nativo no Marketo Engage. Acesse um dos modelos de email predefinidos e prontos para uso ou crie facilmente o seu próprio modelo. Use conteúdo dinâmico e acesse imagens dos serviços em nuvem da Adobe Experience Manager. Use a funcionalidade Gen-AI do Acelerador de conteúdo para criar e-mails inovadores e de alto desempenho em escala.
   <p><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: para acessar o novo designer de email, sua assinatura do Marketo Engage deve ser migrada para o <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview">Adobe Identity Management System (IMS)</a>. Se a sua ainda não tiver sido lançada e você quiser solicitá-la, contate a Equipe de Conta da Adobe (seu gerente de conta) ou o <a href="https://nation.marketo.com/t5/support/ct-p/Support">Suporte da Marketo</a>. Para obter acesso à funcionalidade Gen-AI do Acelerador de conteúdo, entre em contato com a equipe de conta da Adobe.</td>
   <td>Remetido</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">Visão geral do Designer de email</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Cancelar o registro de inscritos de um evento em webinários interativos</strong>: agora, se você não quiser um inscrito em seu webinário por qualquer motivo, poderá cancelar o registro deles. O fluxo de trabalho remove o inscrito do Programa de evento do Marketo e do Adobe Connect.</td> 
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Desabilitar Campanhas no Arquivo Morto</strong>: desabilite campanhas de gatilho ativas e cancele todas as execuções de campanhas em lote agendadas em uma pasta quando ela for arquivada. Como há uma verificação de permissões adicional para pastas de arquivamento que contêm campanhas ativas (Ativar Campanha de Acionador e Campanha em Lote de Agendamento), esse recurso fica desabilitado por padrão com esta versão e pode ser habilitado navegando até <b>Admin</b> &gt; <b>Treasure Chest</b> na sua assinatura do Marketo Engage.</td> 
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anúncios {#announcements}

* **Descontinuação de recursos sociais**: na quarta-feira, 31 de julho de 2024, o Marketo Engage começou a descontinuação dos seguintes recursos sociais no produto:

   * Pesquisas
   * Botão social
   * Oferta da recomendação
   * Compartilhamento de vídeo
   * Sorteios

A partir de então, os usuários não conseguiram criar, clonar ou incorporar esses recursos sociais no Marketo Engage. Os ativos sociais existentes continuarão a funcionar até 31 de janeiro de 2025. Em 1º de fevereiro de 2025, os ativos sociais deixarão de funcionar. Os recursos sociais incorporados às Páginas de aterrissagem precisarão ser removidos. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Obter Atualização da API de Membros do Programa**: Melhoramos a API [Obter Membros do Programa](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} para oferecer suporte à capacidade de recuperar o identificador dos membros do programa. Isso é feito adicionando a id à lista de campos especificados no parâmetro fields da solicitação de API.

* **Descontinuação do parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo está sendo descontinuado e não estará disponível após 30 de junho de 2025. Todas as integrações novas e existentes devem autenticar chamadas de API REST usando o cabeçalho &quot;Autorização&quot;, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API do SOAP**: o suporte para a API do Marketo SOAP terminará em 31 de outubro de 2025. Os serviços que usam os recursos da API do SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
