---
description: Guia de solução de problemas do Adobe IMS - Documentação do Marketo - Documentação do produto
title: Guia de solução de problemas do Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
source-git-commit: eccebb8352c56770dea5af9395c8bc83a08525dd
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Guia de solução de problemas do Adobe IMS {#adobe-ims-troubleshooting-guide}

Durante o processo de migração de usuário do IMS, um usuário do Adobe é criado para cada usuário do Marketo Engage que está sendo migrado. Às vezes, ele não é criado (por vários motivos, relacionados ao registro do usuário no Ative Diretory ou a problemas com o endereço de email). Quando isso acontecer, o administrador do Marketo Engage verá os motivos no campo status de migração do usuário no console de automigração. Consulte como resolver vários problemas de criação de usuários do Adobe abaixo.

## Mensagens de erro {#error-messages}

* <a href="#not-in-directory">Não está no Diretório</a>
* <a href="#gmail-invalid-character">Caractere inválido do Gmail</a>
* <a href="#inactive-user">Usuário Inativo</a>
* <a href="#not-in-domain">Não está no Domínio</a>
* <a href="#create-failure">Criar Falha</a>
* <a href="#type2e-user-failure">Falha de Usuário Type2e</a>



<table>
<thead>
  <tr>
    <th style="width:20%">Mensagem de erro</th>
    <th style="width:40%">Causa raiz</th>
    <th style="width:40%">Resoluções</th>
  </tr>
  </thead>
<tbody>
  <tr>
    <td><i><a id="not-in-directory">Não está no diretório</a></i></td>
    <td>O usuário não existe no Ative Diretory (AD). Para qualquer organização com SSO que tenha a sincronização do AD ativada, a criação de usuários é permitida somente pelo Provedor de identidade (IdP). Portanto, o usuário não pôde ser adicionado por meio do Admin Console durante a migração do usuário.</td>
    <td>Migrar - o usuário precisa ser adicionado ao Ative Diretory com as permissões adequadas. Admin do Marketo para executar novamente a migração de usuário para este usuário no Console de migração. 
    <br>Não migrar - O administrador do Marketo deve ignorar o usuário no Console de Migração. O botão "Migração concluída" aparece quando todos os usuários são considerados ao migrar ou ignorar. Clique nele para concluir o processo de migração do usuário.</td>
  </tr>
  <tr>
    <td><i><a id="gmail-invalid-character">Caractere inválido do Gmail</a></i></td>
    <td>De acordo com a política de segurança da Adobe, '.' Os sinais e "+" não são permitidos somente em um endereço de email do domínio Gmail  
    <br>Ambos os caracteres especiais são permitidos em um endereço de email de domínio não Gmail. </td>
    <td>Migrar - O endereço de email precisa ser atualizado no Marketo Engage para estar em conformidade com a política de segurança da Adobe. Admin do Marketo para executar novamente a migração de usuário para este usuário no Console de migração.<br>Não migrar - O administrador do Marketo deve ignorar o usuário no Console de Migração. O botão "Migração concluída" aparece quando todos os usuários são considerados ao migrar ou ignorar. Clique nele para concluir o processo de migração do usuário.</td>
  </tr>
  <tr>
    <td><i><a id="inactive-user">Usuário inativo</a></i></td>
    <td>A Sincronização do AD está habilitada, e a conta federada do usuário existe, mas com o status inativo/desabilitado.</td>
    <td>Migrar - O status do usuário e as permissões apropriadas precisam ser restaurados. Admin do Marketo para executar novamente a migração de usuário para este usuário no Console de migração.
    <br>Não migrar - O administrador do Marketo deve ignorar o usuário no Console de Migração. O botão "Migração concluída" aparece quando todos os usuários são considerados ao migrar ou ignorar. Clique nele para concluir o processo de migração do usuário.</td>
  </tr>
  <tr>
    <td><i><a id="not-in-domain">Não está no Domínio</a></i></td>
    <td>A imposição de domínio está ativada no Admin Console, mas o domínio do endereço de email do usuário não é um dos domínios permitidos. 
    <br>As políticas de imposição de domínio são definidas no nível de diretório.</td>
    <td>Migrar - O endereço de email precisa ser atualizado no Marketo Engage para estar em conformidade com a política de imposição de domínio, ou o administrador do sistema pode <a href="https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories"> 
    mova o domínio para outro diretório desabilitado de Imposição de Domínio (DE) </a>ou <a href="https://helpx.adobe.com/br/enterprise/using/set-up-identity.html">crie um novo diretório</a>, que não esteja na política DE. Admin do Marketo para executar novamente a migração de usuário para este usuário no Console de migração. <br>Não migrar - O administrador do Marketo deve ignorar o usuário no Console de Migração. O botão "Migração concluída" aparece quando todos os usuários são considerados ao migrar ou ignorar. Clique nele para concluir o processo de migração do usuário.</td>
  </tr>
  <tr>
    <td><i><a id="create-failure">Criar falha</a></i></td>
    <td>Vários motivos no back-end.</td>
    <td>Envie um caso de suporte.</td>
  </tr>
  <tr>
    <td><i><a id="type2e-user-failure">Falha do usuário do Type2e</a></i></td>
    <td>Vários motivos no back-end.</td>
    <td>Envie um caso de suporte.</td>
  </tr>
</tbody>
</table>
