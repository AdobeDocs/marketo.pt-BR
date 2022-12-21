---
unique-page-id: 14352475
description: Instalar campos de evento do Sales Connect no Histórico de atividades - Documentos do Marketo - Documentação do produto
title: Instalar campos de evento do Sales Connect no histórico de atividades
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Instalar campos de evento do Sales Connect no histórico de atividades {#install-sales-connect-event-fields-on-activity-history}

Depois de instalar o pacote Enterprise no Salesforce, você pode instalar os campos de evento Sales Connect na seção do histórico de atividades. Os campos de evento Conexão de Vendas incluem informações como exibições, cliques e campanhas. Isso permite ter informações sobre seus emails importados diretamente para o Salesforce.

Certifique-se de fazer a equipe com o administrador do Salesforce ao executar essas etapas. Neste exemplo, instalaremos os campos no **Layout de Página de Clientes Potenciais**. Também é possível instalar os campos no Contato, Conta e Layouts de Página de Oportunidade. Lembre-se, ao registrar emails em Contas e Oportunidades, você precisará do contato que está enviando por email associado como uma função de contato.

1. Clique em **Configuração**.
1. Clique em **Personalizar**.
1. Clique em **Clientes potenciais**.
1. Clique em **Layouts de página**.
1. Clique em **Editar** ao lado do layout da página que você deseja alterar.

   >[!NOTE]
   >
   >O Sales Connect instalará alguns layouts de página para você, mas se você já tiver um padrão que sua equipe esteja usando, será necessário instalá-lo lá. Você pode excluir os layouts de página da Conexão de Vendas se não quiser usá-los.

1. Role para baixo até a seção Histórico de atividades .
1. Clique na chave inglesa para editar.
1. Selecione os campos Conexão de Vendas que deseja incluir na seção Histórico de Atividades . Se você não estiver vendo os campos Sales Connect aqui, talvez tenha instalado o pacote Salesforce errado.
1. Clique em **Adicionar** para mover os campos desejados.
1. Clique em **OK**.
1. Clique em **Salvar**.

   Seus usuários agora podem ver informações valiosas e atualizações sobre seus emails no Salesforce!
