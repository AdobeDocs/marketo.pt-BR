---
description: Notas de versão atuais - Documentação do Marketo - Documentação do produto
title: Notas da versão atual
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 38ec4726dece1695a15104fdb7fa7592b298d4a9
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 7%

---

# Notas de versão: abril de 2025 {#release-notes-apr-25}

Abaixo você encontrará todos os recursos incluídos na versão de abril de 25. Verifique a edição do Adobe Marketo Engage quanto à disponibilidade de recursos.

As Notas de Versão específicas do Adobe Dynamic Chat [podem ser encontradas aqui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Os recursos indicados por uma estrela (![star](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante da Marketo Engage para obter mais informações.

## Recursos do ciclo de lançamento padrão {#standard-release-cycle-features}

Os recursos a seguir se enquadram no ciclo de lançamento padrão e começarão a ser lançados em **25 de abril de 2025**, com uma implantação em fases dos recursos restantes nas semanas seguintes. Os recursos e as datas de lançamento estão sujeitos a alterações. Verifique o status ao lado de cada recurso.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Recurso</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Documentação</th>
  </tr>
  <tr> 
   <td><strong>Compatibilidade de Modelos para Email Designer</strong>: os modelos de email do editor de email clássico agora são compatíveis com o novo <a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">Designer de Email</a>.</td>
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Autoatendimento SSL</strong>: a criptografia SSL permite tornar seguras as Páginas de Aterrissagem de uma instância do Marketo Engage. A habilitação desse recurso costumava exigir a assistência da equipe de suporte da Adobe. Os usuários do Marketo agora podem ativá-lo por conta própria, economizando tempo valioso.</td> 
   <td><i>Em breve</i></td>
   <td><i>Em breve</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Anúncios {#announcements}

* **Novo Recurso do Analytics - Beta Público**: [Análises Avançadas de BI](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (anteriormente conhecidas como Explorador de Receita e Report Builder Avançado) começam a ser implantadas para todos os usuários atuais do Explorador de Ciclo de Receita em meados de abril. Essa nova ferramenta oferece uma interface flexível de relatórios e visualização para dados do Marketo Engage, fornecendo detalhes detalhados sobre progressão, desempenho e muito mais. Ele oferece interatividade e visualização mais avançadas, desempenho mais rápido e uma experiência do usuário mais contínua e intuitiva.

Para acessar esse recurso, é necessário ter adquirido o complemento Advanced BI Analytics. Entre em contato com a equipe de conta da Adobe (seu gerente de conta) para obter mais detalhes.

* **Descontinuação do parâmetro &#39;access_token&#39; da API**: o parâmetro de consulta `access_token` usado para autenticar chamadas da API REST do Marketo está sendo descontinuado e não estará disponível após 30 de junho de 2025. Todas as integrações novas e existentes devem autenticar chamadas de API REST usando o cabeçalho &quot;Autorização&quot;, [conforme descrito aqui](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Descontinuação da API do SOAP**: o suporte para a API do Marketo SOAP terminará em 31 de outubro de 2025. Os serviços que usam os recursos da API do SOAP devem ser migrados para a [API REST](https://experienceleague.adobe.com/pt-br/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Descontinuação de recursos sociais**: na quarta-feira, 31 de julho de 2024, o Marketo Engage começou a descontinuação dos seguintes recursos sociais no produto:

   * Pesquisas
   * Botão social
   * Oferta da recomendação
   * Compartilhamento de vídeo
   * Sorteios

A partir de então, os usuários não conseguiram criar, clonar ou incorporar esses recursos sociais no Marketo Engage. Os ativos sociais existentes continuarão a funcionar até 31 de janeiro de 2025. Em 1º de fevereiro de 2025, os ativos sociais deixaram de funcionar. Quaisquer recursos sociais incorporados às Páginas de aterrissagem precisarão ser removidos. [Saiba mais](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}
