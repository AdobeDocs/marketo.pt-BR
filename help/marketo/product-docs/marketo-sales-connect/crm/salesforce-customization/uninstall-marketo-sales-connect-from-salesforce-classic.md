---
description: Desinstale o Marketo Sales Connect do Salesforce Classic - Marketo Docs - Documentação do produto
title: Desinstalar o Marketo Sales Connect do Salesforce Classic
exl-id: 17078054-a615-4f2f-bfde-f28fd3ff6f48
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '1186'
ht-degree: 8%

---

# Desinstalar o Marketo Sales Connect do Salesforce Classic {#uninstall-marketo-sales-connect-from-salesforce-classic}

Veja como desinstalar o pacote Marketo Sales Connect da sua conta Salesforce depois de começar a usar as ações do Sales Insight.

## Remover [!DNL Sales Connect] campos do layout da página {#remove-sales-connect-fields-from-page-layout}

1. No [!DNL Salesforce] Classic, clique em **[!UICONTROL Instalação]**.

   ![](assets/uninstall-salesforce-classic-customization-package-1.png)

1. Na navegação à esquerda, em [!UICONTROL Build], expanda (mas não clique em) [!UICONTROL Personalizar] e [!UICONTROL Leads]. Em seguida, selecione **[!UICONTROL Layouts de página]**.

   ![](assets/uninstall-salesforce-classic-customization-package-2.png)

1. Clique em **[!UICONTROL Editar]** ao lado de Layout do cliente potencial.

   ![](assets/uninstall-salesforce-classic-customization-package-3.png)

1. No console, selecione **[!UICONTROL Campos]**. Na Localização Rápida, pesquise &quot;MSC&quot;. Todos os campos acinzentados foram adicionados ao layout da página. Você terá que excluí-los.

   ![](assets/uninstall-salesforce-classic-customization-package-4.png)

   >[!NOTE]
   >
   >Se nenhum dos campos estiver esmaecido, significa que você não os adicionou ao layout da página. Você pode ignorar esta seção.

1. Role até a seção que tem seus Campos Personalizados do [!DNL Sales Connect].

   ![](assets/uninstall-salesforce-classic-customization-package-5.png)

1. Há 10 tipos de campos MSC que podem ser adicionados a esta seção. Remova todos os campos adicionados ou simplesmente exclua a seção inteira.

1. Clique em **[!UICONTROL Salvar rapidamente]** quando terminar.

   ![](assets/uninstall-salesforce-classic-customization-package-6.png)

## Remover botões [!DNL Sales Connect] dos layouts de página {#remove-sales-connect-buttons-from-page-layouts}

1. No console (Etapa 4 acima), selecione **[!UICONTROL Botões]**. Pesquise &quot;MSC.&quot; Todos os botões acinzentados foram adicionados à seção de botão personalizada. Você terá que excluí-los.

   ![](assets/uninstall-salesforce-classic-customization-package-7.png)

   >[!NOTE]
   >
   >Se nenhum dos botões estiver acinzentado, significa que você não os adicionou. Você pode ignorar esta seção.

1. Arraste e solte os botões MSC da seção [!UICONTROL Botões Personalizados] no console.

   ![](assets/uninstall-salesforce-classic-customization-package-8.png)

1. Clique em **[!UICONTROL Salvar rapidamente]** quando terminar.

   ![](assets/uninstall-salesforce-classic-customization-package-9.png)

## Remover [!DNL Sales Connect] Campos da Seção [!UICONTROL Histórico de Atividades] {#remove-sales-connect-fields-from-activity-history-section}

1. Role até a parte inferior da página até a seção da lista relacionada ao [!UICONTROL Histórico de Atividades] e clique no ícone de Chave inglesa.

   ![](assets/uninstall-salesforce-classic-customization-package-10.png)

1. Selecione os [!DNL Sales Connect] Campos da área [!UICONTROL Campos Selecionados] e clique na seta [!UICONTROL Remover]. Clique em **[!UICONTROL OK]** quando terminar.

   ![](assets/uninstall-salesforce-classic-customization-package-11.png)

   >[!NOTE]
   >
   >A abreviação MSE _is_ [!DNL Sales Connect]. É apenas o nome anterior, &quot;Marketo Sales Engage&quot;.

1. Clique em **Salvar** quando terminar de usar a página de clientes potenciais.

## Remover [!DNL Sales Connect] Botões de Ação em Massa da Exibição da Lista de Clientes Potenciais {#remove-sales-connect-bulk-action-buttons-from-lead-list-view}

1. Na navegação à esquerda, em [!UICONTROL Build], expanda (mas não clique em) [!UICONTROL Personalizar] e [!UICONTROL Leads]. Em seguida, selecione **[!UICONTROL Pesquisar Layouts]**.

   ![](assets/uninstall-salesforce-classic-customization-package-12.png)

1. Ao lado de Exibição da Lista de Clientes Potenciais, clique em **[!UICONTROL Editar]**.

   ![](assets/uninstall-salesforce-classic-customization-package-13.png)

1. Selecione **[!UICONTROL Adicionar ao MSC Campaign (Classic)]**, **[!UICONTROL Email com MSC (Classic)]** e **[!UICONTROL Enviar para o MSC (Classic)]** e clique na seta [!UICONTROL Remover]. Depois clique em **[!UICONTROL Salvar]**.

   ![](assets/uninstall-salesforce-classic-customization-package-14.png)

Você não deve mais ver os botões na exibição da lista de clientes potenciais.

## Remover Configuração MSC para Contatos {#remove-msc-configuration-for-contacts}

1. Em [!DNL Salesforce], clique em **[!UICONTROL Instalação]**.

1. Na navegação à esquerda, em [!UICONTROL Compilação], expanda (mas não clique em) [!UICONTROL Personalizar] e [!UICONTROL Contatos]. Em seguida, selecione **[!UICONTROL Layouts de página]**.

1. Ao lado do Layout do Contato, clique em **[!UICONTROL Editar]**.

1. Repita as etapas das três seções.

## Remover Configuração MSC para Oportunidade {#remove-msc-configuration-for-opportunity}

1. Em [!DNL Salesforce], clique em **[!UICONTROL Instalação]**.

1. Na navegação à esquerda, em [!UICONTROL Compilação], expanda (mas não clique em) [!UICONTROL Personalizar] e [!UICONTROL Oportunidades]. Em seguida, selecione **[!UICONTROL Layouts de página]**.

1. Ao lado de Layout da oportunidade, clique em **[!UICONTROL Editar]**.

1. Repita as etapas das três seções.

A visualização da oportunidade tem apenas um botão - &quot;Enviar email MSE&quot; e os seguintes campos:

![](assets/uninstall-salesforce-classic-customization-package-15.png)

## Remover Configuração do MSC para a Conta {#remove-msc-configuration-for-account}

1. Em [!DNL Salesforce], clique em **[!UICONTROL Instalação]**.

1. Na navegação à esquerda, em [!UICONTROL Compilação], expanda (mas não clique em) [!UICONTROL Personalizar] e, em seguida, [!UICONTROL Conta]. Em seguida, selecione **[!UICONTROL Layouts de página]**.

1. Ao lado de Layout da conta, clique em **[!UICONTROL Editar]**.

1. Repita as etapas das três seções.

A exibição Conta tem apenas um botão - &quot;Enviar email do MSE&quot; e os seguintes campos:

![](assets/uninstall-salesforce-classic-customization-package-16.png)

## Remover Caixa de Saída de Vendas do Marketo {#remove-marketo-sales-outbox}

1. No [!DNL Salesforce], clique na guia **+** na parte superior da tela.

1. Clique em **[!UICONTROL Personalizar minhas guias]**.

1. Selecione a opção Caixa de Saída de Vendas do Marketo à direita. Clique na seta [!UICONTROL Remover] e em **[!UICONTROL Salvar]**.

## Excluir Pacote [!DNL Sales Connect] {#delete-sales-connect-package}

Depois de remover todos os objetos da sua conta da Salesforce, siga as etapas abaixo.

1. Em [!DNL Salesforce], clique em **[!UICONTROL Instalação]**.

1. Na caixa Localização Rápida, informe &quot;Classes de Apex&quot;.

1. Clique em **Excluir** ao lado de todas as entradas &quot;MarketoSalesConnectionCustomization&quot; ou &quot;MarketoSalesEngageCustomization&quot; na sua lista.

Pronto!

Veja a seguir uma lista de todos os objetos que precisam ser removidos da instância do Salesforce:

## Detalhes de Personalização de [!DNL Sales Connect] {#sales-connect-customization-details}

<table>
 <tr>
  <th>Campos de atividades personalizadas</th>
  <th>Descrição</th>
  <th>Tipo</th>
  <th>Tipo de dados</th>
 </tr>
 <tr>
  <td>[!UICONTROL ID de Presença Local de Chamada MSC]</td>
  <td>Como usuário, posso escolher Presença Local como uma opção quando faço chamadas do Telefone MSC. As chamadas recebidas mostrarão um número local para o receptor</td>
  <td>Atividade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL de Gravação de Chamada MSC]</td>
  <td>As chamadas podem ser gravadas e um link para a gravação será registrado aqui </td>
  <td>Atividade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>[!UICONTROL Campanha MSC]</td>
  <td>Registra o nome da campanha do MSC em que o contato/lead está</td>
  <td>Atividade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL DA CAMPANHA MSC]</td>
  <td>Registra o URL da campanha criada no MSC. Clicar nisso abrirá a campanha no aplicativo Web do MSC</td>
  <td>Atividade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>[!UICONTROL Etapa Atual da Campanha MSC]</td>
  <td>Se um contato/lead estiver em uma campanha, esse campo registrará o nome da etapa em que ele está no momento</td>
  <td>Atividade</td>
  <td>Caixa de seleção</td>
 </tr>
 <tr>
  <td>[!UICONTROL Anexo de Email MSC Exibido]</td>
  <td>Registra dados quando um email é enviado com um anexo que é visualizado pelo destinatário</td>
  <td>Atividade</td>
  <td>Caixa de seleção</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email MSC Clicado]</td>
  <td>Registra uma marca de seleção quando o destinatário clicar em um link no email</td>
  <td>Atividade</td>
  <td>Caixa de seleção</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email MSC Respondido]</td>
  <td>Registra uma marca de seleção quando o destinatário responde ao email</td>
  <td>Atividade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>[!UICONTROL Status de Email MSC]</td>
  <td>Mostra se um email foi enviado/está em andamento/foi rejeitado (o rastreamento dos emails devolvidos depende do canal de entrega usado)</td>
  <td>Atividade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>[!UICONTROL Modelo de email MSC]</td>
  <td>Registra o nome do modelo MSC que foi usado no email enviado ao cliente potencial/contato</td>
  <td>Atividade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL do Modelo de email do MSC]</td>
  <td>Registra o URL do modelo criado no MSC. Clicar nisso abrirá o modelo no aplicativo Web do MSC</td>
  <td>Atividade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL DE EMAIL DO MSC]</td>
  <td>Clicar nesse URL abrirá a central de comando no MSC e puxará a guia de histórico Exibição de detalhes do usuário, onde o usuário poderá ver o email enviado</td>
  <td>Atividade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email MSC Exibido]</td>
  <td>Registra uma marca de seleção quando o destinatário exibe um email</td>
  <td>Atividade</td>
  <td>Caixa de seleção</td>
 </tr>
</table>

<table>
 <tr>
  <th>Campo de Log de Rollup do MSC</th>
  <th>Descrição</th>
  <th>Tipo</th>
  <th>Tipo de dados</th>
 </tr>
 <tr>
  <td>MSC - Último engajamento de marketing</td>
  <td>Último envolvimento recebido de Marketing</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
  <td>Data e hora</td>
 </tr>
 <tr>
  <td>MSC - Última data de compromisso de marketing</td>
  <td>Carimbo de data e hora do envolvimento do Marketing</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
  <td>Data e hora</td>
 </tr>
 <tr>
  <td>MSC - Última descrição do compromisso de marketing</td>
  <td>Descrição do compromisso</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>MSC - Último envolvimento de marketing Source</td>
  <td>Source do engajamento de marketing</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>MSC - Último Tipo de Compromisso de Marketing</td>
  <td>Tipo de envolvimento (por exemplo: atividade da Web)</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>MSC - Última Atividade por Vendas</td>
  <td>Última atividade de saída executada pela equipe de vendas</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
  <td>Data e hora</td>
 </tr>
 <tr>
  <td>MSC - Última Resposta</td>
  <td>Última resposta de email para Email de vendas</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
  <td>Data e hora</td>
 </tr>
 <tr>
  <td>MSC - Campanha de vendas atual</td>
  <td>Registra o nome da campanha do MSC em que o contato/lead está</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
  <td>Texto</td>
 </tr>
 <tr>
  <td>MSC - Último contrato de vendas</td>
  <td>Último envolvimento recebido de Vendas</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
  <td>Data e hora</td>
 </tr>
 <tr>
  <td>MSC - Recusa</td>
  <td>Campo de recusa</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
  <td>Caixa de seleção</td>
 </tr>
</table>

<table>
 <tr>
  <th>Botões MSC</th>
  <th>Descrição</th>
  <th>Tipo</th>
 </tr>
 <tr>
  <td>[!UICONTROL Enviar Email MSC]</td>
  <td>Enviar emails de vendas de [!DNL Salesforce]</td>
  <td>
  <p>Conta 
  <p>Contato 
  <p>Lead 
  <p>Oportunidade</td>
 </tr>
 <tr>
  <td>[!UICONTROL Adicionar à Campanha MSC]</td>
  <td>Adicionar a campanhas do MSC de [!DNL Salesforce]</td>
  <td>
  <p>Contato
  <p>Lead</td>
 </tr>
 <tr>
  <td>[!UICONTROL Enviar para MSC]</td>
  <td>Contato de push de [!DNL Salesforce] para MSC</td>
  <td>
  <p>Contato
  <p>Lead</td>
 </tr>
 <tr>
  <td>[!UICONTROL Chamar com MSC]</td>
  <td>Fazer chamadas de vendas de [!DNL Salesforce]</td>
  <td>
  <p>Contato
  <p>Lead</td>
 </tr>
</table>

<table>
 <tr>
  <th>Botões de Ação em Massa do MSC</th>
  <th>Descrição</th>
  <th>Tipo</th>
 </tr>
 <tr>
  <td>[!UICONTROL Adicionar à Campanha MSC (Clássica)]</td>
  <td>Adicionar a campanhas do MSC de [!DNL Salesforce]</td>
  <td>
  <p>Contato
  <p>Lead</td>
 </tr>
 <tr>
  <td>[!UICONTROL Enviar para MSC (Clássico)]</td>
  <td>Contato de push de [!DNL Salesforce] para MSC</td>
  <td>
  <p>Contato
  <p>Lead</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email com MSC (Clássico)]</td>
  <td>Email com MSC de [!DNL Salesforce]</td>
  <td>
  <p>Contato
  <p>Lead</td>
 </tr>
</table>
