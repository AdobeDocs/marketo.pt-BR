---
description: A definir.
title: Visão geral do Halo
source-git-commit: a1efdaab40e02861b7ee9ceabeb004fdd6c5de57
workflow-type: tm+mt
source-wordcount: '1341'
ht-degree: 0%

---

# Criar e gerar campanhas de email {#build-and-generate-email-campaigns}

Criar e gerar campanhas de email

As seções marcadas como [FOR KEITH:] precisam de mais conteúdo específico do produto preenchido.\
Os espaços reservados para a captura de tela usam [SCREENSHOT: description] — extraia das capturas de tela já existentes no rascunho de origem ou capture novas do ambiente de avaliação.

Também note Keith, Eu usei &#39;Halo&#39; como um espaço reservado, mas este nome vai mudar com base na decisão da liderança.

Forma

[PARA KEITH: 1-2 frase de introdução que constrói confiança e orienta o leitor. Enquadramento sugerido: &quot;No final deste guia, você terá criado e revisado sua primeira campanha de email completa no Halo. Do início ao fim, leva aproximadamente [TIME ESTIMATE].&quot;]

Forma

Antes de começar

Verifique se você tem:

Uma conta Halo ativa (cadastre-se aqui se ainda não tiver feito isso).

Sua marca está configurada em Seus itens > Marcas. (Saiba mais)

(Opcional, mas recomendado) Um modelo de email do HTML carregado em Seus itens > Modelos de email.

Um CSV de público-alvo pronto para upload. (Baixe um CSV de público-alvo de amostra se precisar de um ponto de partida.)

Uma ideia clara do objetivo da campanha, por exemplo, &quot;conquistar clientes antigos&quot;, &quot;convidar usuários de avaliação para um webinário&quot;.

Dica: se você é novo em escrever prompts para campanhas de marketing, reserve dois minutos para comemorar o Prompting Halo — práticas recomendadas antes de começar. Vai afiar tudo o que se segue.
&lbrack;PARA KEITH: Vamos ter que criar este documento adicional, será baseado em uma combinação de:

1. Práticas de geração de conteúdo/prompts do AJO (seções aplicáveis:

Estrutura co-estrela

Fundamentos do prompt

Escrever objetivos eficazes

Deixar de lado o conteúdo específico)

&#x200B;2. Journey Agent (seções aplicáveis: seções DENTRO e fora do escopo, teremos que adicionar algo assim)

Forma

Etapa 1: iniciar um novo chat

Na home page, você tem três maneiras de começar:

Digite um prompt na barra de prompts central.

Escolha um template de campanha pré-configurado na seção de modelos abaixo da barra de prompts.

Use a opção &quot;help me prompt&quot; na lista suspensa na barra de prompts para que o Halo oriente você durante a escrita de seu prompt.

[CAPTURA DE TELA: Página inicial com barra de prompt, linha de modelo e opção de &quot;prompt do help me&quot; realçada]

[FOR KEITH: breve descrição de cada opção e quando usá-la. Recomende modelos para novatos, solicitações de forma livre para profissionais de marketing que sabem o que desejam e &quot;ajude-me a solicitar&quot; para qualquer pessoa entre eles.]

Forma

Etapa 2: Escreva o prompt

Um prompt Halo forte inclui:

O objetivo da campanha — o que você está tentando alcançar.

O público-alvo — para quem são ou de onde vêm os dados do público-alvo.

O formato e a estrutura — número de emails, cadência, tom.

Sinalizações de marca ou contexto — referências à sua marca, produto ou campanha.

Exemplo:

&quot;Crie uma série de emails de retorno para clientes que compraram no ano passado, mas não devolveram. Use o CSV que foi carregado. Inclua de 2 a 3 emails que pareçam sazonais e lembre-os de fazer compras novamente.&quot;

[FOR KEITH: pode adicionar mais 2-3 exemplos de prompt abrangendo B2B e B2C para fornecer variedade. Extraia os Casos de uso do nosso documento de coleção para fins de consistência.]

[CAPTURA DE TELA: Barra de seleção com exemplo de prompt digitado em]

Forma

Etapa 3: Fazer upload do público

[FOR KEITH: Apresentação do carregamento do CSV. Capa: - Onde o botão de upload está na interface. - Colunas necessárias e expectativas de formato. - Campos de personalização que o Halo pode usar (nome, data do último pedido, categoria do produto etc.). - Link para CSV de amostra. - O que acontece se os dados estiverem confusos ou se os campos estiverem ausentes.]

[CAPTURA DE TELA: Fluxo de carregamento CSV]

Dica: exclua todos os contatos para os quais você não deseja enviar um email — usuários que cancelaram sua inscrição, endereços internos, contas de teste — antes de fazer upload. Embora progressivamente possamos habilitar a funcionalidade para &#39;excluir&#39; usuários específicos ou &#39;adicionar atributos&#39; durante o curso da avaliação, ela não estará disponível imediatamente a partir da data de lançamento.

Forma

Etapa 4: adicionar um resumo e materiais de referência

&lbrack;PARA KEITH: Explique como anexar documentos de referência de marca breves ou outro contexto. Capa: - Tipos de arquivo compatíveis. - Como o Halo usa essas informações (extraídas para o contexto do prompt, aplicadas à geração de conteúdo etc.). - Limites de tamanho de arquivo, se houver

Aqui está um mergulho profundo da minha sessão no summit no qual abordo isso: https://business.adobe.com/br/summit/2026/sessions/3-2-1-launch-project-halo-revealed-s232.html\
Limitações - Eu posso conectá-lo com o engg - Neha Pullabhotla, que será capaz de nos ajudar sobre as especificidades aqui. &rbrack;

[CAPTURA DE TELA: interface do anexo de resumo/referência]

Forma

Etapa 5: gerar a campanha

Clique em &quot;Gerar campanha&quot;. O Halo irá:

Gerar um plano de campanha estruturado

Pergunte pelo seu público-alvo - que também será usado para personalização de conteúdo

Conteúdo de email personalizado de rascunho para cada etapa.

Criar dinamicamente a jornada ao longo do caminho

Reúna tudo em um único quadro de campanha.

[FOR KEITH: descrição da aparência do quadro de campanha e do que ele contém. Cubra a exibição de plano, de jornada e de conteúdo. Observe quanto tempo a geração pode normalmente levar - o que depende do número de pontos de contato em sua jornada. Quando abrirem um editor para o fluxo de trabalho ou para o email, a conversa será exibida para que fiquem no contexto do componente específico, como o editor de email é um editor de email de apontar e clicar com a limitação de que não se destina a ser um designer completo, os usuários podem editar imagens no Adobe Express ou até mesmo se conectar ao Google Drive ou AEM Assets usando o Adobe Express. Todos os ativos de imagem são armazenados no Express, eles geram novamente as imagens no editor de email com o Firefly em linha ou as substituem por uma imagem local do computador. Eles podem trocar o modelo do HTML, regenerar o conteúdo e, finalmente, enviar a si mesmos o &quot;Email de teste&quot; para validar o que o cliente final receberá]

[CAPTURA DE TELA: quadro de campanha gerado com plano, jornada e conteúdo visíveis]

Forma

Etapa 6: revisar e refinar

É aqui que a interface conversacional de Halo ganha seu sustento. Para fazer alterações, entre em contato com o Halo:

&quot;Tornar a linha de assunto do email 2 mais urgente.&quot;

&quot;Diminua a cópia do corpo em todos os e-mails.&quot;

&quot;Troque o público-alvo para clientes somente da região Oeste.&quot;

&quot;Adicione um quarto email com uma CTA mais forte.&quot;

&quot;Alterar a espera de 3 dias para 5 dias&quot;

[FOR KEITH: aborde como fazer alterações via chat e edição direta. Explicar como os artefatos são atualizados no local. Não mencione a capacidade de adicionar mais nós ao workflow por meio do editor, nem o controle de versão existe no momento. Para obter melhores resultados, também recomendamos que solicitem quaisquer alterações em seu fluxo de trabalho geral logo no início, quando seu plano for criado]

[CAPTURA DE TELA: Refinamento de conversa em ação — mostrar um email antes e depois de uma solicitação de chat]

Forma

Etapa 7: enviar um email de prova

Antes de iniciar, envie a campanha para você mesmo ou para um membro de sua equipe para analisar em uma caixa de entrada real.

[FOR KEITH: etapas para enviar uma prova. Capa: - Onde está o botão de prova. - Quem pode receber provas (atualmente, apenas o usuário conectado) - Se todos os emails na jornada são enviados ou apenas um de cada vez (atualmente, apenas 1 de cada vez, a menos que o usuário diga &quot;prova desta série&quot; no chat. - O que verificar na prova (renderização, links, tokens de personalização, rodapé de cancelamento de inscrição).]

[CAPTURA DE TELA: enviar fluxo de prova]

Forma

Etapa 8: iniciar ou exportar

Quando estiver satisfeito com a campanha, você terá algumas opções:

Inicie a campanha. (Não está disponível no momento com nosso lançamento, mas será ativado dentro de 2 semanas de nosso primeiro lançamento, aguardando liberação legal)

Exportar emails individuais como HTML.

Exporte a campanha completa como um documento do Word ou PDF para análise da equipe.

[FOR KEITH: Detalhes sobre cada opção e todas as verificações de pré-inicialização executadas pelo Halo (conformidade, links corrompidos, campos de personalização ausentes etc.).]

[CAPTURA DE TELA: opções de inicialização/exportação]

Forma

Perguntas comuns

&lbrack;PARA KEITH: 4-6 FAQs baseadas no feedback inicial do usuário. Iniciantes sugeridos - para discutir com nossa equipe engajada:
- &quot;Por que a primeira resposta demora tanto?
- &quot;E se a saída de Halo não estiver correta?&quot;
- &quot;Posso editar e-mails diretamente ou apenas via chat?&quot;
- &quot;Como salvar uma campanha sem lançá-la?&quot;
- &quot;E se o CSV do meu público-alvo tiver erros?&quot;
- &quot;Posso duplicar ou remixar uma campanha?&quot;
- &quot;Como faço para compartilhar um rascunho de campanha com um colega de equipe para análise?&quot;&rbrack;

Forma

Próximas etapas

Casos de uso de nossa coleção — Navegue por exemplos de prompts reais para remixar para suas próprias campanhas.

Introdução ao Halo — Retorne à visão geral.

Solicitação do Halo — práticas recomendadas (em breve)
