---
solution: Marketo Engage
product: marketo engage
title: Editar imagens com o Adobe Express
description: Saiba como editar imagens no Editor de email do Adobe Marketo Engage usando o Adobe Express.
level: Beginner, Intermediate
hide: true
hidefromtoc: true
exl-id: 74623a14-8eaf-4f79-952c-d10092ddc34f
source-git-commit: a5fafa0fb218a366b6e2c9b3adfb785791b52447
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 1%

---

# Editar imagens com o Adobe Express {#edit-images-with-adobe-express}

O Adobe Marketo Engage se integra nativamente ao Adobe Express, fornecendo acesso a uma variedade de ferramentas de edição de imagens. Você pode usar essas ferramentas para modificar suas imagens no Marketo Engage Design Studio. A integração oferece os seguintes benefícios principais:

* Maior reutilização de conteúdo ao editar e salvar novas imagens no Marketo Engage.

* Tempo e esforço reduzidos na atualização de imagens ou criação de novas versões de imagens existentes.

>[!NOTE]
>
>No momento, o Adobe Express só oferece suporte aos formatos de arquivo de imagem PNG e JPEG.

## Acessar o editor do Adobe Express {#access-the-adobe-express-editor}

Há duas maneiras de acessar o editor do Adobe Express.

>[!BEGINTABS]

>[!TAB Clique no nome da imagem]

1. No Marketo Engage, vá para o **[!UICONTROL Design Studio]** e selecione **[!UICONTROL Imagens e Arquivos]**.

   ![Selecionando Imagens e Arquivos na navegação à esquerda do Design Studio](assets/edit-images-with-adobe-express-1a.png){width="600" zoomable="yes"}

1. Selecione a imagem que deseja editar (ou crie uma nova).

   CAPTURA DE TELA 2a

   >[!NOTE]
   >
   >* Para exibir os ativos por espaço de trabalho e pasta, abra a estrutura clicando no ícone **[!UICONTROL Mostrar pastas]** na parte superior esquerda.
   >
   >* Para classificar a tabela por qualquer uma das colunas, clique no título da coluna. A seta na linha de título indica a coluna e a ordem de classificação atuais.

1. Na guia da imagem _Detalhes_, clique em **[!UICONTROL Editar no Adobe Express]**.

   CAPTURA DE TELA 3a

   >[!CAUTION]
   >
   >Se a imagem já estiver referenciada em um email ou template de email, qualquer edição feita atualizará essa imagem em todos os lugares em que ela estiver sendo usada no momento.

>[!TAB Ações de imagem e arquivo]

1. No Marketo Engage, vá para o **[!UICONTROL Design Studio]** e selecione **[!UICONTROL Imagens e Arquivos]**.

   ![Selecionando Imagens e Arquivos na navegação à esquerda do Design Studio](assets/edit-images-with-adobe-express-1b.png){width="600" zoomable="yes"}

   >[!NOTE]
   >
   >* Para exibir os ativos por espaço de trabalho e pasta, abra a estrutura clicando no ícone **[!UICONTROL Mostrar pastas]** na parte superior esquerda.
   >
   >* Para classificar a tabela por qualquer uma das colunas, clique no título da coluna. A seta na linha de título indica a coluna e a ordem de classificação atuais.

1. Marque a caixa de seleção ao lado da imagem que deseja editar.

   CAPTURA DE TELA 2b

1. No menu suspenso **[!UICONTROL Ações de imagem e arquivo]**, selecione **[!UICONTROL Editar no Adobe Express]**.

   >[!CAUTION]
   >
   >Se a imagem já estiver referenciada em um email ou template de email, qualquer edição feita atualizará essa imagem em todos os lugares em que ela estiver sendo usada no momento.

>[!ENDTABS]

## Licença do Adobe Express Enterprise {#adobe-express-enterprise-license}

### Usuários com uma licença Enterprise {#users-with-an-enterprise-license}

Se você tiver uma licença Enterprise para o Adobe Express, terá acesso ao editor Express completo. Você pode ajustar as configurações da imagem como cor, brilho, nitidez, contraste, tamanho e muito mais. A opção Mágica de IA permite remover planos de fundo, inserir e remover objetos e apagar partes de uma imagem.

>[!IMPORTANT]
>
>A licença adquirida deve estar na mesma Organização IMS que a sua assinatura do Marketo Engage para acessar todos os recursos de edição do Adobe Express. Além disso, cada usuário individual deve ter uma licença no Adobe Express. Os usuários [sem uma licença](#users-without-an-enterprise-license) só podem acessar as ações rápidas no Adobe Express.

### Usuários sem uma licença Enterprise {#users-without-an-enterprise-license}

Para aqueles sem uma licença Enterprise, você ainda tem acesso a vários recursos de edição de ação rápida. Esses recursos são:

* [Redimensionar imagem](#resize-image)
* [Remover plano de fundo](#remove-background)
* [Cortar imagem](#crop-image)
* [Converter em PNG/JPEG](#convert-to-png-jpeg)

Os recursos podem ser acessados no lado superior esquerdo da página de imagem.

CAPTURA DE TELA

#### Redimensionar imagem {#resize-image}

1. Clique em **Redimensionar imagem**.

1. Faça as alterações desejadas e clique em **Aplicar** quando terminar.

CAPTURA DE TELA

<table><tbody>
  <tr>
    <td><b>Taxa de proporção</b></td>
    <td>No menu suspenso <b>Taxa de proporção</b>, escolha <b>Padrão</b> como EM BRANCO ou <b>Personalizado</b> para definir sua própria largura/altura.</td>
  </tr>
  <tr>
    <td><b>Largura e altura</b></td>
    <td>Por padrão, a taxa de proporção é bloqueada, mantendo as proporções da imagem iguais ao ajustar seu tamanho. Se desejar, é possível selecionar o botão de bloqueio para desbloquear a taxa de proporção.</td>
  </tr>
  <tr>
    <td><b>Redefinir</b></td>
    <td>Clique em <b>Redefinir</b> para remover todas as edições feitas na imagem e retorná-la ao seu estado original.</td>
  </tr>
  <tr>
    <td><b>Zoom e corte</b></td>
    <td>Clique em <b>Aplicar zoom e recortar</b> para aplicar zoom em áreas específicas da imagem.</td>
  </tr>
</tbody>
</table>

#### Remover plano de fundo {#remove-background}

1. Clique em **Remover Plano de Fundo**.

1. O Adobe Express exibe a imagem sem plano de fundo. Clique em **Aplicar**.

PIC

>[!TIP]
>
>Para restaurar o plano de fundo, selecione a imagem e selecione **Remover Plano de Fundo** novamente.

#### Cortar imagem {#crop-image}

1. Clique em Cortar imagem.

1. Arraste os cantos da imagem para criar o corte desejado.

CAPTURA DE TELA

1. Clique em **Aplicar** quando terminar.

#### Converter em PNG/JPEG {#convert-to-png-jpeg}

Converta um PNG em um JPEG ou um JPEG em um PNG.

1. Clique em **Converter em PNG/JPEG**.

1. Clique em **Aplicar**.

CORTAR MATERIAL ABAIXO

Clique em Cortar imagem na página.

No editor do Adobe Express, execute o corte na imagem e clique em Salvar.

Observação: essa ação não substituirá a imagem, mas a apresentará para outras edições.

Você pode fazer mais atualizações usando outra opção no painel esquerdo, clicar em Salvar para substituir a imagem existente ou Salvar como novo ativo para salvar como uma nova imagem.

Clique em Salvar para concluir a ação.

## Salve o trabalho {#save-your-work}

Quando terminar todas as edições, clique em Salvar para salvar o trabalho.

CAPTURA DE TELA

A imagem editada é salva na mesma pasta da imagem original.
