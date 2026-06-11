---
description: Um guia passo a passo para criar uma campanha de e-mail no CX Enterprise Co-worker, desde escrever prompts até revisar e exportar sua campanha.
title: Criar e gerar campanhas de email
source-git-commit: e72cf50e03dcf225a47872dc5ade976d46445c86
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 0%

---

# Criar e gerar campanhas de email {#build-and-generate-email-campaigns}

Saiba como criar e revisar campanhas de email completas em minutos.

## Antes de começar

Verifique se você tem:

* Uma conta ativa do CX Enterprise Co-worker ([inscreva-se aqui](https://coworker-essentials.experience.adobe.com/) se você ainda não tiver uma).

* Sua marca foi configurada em **Seus itens** > **Marcas**.

* (Opcional, mas recomendado) Um modelo de email do HTML carregado em **Seus itens** > **Modelos de email**.

* Um CSV de público-alvo pronto para upload.

* Uma ideia clara do objetivo da campanha (por exemplo, &quot;conquistar clientes antigos&quot;, &quot;convidar usuários de avaliação para um webinário&quot;).

>[!TIP]
>
>Se você nunca escreveu prompts para campanhas de marketing, reserve dois minutos para ignorar _Solicitação do CX Enterprise Co-worker: práticas recomendadas_ antes de começar.

## Etapa 1: iniciar um novo chat

Na home page, você tem três maneiras de começar:

* Digite um prompt na barra de prompts central.
* Escolha um template de campanha pronto na seção de modelos abaixo da barra de prompts.
* Use a opção &quot;help me prompt&quot; na lista suspensa na barra de prompts para que o CX Enterprise Coworker o oriente durante a escrita de seu prompt.

[CAPTURA DE TELA: Página inicial com barra de prompt, linha de modelo e opção de &quot;prompt do help me&quot; realçada]

![](assets/generate-email-campaigns-.png)

[FOR KEITH: breve descrição de cada opção e quando usá-la. Recomende modelos para novatos, solicitações de forma livre para profissionais de marketing que sabem o que desejam e &quot;ajude-me a solicitar&quot; para qualquer pessoa entre eles.]

## Etapa 2: Escreva o prompt

Um forte prompt do CX Enterprise Co-worker inclui:

* A meta da campanha (o que você está tentando alcançar).
* O público-alvo (para quem são ou de onde vêm os dados do público-alvo).
* O formato e a estrutura (número de emails, cadência, tom).
* Sinalizações de marca ou contexto (referências à sua marca, produto ou campanha).

Exemplo:

```
"Create a win-back email series for customers who bought last year but haven't returned. Use the CSV I uploaded. Include 2–3 emails that feel seasonal and remind them to shop again."
```

[FOR KEITH: pode adicionar mais 2-3 exemplos de prompt abrangendo B2B e B2C para fornecer variedade. Extraia os Casos de uso do nosso documento de coleção para fins de consistência.]

[CAPTURA DE TELA: Barra de seleção com exemplo de prompt digitado em]

![](assets/generate-email-campaigns-.png)

## Etapa 3: Fazer upload do público

[FOR KEITH: Apresentação do carregamento do CSV. Capa: - Onde o botão de upload está na interface. - Colunas necessárias e expectativas de formato. - Campos de personalização que o CX Enterprise Co-worker pode usar (nome, data do último pedido, categoria do produto etc.). - Link para CSV de amostra. - O que acontece se os dados estiverem confusos ou se os campos estiverem ausentes.]

[CAPTURA DE TELA: Fluxo de carregamento CSV]

![](assets/generate-email-campaigns-.png)

>[!TIP]
>
>Exclua todos os contatos para os quais você não deseja enviar um email (usuários que cancelaram a inscrição, endereços internos, contas de teste) antes de fazer upload. Embora progressivamente possamos habilitar a funcionalidade para &#39;excluir&#39; usuários específicos ou &#39;adicionar atributos&#39; durante o curso da avaliação, ela não estará disponível imediatamente a partir da data de lançamento.

## Etapa 4: adicionar um resumo e materiais de referência

&lbrack;PARA KEITH: Explique como anexar documentos de referência de marca breves ou outro contexto. Capa: - Tipos de arquivo compatíveis. - Como o CX Enterprise Co-Worker usa essas informações (extraídas para o contexto do prompt, aplicadas à geração de conteúdo etc.). - Limites de tamanho de arquivo, se houver

Aqui está um mergulho profundo da minha sessão no summit no qual abordo isso: https://business.adobe.com/br/summit/2026/sessions/3-2-1-launch-project-halo-revealed-s232.html\
Limitações - Eu posso conectá-lo com o engg - Neha Pullabhotla, que será capaz de nos ajudar sobre as especificidades aqui. &rbrack;

[CAPTURA DE TELA: interface do anexo de resumo/referência]

![](assets/generate-email-campaigns-.png)

## Etapa 5: gerar a campanha

Clique em **Gerar campanha**. O CX Enterprise Co-worker irá:

* Gerar um plano de campanha estruturado.
* Pergunte pelo seu público-alvo, que também será usado para personalização de conteúdo.
* Conteúdo de email personalizado de rascunho para cada etapa.
* Crie dinamicamente a jornada ao longo do caminho.
* Reúna tudo em um único quadro de campanha.

[FOR KEITH: descrição da aparência do quadro de campanha e do que ele contém. Cubra a exibição de plano, de jornada e de conteúdo. Observe quanto tempo a geração pode normalmente levar - o que depende do número de pontos de contato em sua jornada. Quando abrirem um editor para o fluxo de trabalho ou para o email, a conversa será exibida para que fiquem no contexto do componente específico, como o editor de email é um editor de email de apontar e clicar com a limitação de que não se destina a ser um designer completo, os usuários podem editar imagens no Adobe Express ou até mesmo se conectar ao Google Drive ou AEM Assets usando o Adobe Express. Todos os ativos de imagem são armazenados no Express, eles geram novamente as imagens no editor de email com o Firefly em linha ou as substituem por uma imagem local do computador. Eles podem trocar o modelo do HTML, regenerar o conteúdo e, finalmente, enviar a si mesmos o &quot;Email de teste&quot; para validar o que o cliente final receberá]

[CAPTURA DE TELA: quadro de campanha gerado com plano, jornada e conteúdo visíveis]

![](assets/generate-email-campaigns-.png)

## Etapa 6: revisar e refinar

A interface conversacional torna o refinamento simples. Para fazer alterações, entre em contato com o CX Enterprise Co-worker:

* &quot;Tornar a linha de assunto do email 2 mais urgente.&quot;
* &quot;Diminua a cópia do corpo em todos os e-mails.&quot;
* &quot;Troque o público-alvo para clientes somente da região Oeste.&quot;
* &quot;Adicione um quarto email com uma CTA mais forte.&quot;
* &quot;Altere a espera de 3 dias para 5 dias.&quot;

[FOR KEITH: aborde como fazer alterações via chat e edição direta. Explicar como os artefatos são atualizados no local. Não mencione a capacidade de adicionar mais nós ao workflow por meio do editor, nem o controle de versão existe no momento. Para obter melhores resultados, também recomendamos que solicitem quaisquer alterações em seu fluxo de trabalho geral logo no início, quando seu plano for criado]

[CAPTURA DE TELA: Refinamento de conversa em ação — mostrar um email antes e depois de uma solicitação de chat]

![](assets/generate-email-campaigns-.png)

## Etapa 7: enviar um email de prova

Antes de iniciar, envie a campanha para você mesmo ou para um membro de sua equipe para analisar em uma caixa de entrada real.

[FOR KEITH: etapas para enviar uma prova. Capa: - Onde está o botão de prova. - Quem pode receber provas (atualmente, apenas o usuário conectado) - Se todos os emails na jornada são enviados ou apenas um de cada vez (atualmente, apenas 1 de cada vez, a menos que o usuário diga &quot;prova desta série&quot; no chat. - O que verificar na prova (renderização, links, tokens de personalização, rodapé de cancelamento de inscrição).]

[CAPTURA DE TELA: enviar fluxo de prova]

![](assets/generate-email-campaigns-.png)

## Etapa 8: iniciar ou exportar

Quando estiver satisfeito com a campanha, você terá algumas opções:

>[!AVAILABILITY]
>
>O Launch não está disponível na versão inicial, mas está planejado para ser ativado até o final de junho. Verifique aqui se há atualizações.

* Inicie a campanha.
* Exportar emails individuais como HTML.
* Exporte a campanha completa como um documento do Word ou PDF para análise da equipe.

[FOR KEITH: Detalhes sobre cada opção e todas as verificações de pré-lançamento que o CX Enterprise Co-worker executa (conformidade, links com falha, campos de personalização ausentes etc.).]

[CAPTURA DE TELA: opções de inicialização/exportação]

![](assets/generate-email-campaigns-.png)

## Perguntas comuns

&lbrack;PARA KEITH: 4-6 FAQs baseadas no feedback inicial do usuário. Iniciantes sugeridos - para discutir com nossa equipe de inglês:
* &quot;Por que a primeira resposta demora tanto?
* &quot;E se o resultado do CX Enterprise Co-worker não estiver certo?&quot;
* &quot;Posso editar e-mails diretamente ou apenas via chat?&quot;
* &quot;Como salvar uma campanha sem lançá-la?&quot;
* &quot;E se o CSV do meu público-alvo tiver erros?&quot;
* &quot;Posso duplicar ou remixar uma campanha?&quot;
* &quot;Como faço para compartilhar um rascunho de campanha com um colega de equipe para análise?&quot;&rbrack;
