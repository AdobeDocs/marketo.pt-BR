---
description: Documente a configuração da sua nova instância do Marketo Engage.
title: Novas práticas recomendadas de instância - documente sua configuração
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 2%

---

# Novas práticas recomendadas de instância: documentar sua configuração {#new-instance-best-practices-document-your-setup}

Agora que você aprendeu as principais áreas de produto para configurar para uma nova instância do Marketo Engage, a próxima etapa é criar a documentação para a configuração da sua instância e pilha técnica. Ao criá-la por meio de uma planilha ou um aplicativo de gerenciamento de projeto, sua documentação será um excelente recurso para rastrear o progresso e registrar os detalhes, bem como manter sua instância estruturada e sustentável para futuros profissionais de marketing em sua organização.

## Dados {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Importação de lista</td>
    <td><li>Obtenha uma lista das fontes de dados cujos registros serão extraídos para <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people" target="_blank">importar para o Marketo Engage</a>.</li>
    <li>Se você estiver importando de várias fontes de dados, considere usar Listas Mestras ou <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">criar um campo personalizado</a> no registro de pessoa para indicar a fonte de dados.</li></td>
  </tr>
  <tr>
    <td>Integração de banco de dados</td>
    <td><li>Ao aproveitar a sincronização nativa entre o Marketo Engage e o CRM, considere cuidadosamente quais campos você deseja sincronizar entre sistemas. Nem todos os campos precisam ser sincronizados, portanto, seja estratégico em relação aos fluxos de dados.</li></td>
  </tr>
</tbody>
</table>

## Documentação {#documentation}

<table>
<thead>
  <tr>
    <th style="width:20%">Área</th>
    <th style="width:80%">Itens de ação</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Usuários</td>
    <td><li>Documente os <a href="https://experienceleague.adobe.com/pt-br/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">usuários atuais</a> em sua instância por motivos de segurança. Os seguintes detalhes devem ser incluídos no mínimo (e estão visíveis ao acessar Admin &gt; Usuários e funções):</li>
    <ul>
    <li>Nome</li>
    <li>Email</li>
    <li>Login</li>
    <li>Função</li>
    <li>Data de expiração do acesso</li>
    <li>Data de criação do usuário</li>
    <li>Data de logon mais recente</li></ul>
    <p><img src="assets/note-icon.png" alt="ícone de nota"> OBSERVAÇÃO: você também pode expandir essa documentação para incluir funções/permissões.
    <p>
    <li>Como administrador de produto do Marketo Engage, desenvolva um processo interno para auditar e atualizar a lista de usuários do Marketo Engage regularmente. Para fazer alterações na lista de usuários no Adobe Admin Console, considere <a href="https://helpx.adobe.com/br/enterprise/using/users.html" target="_blank">realizar ações em massa</a>, como carregar um .CSV, usar a API REST de gerenciamento de usuários etc.</li></td>
  </tr>
  <tr>
    <td>Organização</td>
    <td><li>Documente a estrutura de pastas acordada, as convenções de nomenclatura padrão para programas, ativos, etc. e o porquê por trás das decisões tomadas. <a href="https://experienceleague.adobe.com/pt-br/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">Saiba mais sobre as práticas recomendadas aqui.</a></li></td>
  </tr>
  <tr>
    <td>Changelog</td>
    <td><li>Crie um changelog no qual você pode documentar o que está mudando na sua instância e o porquê das modificações. <a href="https://experienceleague.adobe.com/pt-br/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">Saiba mais sobre as práticas recomendadas aqui.</a></li></td>
  </tr>
  <tr>
    <td>Playbooks</td>
    <td><li>Crie um Manual do usuário ou um Manual do administrador para usuários internos que estão integrando a instância.</li></td>
  </tr>
  <tr>
    <td>Conversas com equipes internas</td>
    <td><li>Alinhe as expectativas da equipe interna de marketing em relação ao Marketo Engage com os recursos de Marketo Engage.</li>
    <li>Identifique as equipes que serão suas partes interessadas na instância do Marketo Engage e documente suas metas para alcançar usando o Marketo Engage como uma tecnologia.</li></td>
  </tr>
  <tr>
    <td>Espaços de trabalho e partições (se aplicável)</td>
    <td><li>Documente como os espaços de trabalho são definidos e como eles se relacionam com as partições de banco de dados (por exemplo, um espaço de trabalho Global que mostra todos vs. setores de negócios).</li>
    <li>Importar novos registros para a partição apropriada.</li>
    <li>Defina o valor no CRM que coloca os usuários na partição apropriada.</li></td>
  </tr>
</tbody>
</table>
