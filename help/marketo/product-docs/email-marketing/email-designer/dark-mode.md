---
description: Modo escuro — Documentação do Marketo — Documentação do produto
title: Modo escuro
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: f960d7918d97a2c5e3d16673bc4c5c592004ff1e
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 1%

---

# Modo escuro {#dark-mode}

Ao criar seus emails, o Designer de Email permite alternar para o modo de exibição **[!UICONTROL Escuro]**.

No **[!UICONTROL modo escuro]**, você pode definir configurações personalizadas específicas a serem exibidas ao oferecer suporte a clientes de email quando o modo escuro estiver ativado.

## O que é o modo escuro? {#what-is-dark-mode}

O modo escuro permite que clientes de email e aplicativos exibam emails com planos de fundo mais escuros e cores mais claras para texto, botões e outros elementos da interface do usuário. Ele ajuda a reduzir a tensão ocular, economiza bateria e melhora a legibilidade em ambientes com pouca luz, para proporcionar uma experiência de visualização mais confortável.

## Medidas de proteção {#guardrails}

A renderização no modo escuro pode variar bastante em clientes de email diferentes.

Antes de usar o modo escuro, é importante entender como os principais clientes de email lidam com ele. Há três casos a distinguir:

### Clientes sem suporte para o modo escuro {#not-supporting}

Alguns clientes de email não oferecem suporte a esse recurso, como:

* Yahoo!Mail
* AOL

Esses clientes de email nunca exibem nenhuma renderização no modo escuro, independentemente de você definir ou não as configurações personalizadas do modo escuro.

### Clientes que aplicam seu próprio modo escuro {#default-support}

Alguns clientes de email aplicam sistematicamente seu próprio modo escuro padrão para todos os emails recebidos. As cores, os planos de fundo, as imagens, etc., são ajustados automaticamente com as configurações do modo escuro específicas desse cliente de email. Nenhuma modificação externa é possível.

Esses clientes, por exemplo:

* Gmail (Webmail Para Desktop, iOS, Android, Webmail Para Dispositivos Móveis)
* Windows do Outlook
* Outlook Windows Mail

Nesse caso, se você definir configurações personalizadas do modo escuro no Designer de email, essas configurações serão substituídas pelas configurações do cliente de email.

Portanto, embora esses clientes de email lidem com o modo escuro, o design específico do modo escuro não será renderizado.

### Clientes que oferecem suporte ao modo escuro personalizado {#custom-support}

Outros clientes de email oferecem a opção de renderizar o modo escuro personalizado com a consulta `@media (prefers-color-scheme: dark)`, que é o método usado pelo Designer de Email [!DNL Marketo Engage].

Esta é uma lista dos principais clientes que lidam com essa opção:

* Apple Mail macOS
* Apple Mail iOS
* Outlook macOS
* Outlook.com
* Outlook iOS
* Outlook Android

Nesse caso, as configurações definidas no Designer de email devem ser exibidas.

>[!NOTE]
>
>Saiba como definir configurações personalizadas do modo escuro com o Email Designer em [esta seção](#define-custom-dark-mode).

No entanto, algumas restrições podem se aplicar de acordo com cada cliente de email. Por exemplo, alguns clientes, como o Apple Mail 16 (macOs 13), não gerarão o modo escuro se as imagens estiverem presentes.

Para obter os melhores resultados, teste seu conteúdo nos clientes de email que você está direcionando. Para ver uma simulação que se aproxime o máximo possível do resultado final para cada cliente, use o recurso [Renderização de email](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) no Designer de email.

## Modo escuro no designer de email {#dark-mode-email-designer}

Quando se trata do modo escuro no Designer de email, há dois aspectos a serem considerados:

* Você pode obter uma visualização de como o modo escuro padrão será renderizado na maioria dos clientes de email de suporte. [Saiba mais](#preview-dark-mode)

* Se quiser substituir as configurações padrão de clientes de email de suporte, defina as configurações personalizadas do modo escuro no email que você está editando. [Saiba mais](#define-custom-dark-mode)

### Visualizar modo escuro padrão {#preview-dark-mode}

Para acessar o modo escuro no Designer de email e pré-visualizar as configurações padrão do modo escuro, siga as etapas abaixo.

1. Na página inicial do Designer de Email, selecione a opção **[!UICONTROL Design do zero]**.

1. Adicione [estruturas e conteúdo](/help/marketo/product-docs/email-marketing/email-designer/email-authoring.md#add-structure-and-content) ao seu email.

1. No canto superior direito, habilite a opção **[!UICONTROL Modo escuro]**.

   CAPTURA DE TELA

1. A visualização padrão do modo escuro é exibida.

   CAPTURA DE TELA

Por padrão, a pré-visualização do modo escuro do Email Designer aplica o esquema de cor &quot;inversão de cor completa&quot; a todos os elementos, exceto imagens e ícones.

Isso significa que ele detecta áreas com elementos claros e escuros e os inverte, de modo que os planos de fundo claros se tornam escuros e o texto escuro se torna claro, enquanto os planos de fundo escuros se tornam claros e o texto claro se torna escuro.

>[!CAUTION]
>
>A renderização final pode variar de acordo com o cliente de email do recipient. Para ver uma simulação que se aproxime o máximo possível do resultado final de cada cliente de email, use a opção [Renderização de email](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).

### Definir modo escuro personalizado {#define-custom-dark-mode}

Depois de alternar para o **[!UICONTROL modo escuro]**, você pode optar por editar elementos de estilo específicos do seu conteúdo, que será exibido somente quando o modo escuro estiver habilitado no cliente de email do destinatário, desde que ele seja compatível com esse recurso.

>[!WARNING]
>
>A renderização final no modo escuro depende de cada cliente de email, portanto, os resultados podem variar de um para o outro. [Saiba mais](#guardrails)

Para utilizar o estilo de modo escuro personalizado do Email Designer, o Journey Optimizer usa a consulta CSS `@media (prefers-color-scheme: dark)`, que detecta se o cliente de email do usuário está definido como modo escuro e aplica o design de tema escuro definido no seu email.

Para definir configurações personalizadas do modo escuro, siga as etapas abaixo.

1. Alterne para a visualização do **[!UICONTROL Modo escuro]** no Designer de email. [Saiba como](#preview-dark-mode)

1. Edite quaisquer atributos de cor de estilo, como texto, planos de fundo, botão etc.

1. Não é possível alterar as cores das imagens e dos ícones, mas você pode definir ativos específicos somente para o modo escuro. Para fazer isso, selecione qualquer imagem. Alterne para o **[!UICONTROL modo escuro]** usando a opção dedicada no painel **[!UICONTROL Configurações]** e selecione um ativo diferente.

   CAPTURA DE TELA

1. A qualquer momento, você pode **[!UICONTROL Alternar para o modo de exibição ativo]** para verificar como o conteúdo pode ser renderizado em vários tamanhos de dispositivo. Nesta exibição, selecione o botão Modo escuro na parte superior da tela para visualizar a versão em modo escuro do seu conteúdo em diferentes dispositivos.

   CAPTURA DE TELA

   >[!CAUTION]
   >
   >A visualização em tempo real é uma visualização genérica criada para comparar a aparência da renderização em vários tamanhos de dispositivo. A renderização final pode variar de acordo com o cliente de email do recipient.

1. Quando estiver satisfeito com as alterações do modo escuro, clique em **[!UICONTROL Simular Conteúdo]**.

   ![](assets/dark-mode-simulate.png)

1. Selecione **[!UICONTROL Renderizar email]** e conecte-se à sua conta Litmus. Você pode ver a renderização final do modo escuro para vários clientes de email. Saiba mais sobre [Renderização de email](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md).

   >[!WARNING]
   >
   >Embora a simulação se aproxime da forma como os emails aparecerão no modo escuro, a renderização real pode ser diferente devido a variações nos provedores de serviços de email ou nas configurações no nível do dispositivo.

## Práticas recomendadas {#best-practices}

À medida que a adoção do modo escuro aumenta nos principais clientes de email, é essencial considerar como seus emails são renderizados em ambientes claros e escuros, esteja você usando o [modo escuro personalizado](#define-custom-dark-mode) ou não.

O modo escuro pode alterar cores, planos de fundo e imagens — às vezes substituindo as opções de design. Para garantir a consistência visual, a acessibilidade e a integridade da marca, siga as práticas recomendadas listadas abaixo.

**Otimize suas imagens e logotipos**

* Salve logotipos e ícones como PNGs com fundo transparente para evitar caixas brancas visíveis no modo escuro.

* Evite imagens com fundos brancos ou claros codificados.

* Se a transparência não for uma opção, coloque as imagens em um plano de fundo sólido no design para evitar inversões de cores estranhas.

**Veja seus planos de fundo**

* Verifique se há contraste suficiente entre o texto e as cores do plano de fundo para facilitar a leitura nos modos claro e escuro.

* Evite depender apenas das cores do plano de fundo para o conteúdo crítico. Alguns clientes substituem as cores do plano de fundo no modo escuro, portanto, verifique se as informações principais ainda estão visíveis.

**Criar conteúdo acessível no modo escuro**

* Use combinações de cores fáceis de distinguir para pessoas com daltonismo.

* Use uma paleta de tons médios para garantir o contraste em planos de fundo claros e escuros.

* Use combinações de cores acessíveis com alto contraste para melhorar a legibilidade e atender aos padrões das Diretrizes de acessibilidade de conteúdo da Web (WCAG). Use ferramentas como o Verificador de contraste do WebAIM para verificar o contraste de cores.

* Evite fontes finas, pois isso pode afetar a legibilidade. Se sua marca requer uma fonte fina, coloque-a em negrito no modo escuro.

* Ignorar branco puro em preto puro, pois pode causar tensão nos olhos e ser automaticamente invertido por alguns clientes de email.

* Fornecer estilo de fallback acessível se o modo escuro não for compatível.

**Testar seus emails no ambiente no modo escuro**

* Use a [visualização de modo escuro](#preview-dark-mode) do Email Designer, que usa esquemas de cores invertidas para detectar problemas antecipadamente.

* Use a opção [Renderização de email](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md) que usa o Litmus para simular seus designs nos principais clientes de email (Apple Mail, Gmail, Outlook) e ver como as cores e as imagens se comportam no modo escuro.
