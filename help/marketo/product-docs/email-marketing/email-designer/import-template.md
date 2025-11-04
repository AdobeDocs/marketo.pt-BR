---
solution: Marketo Engage
product: marketo
title: Importação de modelo
description: Saiba como importar seus modelos de email existentes do editor clássico para o novo Designer de email.
level: Beginner, Intermediate
feature: Email Designer
badge: Beta
hide: true
hidefromtoc: true
source-git-commit: 3923ddfdffc21b5afd196c413bcf0ea3e2b806f5
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 1%

---

# Importação de modelo {#template-import}

Importe facilmente seus modelos de email existentes do editor clássico para o novo Designer de email, preservando seus designs e acelerando a criação de modelos com estruturas familiares e reutilizáveis. Revise as [práticas recomendadas](#best-practices) e saiba mais sobre as [limitações e soluções](#limitations-and-remedies).

>[!NOTE]
>
>Os templates de email clássicos foram desenvolvidos com o HTML de estilo livre, portanto, esse importador nem sempre pode importar perfeitamente todos os componentes. Revise seus modelos importados para garantir que todas as seções sejam editáveis e mapeadas corretamente. Se uma área não for selecionável, recrie-a para obter melhores resultados.

## Importar um modelo {#import-a-template}

1. Vá para o **Design Studio**.

   ![](assets/import-template-1.png)

1. Clique em **Modelos de email** e selecione **Modelos de email (Novos)**.

   ![](assets/import-template-2.png)

1. Clique em **Criar Modelo**.

   ![](assets/import-template-3.png)

1. Insira um _Nome_ e (opcional) _Descrição_.

   ![](assets/import-template-4.png)

1. Clique na guia **Modelos do Marketo** e escolha entre os Modelos existentes criados no editor de email clássico.

   ![](assets/import-template-5.png)

   >[!NOTE]
   >
   >Somente modelos aprovados e modelos que foram compartilhados com o espaço de trabalho atual estão disponíveis para importação.

1. Clique em **Usar este modelo**.

   ![](assets/import-template-6.png)

1. O modelo importado é aberto no Designer de email.

1. Revise os componentes para uma conversão correta e faça os ajustes desejados usando o Designer. Quando estiver satisfeito com o modelo, aprove-o para uso em emails.

## Criar fragmentos {#create-fragments}

É uma boa ideia criar fragmentos de seções repetíveis para uso posterior.

1. Clique no botão **...Mais** acima e selecione **Salvar como fragmento**.

   ![](assets/import-template-7.png)

1. Selecione um componente ou uma estrutura e clique em **Criar**.

   ![](assets/import-template-8.png)

1. Insira um nome (e uma descrição opcional) e clique em **Salvar**.

   ![](assets/import-template-9.png)

## Práticas recomendadas {#best-practices}

* Os templates de email clássicos foram desenvolvidos com o HTML de estilo livre, portanto, esse importador nem sempre pode importar perfeitamente todos os componentes. Revise seus modelos importados para garantir que todas as seções sejam editáveis e mapeadas corretamente. Se uma área não for selecionável, recrie-a para obter melhores resultados.

* Após a importação, é possível salvar seções reutilizáveis como fragmentos e aprová-las para uso por autores de email. Aplique temas de marca para manter a consistência e a conformidade.

* Você pode continuar usando o script do Velocity e considerar a reimplementação de trechos mais antigos usando uma combinação de fragmentos e conteúdo condicional para melhorar a flexibilidade e o controle.

## Limitações e soluções {#limitations-and-remedies}

<table><thead>
  <tr>
    <th>Limitação</th>
    <th>Motivo</th>
    <th>Solução</th>
  </tr></thead>
<tbody>
  <tr>
    <td>As variáveis definidas no editor de email clássico não estão disponíveis no nível de email.</td>
    <td>As variáveis foram originalmente projetadas para simplificar a edição de email quando o editor ainda não oferecia os recursos do WYSIWYG. No Designer de email, os usuários podem obter flexibilidade semelhante por meio dos controles disponíveis. O importador mantém a estrutura e os componentes do seu modelo existente, ajudando você a recriá-lo com eficiência no Designer de email.</td>
    <td>Os usuários devem conseguir isso no Designer. <p>
    Para módulos do, é possível salvar diferentes segmentos como fragmentos. Os fragmentos aprovados estarão disponíveis para uso no nível do email.</td>
  </tr>
  <tr>
    <td>Se o HTML de origem contiver blocos aninhados, as camadas mais profundas não serão endereçáveis no Designer.</td>
    <td>O Designer de email não é compatível com comentários aninhados.</td>
    <td>Embora o Designer não permita a edição de estruturas aninhadas, ele deve ser renderizado com precisão. Certifique-se de testar o modelo primeiro.<p>
    Recrie a estrutura usando a Grade.</td>
  </tr>
  <tr>
    <td>Às vezes, os botões são importados como contêineres simples com texto interno.</td>
    <td>Alguns estilos de implementação que usam o HTML podem ser interpretados incorretamente durante a importação.</td>
    <td>Recrie o botão na Designer.</td>
  </tr>
  <tr>
    <td>Às vezes, os botões podem estar superdimensionados.</td>
    <td>Conflito entre o CSS do email do Marketo com outros elementos de nível inferior (<code>&lt;span&gt;</code>)</td>
    <td>Tente ajustar as margens e os preenchimentos do botão no Designer.</td>
  </tr>
  <tr>
    <td>Os marcadores não são suportados nativamente.</td>
    <td>O Designer de email não oferece marcadores no momento.</td>
    <td>Considere recriar marcadores usando técnicas alternativas.</td>
  </tr>
  <tr>
    <td>O alinhamento vertical é distorcido onde o conteúdo do contêiner não respeita o valor do atributo de valor.</td>
    <td><code>valign</code> não funciona dentro de contêineres definidos no modelo.</td>
    <td>Tente ajustar as margens e os preenchimentos do botão no Designer de email.</td>
  </tr>
  <tr>
    <td>Os tokens do Personalization (Meus tokens) no nível do modelo podem encontrar erros de validação.</td>
    <td>Os modelos de email não suportam tokens no nível do programa.</td>
    <td>Substitua-os por outros tipos de token dentro de modelos e substitua-os por Meus tokens dentro dos emails individuais.</td>
  </tr>
  <tr>
    <td>Os componentes do divisor podem não ser selecionáveis.</td>
    <td>Os componentes divisores não são abordados na versão.</td>
    <td>n/d</td>
  </tr>
  <tr>
    <td>Se o HTML original tiver estruturas mal formadas, elas provavelmente serão transferidas.</td>
    <td>Problemas com o HTML original.</td>
    <td>Os problemas precisariam ser corrigidos antes da importação.</td>
  </tr>
  <tr>
    <td>Para o conteúdo importado, o uso da pré-visualização de conteúdo não é um indicador confiável.</td>
    <td>A função de visualização do Designer não é compatível com o HTML personalizado.</td>
    <td>É recomendável testar seu email usando a opção <b>Enviar prova</b> na tela <i>Simular conteúdo</i>.</td>
  </tr>
  <tr>
    <td>Os trechos no modelo antigo não funcionarão no Designer de email.</td>
    <td>O Designer de email não é compatível com snippets.</td>
    <td>Recrie seus trechos como fragmentos combinados com conteúdo condicional.</td>
  </tr>
</tbody></table>
