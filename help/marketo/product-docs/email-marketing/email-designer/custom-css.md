---
solution: Marketo Engage
product: marketo
title: Adicionar CSS personalizado ao conteúdo do email
description: Saiba como adicionar CSS personalizado ao seu conteúdo de email diretamente no Designer de email no Marketo Engage.
level: Intermediate
feature: Email Designer
exl-id: c191b44a-47ab-41f8-aa95-9268e359e5db
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 4%

---

# Adicionar CSS personalizado ao conteúdo do email {#custom-css}

Adicione seu próprio CSS personalizado diretamente no Designer de email do Marketo Engage para obter um estilo avançado e específico.

## Definir CSS personalizado {#define-custom-css}

1. Verifique se há conteúdo definido no Designer de email adicionando pelo menos um componente.

1. Selecione **[!UICONTROL Corpo]**, na **[!UICONTROL Árvore de navegação]** à esquerda ou no painel direito. **[!UICONTROL Estilos CSS]** são exibidos à direita.

   ![](assets/custom-css-1.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >A seção **[!UICONTROL Estilos CSS]** só está disponível quando há conteúdo no editor.

1. Clique no botão **[!UICONTROL + Adicionar CSS personalizado]**.

   >[!NOTE]
   >
   >O botão **[!UICONTROL Adicionar CSS personalizado]** só está disponível quando **[!UICONTROL Corpo]** é selecionado. No entanto, você pode aplicar estilos CSS personalizados a todos os componentes dentro do conteúdo.

1. Insira seu código CSS na área de texto dedicada que aparece. Verifique se o CSS personalizado [ é válido e segue a sintaxe adequada](#use-valid-css). Clique em **Salvar** quando terminar.

   ![](assets/custom-css-2.png)

   >[!NOTE]
   >
   >Você não pode adicionar CSS personalizado ao seu conteúdo ao usar um [modelo com conteúdo bloqueado](/help/marketo/product-docs/email-marketing/email-designer/content-locking.md). O rótulo do botão é alterado para **[!UICONTROL Exibir CSS personalizado]** e qualquer CSS personalizado exibido é somente leitura.

1. Certifique-se de que o CSS se aplique ao seu conteúdo. Caso contrário, verifique a seção [Solução de problemas](#troubleshooting).

   ![](assets/custom-css-3.png)

   >[!NOTE]
   >
   >Se você remover todo o conteúdo, a seção desaparecerá e o CSS personalizado definido anteriormente não será mais aplicado. Adicione conteúdo de volta para fazer com que a seção **[!UICONTROL Estilos CSS]** reapareça. O CSS personalizado é aplicado novamente.

## Uso de CSS válido {#using-valid-css}

Você pode inserir qualquer string CSS válida na área de texto **[!UICONTROL Adicionar CSS personalizado]**. O CSS adequadamente formatado é aplicado imediatamente ao conteúdo.

>[!CAUTION]
>
>Você é responsável pela segurança do CSS personalizado. Certifique-se de que o CSS não introduza vulnerabilidades ou conflitos com o conteúdo existente.
>
>Evite usar CSS que possa quebrar involuntariamente o layout ou a funcionalidade do conteúdo.

+++ Exemplos de CSS válido

Abaixo estão exemplos de CSS válido.

```css
.acr-component[data-component-id="form"] {
  display: flex;
  justify-content: center;
  background: none;
}

.acr-Form {
  width: 100%;
  padding: 20px 100px;
  border-spacing: 0px 8px;
  box-sizing: border-box;
  margin: 0;
}

.acr-Form .spectrum-FieldLabel {
  width: 20%;
}

.acr-Form.spectrum-Form--labelsAbove .spectrum-FieldLabel,
.acr-Form [data-form-item="checkbox"] .spectrum-FieldLabel {
  width: auto;
}

.acr-Form .spectrum-Textfield {
  width: 100%;
}

#acr-form-error,
#acr-form-confirmation {
  width: 100%;
  padding: var(--spectrum-global-dimension-static-size-500);
  display: flex;
  align-items: center;
  flex-direction: column;
  justify-content: center;
  gap: var(--spectrum-global-dimension-static-size-200);
}

.spectrum-Form-item.is-required .spectrum-FieldLabel:after{
  content: '*';
  font-size: 1.25rem;
  margin-left: 5px;
  position: absolute;
}

/* Error field placeholder */
.spectrum-HelpText {
  display: none !important;
}

.spectrum-HelpText.is-invalid,
.is-invalid ~ .spectrum-HelpText {
  display: flex !important;
}
```

```css
@media only screen and (min-width: 600px) {
  .acr-paragraph-1 {
    width: 100% !important;
  }
}
```

+++

+++ Exemplos de CSS inválido

Se um CSS inválido for inserido, uma mensagem de erro será exibida, indicando que o CSS não pode ser salvo. Abaixo estão exemplos de CSS inválido.

O uso de `<style>` tags não é aceito:

```html
<style type="text/css">
  .acr-Form {
    width: 100%;
    padding: 20px 100px;
    border-spacing: 0px 8px;
    box-sizing: border-box;
    margin: 0;
  }
</style>
```

Sintaxe inválida, como chaves ausentes, não é aceita:

```css
body {
  background: red;
```

+++

## Implementação técnica {#implementation}

Seu CSS personalizado é adicionado ao final da seção `<head>` como parte de uma marca `<style>` com o atributo `data-name="global-custom"`, como no exemplo abaixo. Isso garante que os estilos personalizados sejam aplicados globalmente ao conteúdo.

+++ Ver exemplo

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="content-version" content="3.3.31">
    <meta name="x-apple-disable-message-reformatting">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <style data-name="default" type="text/css">
      td { padding: 0; }
      th { font-weight: normal; }
    </style>
    <style data-name="grid" type="text/css">
      .acr-grid-table { width: 100%; }
    </style>
    <style data-name="acr-theme" type="text/css" data-theme="default" data-variant="0">
      body { margin: 0; font-family: Arial; }
    </style>
    <style data-name="media-default-max-width-500px" type="text/css">
      @media screen and (max-width: 500px) {
        body { width: 100% !important; }
      }
    </style>
    <style data-name="global-custom" type="text/css">
      /* Add you custom CSS here */
    </style>
  </head>
  <body>
    <!-- Minimal content -->
  </body>
</html>
```

+++

O CSS personalizado não é interpretado ou validado pelo painel **[!UICONTROL Configurações]** do Email Designer. Ela é totalmente independente e só pode ser modificada por meio da opção **[!UICONTROL Adicionar CSS personalizado]**.

### Grades de Proteção - Conteúdo importado {#guardrails}

Se você quiser usar o CSS personalizado com o conteúdo importado para o Designer de email, considere o seguinte:

* Se [você estiver importando conteúdo externo do HTML](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#import-html), incluindo CSS, a menos que converta esse conteúdo, ele estará no **[!UICONTROL Modo de compatibilidade]**, onde a seção **[!UICONTROL Estilos CSS]** não está disponível.

* Se a importação de conteúdo criado com o Designer de email incluir CSS aplicado por meio da opção **[!UICONTROL Adicionar CSS personalizado]**, o CSS aplicado anteriormente ficará visível e poderá ser editado na mesma opção.

## Solução de problemas {#troubleshooting}

Se o CSS personalizado não for aplicado, tente as sugestões abaixo.

* Verifique se o CSS é válido e está livre de erros de sintaxe (como chaves ausentes, nomes de propriedades incorretos). [Saiba como](#use-valid-css)

* Verifique se o CSS está sendo adicionado à tag `<style>` com o atributo `data-name="global-custom"`.

* Verifique se a marca de estilo `global-custom` tem o atributo `data-disabled` definido como `true`. Nesse caso, o CSS personalizado não será aplicado.

+++ Por exemplo:

  ```html
  <style data-name="global-custom" type="text/css" data-disabled="true"> body: { color: red; } </style>
  ```

+++

* Certifique-se de que o CSS não seja substituído por outras regras CSS.

   * Use as ferramentas de desenvolvedor do navegador para inspecionar o conteúdo e verificar se o CSS está direcionando os seletores corretos.

   * Considere adicionar `!important` às suas declarações para garantir que elas tenham prioridade.

+++ Por exemplo:

     ```css
     .acr-Form {
       background: red !important;
     }
     ```

+++

>[!NOTE]
>
>O Suporte do Marketo Engage não está configurado para ajudar na solução de problemas de CSS personalizado. Para obter assistência sobre CSS, consulte um desenvolvedor da Web.
