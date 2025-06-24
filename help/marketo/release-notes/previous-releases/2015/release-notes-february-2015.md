---
unique-page-id: 6094890
description: Notas de versão - fevereiro de 2015 - Documentação do Marketo - Documentação do produto
title: Notas de versão - fevereiro de 2015
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 13%

---

# Notas de versão: fevereiro de 2015 {#release-notes-february}

Os seguintes recursos estão incluídos na versão de fevereiro de 2015. Verifique a disponibilidade de recursos na sua Marketo Edition. Após o lançamento, não se esqueça de voltar para encontrar links para artigos detalhados para cada recurso. Rolo de tambor...

## Aprimoramentos de automação de marketing {#marketing-automation-enhancements}

**[Mover campanha inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

Alegre-se! Agora você pode arrastar e soltar ou usar o recurso Mover, da árvore, para incluir ou retirar campanhas inteligentes de programas.

**[[!DNL Dynamics] 2015 (Online)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** - com suporte!

**Alterações no Certificado HTTPS**

Para proteger a confidencialidade e a integridade dos dados do cliente e dos serviços SaaS, a Marketo segue as práticas recomendadas do setor de SaaS

e substituirá os protocolos de segurança atualmente usados (SHA-1 e SSL) por versões mais seguras (SHA-2 (também conhecido como SHA-256) e TLS) para os seguintes domínios:

* marketo.net (tráfego [!DNL Munchkin] criptografado)

* [marketo.com](https://marketo.com) (principais aplicativos SaaS)

Isso ocorrerá logo após essa versão. O protocolo SHA-1 terá suporte temporário no domínio [mktoapi.com](https://mktoapi.com) até dezembro de 2015 para permitir que os proprietários de sistemas e aplicativos herdados atualizem seus sistemas com compatibilidade SHA-2.

**Seguro[!DNL Munchkin]**

Estamos removendo nosso suporte para SSL3. Mantivemos o SSL3 até agora para manter o suporte para navegadores antigos, mas em 2015 não estamos mais vendo tráfego significativo da Web desses navegadores. Isso só afetaria o [!DNL Munchkin] quando usado em páginas seguras e será implantado lentamente após o lançamento de fevereiro.

## Aprimoramentos do Real-Time Personalization {#real-time-personalization-enhancements}

**[URL de Destino para Campanhas](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Selecione as páginas nas quais você deseja que sua campanha em tempo real seja exibida usando &quot;Adicionar um URL de direcionamento&quot;. Esse recurso funciona com todos os tipos de campanha (caixa de diálogo, na zona, widgets), mas é especialmente valioso para campanhas na zona, onde uma campanha será renderizada na ID da zona somente para o URL de destino selecionado. Ela é compatível com a adição de vários URLs para direcionar páginas da Web diferentes.

![](assets/image2015-2-19-11-3a0-3a30.png)

**País e Estado adicionados ao direcionamento baseado em conta**

Agora é possível adicionar país e estado a Listas de contas nomeadas. Direcionar potenciais contas chave de locais específicos.
