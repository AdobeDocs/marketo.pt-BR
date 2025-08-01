---
description: Etapa 1 de 3 - Adicionar campos do Marketo à Salesforce (Enterprise/Unlimited) - Documentação do Marketo - Documentação do produto
title: Etapa 1 de 3 - Adicionar campos do Marketo à Salesforce (Enterprise/Unlimited)
hide: true
hidefromtoc: true
feature: Salesforce Integration
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Etapa 1 de 3: Adicionar campos do Marketo à Salesforce (Enterprise/Unlimited) {#step-of-add-marketo-fields-to-salesforce-enterprise-unlimited}

>[!PREREQUISITES]
>
>Você deve ter acesso às APIs do Salesforce para sincronizar entre o Marketo Engage e o Salesforce.

O Marketo usa um conjunto de campos para capturar determinados tipos de informações relacionadas a marketing. Se quiser esses dados no Salesforce, siga as instruções abaixo.

1. Crie três campos personalizados no Salesforce no cliente potencial e objetos de contato: Pontuação, Programa de aquisição e Data de aquisição.
1. Mapeie esses campos personalizados entre clientes potenciais e contatos para que, na conversão no Salesforce, os valores continuem.
1. Você pode criar outros campos adicionais, se necessário (consulte a tabela abaixo).

Todos esses campos personalizados são opcionais e não são necessários para sincronizar o Marketo e o Salesforce. Como prática recomendada, é recomendado criar campos para Pontuação, Programa de aquisição e Data de aquisição.

## Adicionar campos do Marketo à Salesforce {#add-marketo-fields-to-salesforce}

Adicione três campos personalizados aos objetos de cliente potencial e contato no Salesforce listados acima. Se quiser adicionar mais, consulte a tabela de campos disponíveis no final desta seção.

Execute as etapas a seguir para cada um dos três campos personalizados para adicioná-los. Comece com Pontuação.

1. Faça logon no Salesforce e clique em Configurar.

   CAPTURA DE TELA

1. Na Localização Rápida, procure a palavra &quot;Objeto&quot;

   CAPTURA DE TELA

1. Clique em Gerenciadores de objetos e procure por &quot;Clientes potenciais&quot;

   CAPTURA DE TELA

1. Clique em Lead em RÓTULO e, em seguida, clique em Campos e Relações à esquerda.

   CAPTURA DE TELA

1. Clique no botão Novo na página &quot;Campos e relacionamentos&quot;

   CAPTURA DE TELA

1. Escolha o tipo de campo apropriado (para Pontuação - número; Programa de aquisição - texto; Data de aquisição - Data/hora).

   CAPTURA DE TELA

1. Clique em Avançar.

   CAPTURA DE TELA

1. Insira o Rótulo do campo, Comprimento e Nome do campo do campo, conforme mostrado na tabela abaixo.

   TABELA

   >[!NOTE]
   >
   >O Salesforce anexa __c a Nomes de campos quando os usa para criar Nomes de API.

   CAPTURA DE TELA

   >[!NOTE]
   >
   >Os campos de texto e número exigem comprimento, mas os campos de Data/Hora não. Uma descrição é opcional.

1. Clique em Avançar.

   CAPTURA DE TELA

1. Especifique as configurações de acesso e clique em Próximo:

   Definir todas as funções como Visível e Somente Leitura

   Desmarque a caixa de seleção Somente leitura para o perfil do seu usuário de sincronização:

   Se você tiver um usuário com o perfil de Administrador do sistema como o usuário de sincronização, desmarque a caixa de seleção Somente leitura do perfil de Administrador do sistema (como mostrado abaixo)
Se você criou um perfil personalizado para o usuário de sincronização, desmarque a caixa de seleção Somente leitura desse perfil personalizado

   CAPTURA DE TELA

1. Escolha os layouts de página que devem exibir o campo.

   CAPTURA DE TELA

1. Clique em Salvar e novo para voltar e criar cada um dos outros dois campos personalizados. Clique em Salvar ao concluir com todos os três.

   CAPTURA DE TELA

* No Gerenciador de objetos, pesquise &quot;Contatos&quot;. Clique em Campos e relacionamentos.
* Execute as etapas de 5 a 12 para os campos Pontuação, Data de aquisição e Programa de aquisição no objeto de contato, da mesma forma que fazia para o objeto de lead.
* Como opção, use o procedimento acima para qualquer campo personalizado adicional desta tabela.

  TABELA

  >[!NOTE]
  >
  >Os valores nos campos atribuídos automaticamente pelo Marketo não estarão imediatamente disponíveis no Salesforce quando o novo campo for criado. O Marketo sincronizará os dados com o Salesforce na próxima atualização do registro em qualquer sistema (ou seja, uma atualização para qualquer um dos campos sincronizados entre o Marketo e o Salesforce).

## Mapear campos personalizados para conversões {#map-custom-fields-for-conversions}

Um campo personalizado no objeto de cliente potencial no Salesforce deve ser mapeado para um campo de contato no objeto de contato para que os dados sejam transportados quando ocorrer uma conversão.

1. No canto superior direito, clique em Configurar.

   CAPTURA DE TELA

1. Na Localização Rápida, procure a palavra &quot;Objeto&quot;

   CAPTURA DE TELA

1. Vá para a seção Relacionamentos e campos personalizados de lead e clique em Mapear campos de lead

   CAPTURA DE TELA

1. Clique na lista suspensa ao lado do campo que deseja mapear, na guia correspondente - conta, contato ou oportunidade .

   CAPTURA DE TELA

1. Selecione o campo personalizado de contato correspondente.

   CAPTURA DE TELA

1. Repita as etapas acima para qualquer outro campo criado.

1. Clique em Salvar ao concluir.
