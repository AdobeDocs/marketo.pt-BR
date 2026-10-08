---
solution: Marketo Engage
product: marketo
title: Editar modelos de email com o editor avançado do HTML
description: Saiba como visualizar e editar o código-fonte bruto do HTML no Marketo Engage Email Designer, incluindo medidas de proteção, etapas de acesso e limitações principais.
level: Intermediate
feature: Email Designer
exl-id: b030e56a-de70-4b0d-9788-04a01235cffb
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c2dbad80-0f5c-4d96-a798-2a65f93b8721
    internal-label: Assets
subfeature_v2:
  - id: f8f7d99a-f455-45bb-8028-428a55a7130b
    internal-label: Email Designer
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%
---
# Editar modelos de email com o editor avançado do HTML {#advanced-html-mode}

O modo HTML avançado permite exibir e editar o código fonte bruto de modelos de email diretamente da interface do Designer de email do [!DNL Marketo Engage].

Esse recurso permite inserir expressões avançadas diretamente na origem. Ao voltar para a visualização visual (desktop), o conteúdo é renderizado novamente para que você possa verificar sua aparência e continuar editando em ambas as visualizações.

## Medidas de proteção {#guardrails}

Ao usar o editor avançado do HTML, as seguintes medidas de proteção protegem a compatibilidade do conteúdo e definem expectativas.

* O editor avançado do HTML **não valida** seu código. Ele não verifica erros de sintaxe ou layouts com falha. Revise seu conteúdo cuidadosamente antes de salvar.

* Atualizações futuras do sistema podem substituir as alterações feitas na marcação padrão. **As alterações não podem persistir**.

* [!DNL Adobe] suporte **não pode solucionar ou resolver** problemas causados por código personalizado e alterações manuais. Mantenha um backup do seu conteúdo caso precise reverter.

* Não é possível simular conteúdo na visualização avançada do HTML. Alterne para o modo de exibição de Área de Trabalho para visualizar seu conteúdo.

* Para garantir a compatibilidade do conteúdo, **não é possível salvar** no modo de exibição avançado do HTML. Volte para a exibição da área de trabalho quando estiver pronto para salvar suas alterações.

## Acessar o modo HTML avançado {#access-html-mode}

Para abrir o editor avançado do HTML e editar a fonte do modelo, siga estas etapas.

1. Abra ou [crie um modelo de email](/help/marketo/product-docs/email-marketing/email-designer/email-template-authoring.md#create-an-email-template) no Designer de email.

1. Na tela _Editar modelo de email_, clique no botão HTML no canto superior direito.

   ![](assets/advanced-html-mode-1.png){width="800" zoomable="yes"}

1. Na primeira vez que você abrir o editor avançado do HTML, uma mensagem de aviso será exibida. Revise e clique em **[!UICONTROL OK]** quando terminar.

   ![](assets/advanced-html-mode-2.png)

   >[!NOTE]
   >
   >Este aviso é exibido na primeira vez que você abre o editor avançado do HTML e redefine a cada mês.

1. O editor avançado do HTML é exibido.

   ![](assets/advanced-html-mode-3.png){width="800" zoomable="yes"}

1. Adicione as alterações desejadas ao conteúdo do email.

   >[!WARNING]
   >
   >Insira o código HTML e CSS correto, pois não há um processo de validação de sintaxe e o Suporte da Adobe não pode ajudar com as edições do HTML.

1. A simulação e o salvamento de conteúdo não estão disponíveis na visualização avançada do HTML por motivos de compatibilidade. Volte para a exibição da área de trabalho para visualizar seu conteúdo e salvar suas alterações.

   ![](assets/advanced-html-mode-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >As edições são preservadas ao alternar entre exibições.
