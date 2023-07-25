---
description: Notas de versão - agosto de 2021 - Documentação do Marketo - Documentação do produto
title: Notas de versão - agosto de 2021
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Notas de versão: agosto de 2021 {#release-notes-aug-21}

Os seguintes recursos estão incluídos na versão de agosto de 2021. Verifique a disponibilidade de recursos na sua edição do Marketo Engage.

>[!AVAILABILITY]
>
>Recursos indicados por uma estrela (![](assets/yellow-star.png)) são complementos pagos. Entre em contato com seu representante da Adobe Marketo Engage para obter mais informações.

**_Versões trimestrais_**

Os seguintes recursos serão lançados em **20 de agosto de 2021**.

## Automação de experiência {#experience-automation}

* **Autenticação de usuário Marketo Engage por meio da identidade Adobe**: Em breve, novos usuários do Marketo Engage com pacotes Enterprise serão integrados usando as credenciais de usuário do Adobe ID. A migração dos atuais utilizadores para o sistema de identidade integrado só ocorrerá em meados de 2022 e não é necessária qualquer ação até nova ordem. A autenticação de usuário de identidade de Adobe permite que os administradores de TI/segurança gerenciem várias instâncias de produtos de Marketo Engage juntamente com outras soluções de Experience Cloud, além de configurar o SSO por meio de um console comum. Os administradores podem gerenciar convenientemente grupos de usuários e direitos de usuário em um único local.

* **Aninhamento de campanha executável**: as campanhas executáveis agora também podem chamar outras campanhas executáveis, permitindo que você as aninhe em até três níveis. Isso permite uma maior consolidação de fluxos operacionais comuns e melhora o gerenciamento do Smart Campaign.

* **Página Ação de Fluxo Único em Detalhes da Pessoa** (Disponível até 9 de setembro): Execute ações de fluxo como enviar email, alterar o proprietário da pessoa ou qualquer outra ação de campanha inteligente em pessoas individuais na página de detalhes da pessoa usando o menu de ação de fluxo sem alternar para a exibição de grade do banco de dados.

* **[Exportar atividades personalizadas](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: a exportação de metadados agora é compatível com todos os objetos e respectivos metadados que podem ser usados para compartilhar, analisar e projetar seu modelo de dados de assinatura.

## Aprimoramentos na API {#api-enhancements}

* **Enviar API de formulário**: quando um endereço de email é duplicado em dois ou mais registros de cliente potencial, atualizamos o registro &quot;atualizado pela última vez&quot; em vez de ignorarmos completamente. Fornece paridade com a API do Forms 2.0.

* **API de e-mail**: recupere ativos de email de campeões ou desafiantes. Recupere ativos de email usando o filtro de intervalo de datas.

**_Lançamento durante todo o trimestre_**

Os recursos a seguir estão em um ciclo não trimestral e serão lançados nos próximos meses.

## Sales Insight {#sales-insight}

![(estrela)](assets/yellow-star.png)

* **Maior visibilidade das atividades de lead, contato, conta e oportunidade para usuários do Salesforce CRM**: o engajamento com clientes potenciais durante longos ciclos de vendas é mais bem informado devido a um maior número de registros de engajamento no Sales Insight. As guias de momentos interessantes, atividade da Web, email e pontuação mostram até 400 atividades em objetos de cliente potencial, contato, conta e oportunidade.

## SalesConnect {#sales-connect}

![(estrela)](assets/yellow-star.png)

* **Limitação Da Conexão De Email (Beta)**: melhore a capacidade de entrega de email e dimensione a comunicação de vendas personalizada com a limitação da conexão de email para o Sales Connect. Essa nova tecnologia gerencia automaticamente o tempo de envio de email para criar experiências perfeitas para usuários do Exchange e do Gmail. Diminua ou elimine o uso de aplicativos de envio de email de terceiros em massa e envie todos os seus emails do Sales Connect com confiança.

>[!NOTE]
>
>A limitação de email está disponível na versão beta agora. [Saiba mais](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Insights aprimorados das atividades de vendas**: capture e ative o engajamento personalizado com base nas atividades anteriores de sua equipe de vendas. Novos atributos, como Link de registro de chamada de vendas, Nome da campanha de vendas e Assunto do email de vendas, podem ser usados nas listas inteligentes de Marketo Engage.  Essas atividades podem ser exportadas e relatadas por meio da API REST do Marketo Engage ou Exportação em massa e estão disponíveis em filtros e acionadores como restrições adicionais para smart lists.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integração Bizible LinkedIn Lead Gen Forms**: os profissionais de marketing agora podem executar a atribuição de receita em conversões que ocorrem quando o LinkedIn captura preenchimentos de formulário por meio de suas unidades de anúncio de geração de lead Forms. Esses insights podem ser usados para otimizar o desempenho do formulário e os investimentos em mídia paga. A linkedIn Lead Gen Forms é uma das ofertas de mídia paga de crescimento mais rápido da LinkedIn e esse novo recurso está incluído em nossa integração existente do LinkedIn Ads com a Bizible.

* **Painel do Velocity aprimorado**: adicionamos uma nova métrica de velocidade e um filtro de painel para obter insights mais profundos. Esse painel é usado pelos profissionais de marketing para entender a velocidade do lead e da oportunidade estágio por estágio e a eficiência de diferentes formas de envolvimento de marketing e vendas.

* **Novo painel de Jornada em cascata de coorte**: isso permitirá que os profissionais de marketing visualizem a progressão de um coorte selecionado por meio de um conjunto clássico de estágios &quot;em cascata de demanda&quot;, fornecendo um rápido entendimento das taxas de conversão e da causalidade de conversão implícita no estágio em cada estágio.

## Integração da Bizible com o Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Esta seção inclui novos recursos para usuários da Bizible que concluíram a migração do Adobe Identity Management System (IMS). Se tiver migrado, você verá seu novo Adobe ID nas Configurações da Bizible na guia Adobe ID. Todas as contas devem ser migradas até o final de 2021.

* **Integração da Bizible com o Adobe Privacy Service** (disponível em setembro de 2021): a integração da Bizible com o Privacy Service Adobe centraliza a conformidade com as regulamentações críticas de privacidade de dados (como o GDPR) em todos os aplicativos da Adobe Experience Cloud. Agora você pode aproveitar esse serviço e gerenciar todas as solicitações de privacidade centralmente para que as solicitações de alteração que entram na Bizible e outros produtos Adobe sejam refletidas em todos os aplicativos.

* **Bizible na Interface do Adobe Experience Cloud**: a adoção da Adobe Experience Cloud Interface pela Bizible oferece aos usuários novos recursos que aparecerão na barra de cabeçalho do aplicativo Bizible e incluem melhor acesso a recursos de suporte e alternância de aplicativos. A interface de Experience Cloud ajuda a criar uma experiência consistente entre o Bizible e outros aplicativos da Adobe Experience Cloud.

* **Propriedade de domínio da Bizible e autogestão**: os usuários da Bizible podem aproveitar o Adobe Admin Console para gerenciar os domínios que desejam que a Bizible rastreie. Isso leva o autoatendimento a um processo anteriormente manual e fornece uma experiência consistente sobre como a propriedade e o rastreamento de domínios são gerenciados nos aplicativos da Adobe Experience Cloud.

## Anúncios {#announcements}

* **Atualização das Configurações de ID universal da assinatura**: para oferecer suporte à futura integração de Marketo Engage e Adobe Identity para os usuários existentes, todas as assinaturas de Marketo Engage serão unificadas na habilitação do suporte à Universal ID. Mais informações [pode ser encontrado aqui](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webinário de lançamento do produto_**

[Webinário da versão de agosto de 2021 do Marketo Engage](https://engage.marketo.com/August21_Release_Webinar.html)
