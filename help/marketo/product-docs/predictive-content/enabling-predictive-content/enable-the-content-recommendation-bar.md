---
unique-page-id: 4720108
description: Ativar a barra de recomendação de conteúdo - Documentos do Marketo - Documentação do produto
title: Ativar a Barra de Recomendação de Conteúdo
exl-id: f2244db1-51a9-4e26-9bf7-b2c79df25552
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Ativar a Barra de Recomendação de Conteúdo {#enable-the-content-recommendation-bar}

O mecanismo de recomendação de conteúdo usa análises preditivas e algoritmos de aprendizado de máquina para fornecer conteúdo relevante a cada visitante da Web. O mecanismo de recomendação prevê qual conteúdo terá melhor desempenho por visitante. O conteúdo do mecanismo é monitorado e controlado na página do Recommendations, ajudando você a otimizar o ROI do conteúdo.

>[!PREREQUISITES]
>
>Antes de ativar o Conteúdo preditivo, você deve:
>
>* **Preparar seu conteúdo preditivo**
   >
   >   * [Editar conteúdo preditivo para emails](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md) ou
   >   * [Editar conteúdo preditivo para mídias avançadas](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md) ou
   >   * [Editar conteúdo preditivo para a barra de recomendação](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md)
>
>* [Aprovar um título para conteúdo preditivo](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md)


## Ativar e personalizar a barra de recomendação de conteúdo {#enable-and-customize-the-content-recommendation-bar}

1. Ir para **Configurações de conteúdo**.

   ![](assets/settings-dropdown-hand.png)

1. Clique em **Barra**.

   ![](assets/content-settings-bar-hand.png)

1. Para ativar a Barra de recomendação de um URL, basta clicar em **Ligado** e depois **Salvar**.

   ![](assets/bar-enable.png)

1. Para personalizar um URL, selecione cores, estilo, formato, setas para a barra de recomendação e páginas para incluir ou excluir a barra. Personalizar para ajustar a marca de seu site. Clique em **Salvar**.

   ![](assets/bar-customize-details-hands.png)

   >[!NOTE]
   >
   >**Incluir / Excluir URL de exibição**
   >
   >* O URL de exibição deve ser o caminho do domínio
   >* Não inclua https:// ou https://
   >* Use &#42; para curingas
   >* Usar ponto e vírgula como separador
   >* Exemplo: /contact_us&#42;; &#42;action=logout&#42;
   >* Este campo diferencia maiúsculas de minúsculas


## Considerações sobre a barra de recomendação {#recommendation-bar-considerations}

* Você precisa de pelo menos um conteúdo para a barra de recomendações definida como **Ligado** na página Recommendations para que o mecanismo do Recommendation funcione. Se nenhum conteúdo estiver ativado e a Barra estiver definida como **Ligado**, o efeito Seta será exibido na parte inferior direita da página da Web, mas nenhum conteúdo recomendado será exibido.

* Quanto mais conteúdo estiver sendo executado no mecanismo de recomendação, melhor será o algoritmo testar e aprender qual conteúdo funciona melhor. Recomendamos começar com 10 a 20 partes de conteúdo em execução e ativas e continuar adicionando novas.
* A parte de conteúdo que você habilita para a recomendação deve incluir a tag Javascript RTP. Isso ajuda o algoritmo a rastrear e otimizar o conteúdo recomendado.

>[!MORELIKETHIS]
>
>[Ativar conteúdo preditivo para mídia avançada da Web](/help/marketo/product-docs/predictive-content/enabling-predictive-content/enable-predictive-content-for-web-rich-media.md)
