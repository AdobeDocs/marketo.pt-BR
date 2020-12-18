---
unique-page-id: 4720108
description: Ativar a barra de recomendação de conteúdo - Documentos de marketing - Documentação do produto
title: Ativar a barra de recomendação de conteúdo
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---


# Ativar a barra de recomendação de conteúdo {#enable-the-content-recommendation-bar}

O mecanismo de recomendação de conteúdo usa análises preditivas e algoritmos de aprendizado de máquina para fornecer conteúdo relevante a cada visitante da Web. O mecanismo de recomendação prevê qual conteúdo teria melhor desempenho por visitante. O conteúdo do mecanismo é monitorado e controlado na página do Recommendations, ajudando a otimizar o retorno sobre o investimento do seu conteúdo.

>[!PREREQUISITES]
>
>Antes de ativar o conteúdo preditivo, você deve:
>
>* [Preparar seu conteúdo preditivo](http://docs.marketo.com/display/docs/edit+predictive+content)
>* [Aprovar um título para conteúdo previsível](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Ativar e personalizar a barra de recomendação de conteúdo {#enable-and-customize-the-content-recommendation-bar}

1. Vá para **Configurações de conteúdo**.

   ![](assets/settings-dropdown-hand.png)

1. Clique em **Barra**.

   ![](assets/content-settings-bar-hand.png)

1. Para habilitar a Barra de recomendação para um URL, basta clicar em **On** e em **Salvar**.

   ![](assets/bar-enable.png)

1. Para personalizar um URL, selecione cores, estilo, formato, setas para a barra de recomendações e páginas para incluir ou excluir a barra. Personalize para se ajustar à marca do site. Clique em **Salvar**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Incluir / Excluir URL de exibição**
   >
   >    * O URL de exibição deve ser o caminho do domínio
   >    * Não inclua http:// ou https://
   >    * Usar * para curingas
   * Usar ponto e vírgula como separador
   * Exemplo: /contact_us*; *action=logout*
   * Esse campo diferencia maiúsculas de minúsculas


## Considerações da Barra de Recomendações {#recommendation-bar-considerations}

* É necessário pelo menos um conteúdo para que a barra de recomendações seja definida como **On** na página do Recommendations para que o mecanismo de recomendação funcione. Se nenhum conteúdo estiver ativado e a barra estiver definida como **On**, o efeito Seta será exibido na parte inferior direita da página da Web, mas nenhum conteúdo recomendado será exibido.

* Quanto mais conteúdo for executado no mecanismo de recomendação, melhor será para o algoritmo testar e saber qual conteúdo funciona melhor. Recomendamos começar com 10 a 20 itens de conteúdo em execução e ativos e continuar adicionando novos.
* O conteúdo que você habilita para a recomendação deve incluir a tag RTP Javascript. Isso ajuda o algoritmo a rastrear e otimizar o conteúdo recomendado.

>[!NOTE]
**Artigos relacionados**
* [Ativar conteúdo preditivo para mídias avançadas da Web](enable-predictive-content-for-web-rich-media.md)

