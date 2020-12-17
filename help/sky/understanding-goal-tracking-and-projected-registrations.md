---
title: entendimento-objetivo-rastreamento-e-projetado-registros
description: Compreensão do rastreamento de metas e registros projetados
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---


# Compreensão do rastreamento de metas e registros projetados

<br> 

Depois de [definir objetivos de evento](/help/sky/setting-event-goals.md) e enviar convites por meio de uma [campanha inteligente](/help/sky/create-a-smart-campaign.md), veja como rastrear o progresso de sua meta e entender as previsões de Marketo.

>[!NOTE]
>
>Quando um programa de evento é criado na experiência do Marketo Classic, a data do start de evento assume o padrão da data de criação do evento. Uma vez que os registros projetados têm em conta a quantidade de tempo antes da data do start, esses números podem não ser exatos se a data do start e a data de criação forem as mesmas (a menos que sejam definidos intencionalmente).

## Rastreamento de metas e registros projetados

1. Você pode encontrar detalhes de rastreamento de meta na guia **[!UICONTROL Relatórios]** do programa do evento. Neste exemplo em particular, há 150 membros registrados até agora contra uma meta de 200 (75%).

   ![Imagem Um](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-1.png)

Você também verá seus registros **[!UICONTROL Projetados]**. Passe o mouse sobre o ícone de informações para ver um detalhamento desse número por segmento de Probabilidade.

![Imagem dois](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-2.png)

>[!NOTE]
>
>O gráfico Participantes e Superior permanecerá vazio até o dia do evento.

1. Clique na alternância de Gráfico para alternar para um detalhamento de seus membros por probabilidade de registro. Você verá as porcentagens de registro atuais para cada segmento, em comparação à porcentagem média para esse segmento em seus programas anteriores.

   ![Imagem Três](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-3.png)

Todos os membros (registrados e ainda não registrados) são classificados com base na probabilidade de registro. Passe o mouse sobre o ícone de informações para ver como essas categorias de probabilidade são definidas.

![Imagem quatro](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-4.png)

>[!NOTE]
>
>Os números de previsão são atualizados a cada 24 horas até o dia do evento. Todos os membros listados como _Processando_ serão incluídos no próximo ciclo de cálculo.

## Programas semelhantes

Você pode obter algum insight sobre o seu evento atual, observando o desempenho de programas similares no passado. Esta seção mostra até 5 programas semelhantes dos últimos 6 meses, com o número/porcentagem de membros que foram _Registrados_ ou superiores.

Ao calcular programas semelhantes, incluímos os seguintes fatores, entre outros:

* Tipo de programa
* Canal programa
* tamanho da audiência
* Tags de programa
* Duração do tempo da criação do evento ao start do evento
* duração do evento

   ![Imagem cinco](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-5.png)

## Recommendations

Na parte superior da página Relatórios, você pode encontrar recomendações orientadas por AI/ML com base no seu progresso. Verifique periodicamente se há dicas e insights úteis!

![Imagem seis](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-6.png)

## previsões de nível de pessoa

Clique na guia **[!UICONTROL Members]** para visualização de todos os membros do programa. Passe o cursor do mouse sobre as barras **[!UICONTROL Probabilidade de registro]** ou **[!UICONTROL Probabilidade de participação]** para ver as percentagens exatas e as categorizações. Em seguida, você pode agir com os membros em uma categoria específica (por exemplo, todos na categoria &quot;Menos provável&quot; para registrar a categoria) e especificamente público alvo-os para aumentar seus números de registro.

![Imagem sete](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-7.png)

>[!NOTE]
>
>A probabilidade individual leva em conta mais de 40 fatores pessoais, incluindo atributos de perfil, atividade pessoal e atividades convidadas/registradas/presentes.

## Perguntas frequentes

**P: Qual é o segmento?**

A: Provavelmente registrar é um valor de 0 a 100. Cada pessoa que é membro do programa do evento terá um valor de probabilidade entre 0-100.

Colocamos valores de probabilidade em três segmentos:

* Probabilidade de registrar > 50% = segmento altamente provável
* Probabilidade de registrar > 25% a &lt;50% = Segmento provável
* Probabilidade de registrar &lt;25% = Segmento menos provável

Quando uma pessoa tem probabilidade de se registrar, a previsão cairá em um desses segmentos (cada pessoa que é membro de um programa cairá em um deles). Por exemplo, se um programa de eventos tiver 1000 membros com base nas previsões de probabilidade, esses 1000 serão distribuídos nos segmentos _Highly Probely_, _Provavelmente_ ou _Menos Provável_.

Portanto, as pessoas que caírem no segmento Altamente Provável terão maiores chances de se inscrever no evento.

Conversão para registrar = # de pessoas no segmento registrado dividido pelo número de pessoas que se encaixam no segmento (por exemplo, se 100 pessoas se encaixarem no segmento Altamente provável e 60 delas se inscreverem, a taxa de conversão será de 60%).

A % de conversão para registro seguirá este padrão: Altamente provável > Provável > Menos provável.

**P: Como usar os insights?**

A: As melhores práticas implicam o seguinte:

i. Você cria um programa e, em seguida, uma Campanha inteligente usa filtros preditivos com &quot;maior que X&quot;, o que resultaria em uma certa quantidade de pessoas (digamos 1000) e você executa a campanha.

ii. Após 24 horas, na guia [!UICONTROL Relatórios], é possível ver os registros projetados que são calculados com base na probabilidade de registrar valores de todas as pessoas que estão atualmente convidadas.

iii. Se os registros projetados forem menores que a meta, você precisará convidar mais pessoas. Neste ponto, você pode ver os insights que nos dizem qual era o limiar que funcionava em programas passados.

![Imagem Oito](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-8.png)

iv. Você pode criar uma nova Campanha inteligente com esse limite para convidar mais pessoas.

v. A qualquer momento, se você quiser entender por que um número projetado está sendo exibido, é possível alternar para ver a distribuição da audiência nos segmentos, suas taxas de conversão do passado e aplicar essas taxas de conversão à audiência atual (veja a captura de tela abaixo).

**P: O que é o gráfico Segmentos por registro?**

A: Três barras, cada uma representando um segmento (Altamente provável, provável, menos provável).

**Linha pontilhada violeta:taxa** média de conversação para registro nesse segmento, com base em programas similares passados.

**Barra azul:porcentagem** de registro de todas as pessoas nesse segmento.

![Imagem Nove](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-9.png)

Por exemplo, digamos que 100 pessoas têm probabilidade de se registrar > 50% e 60 dessas 100 pessoas registradas. Muito provavelmente tem 60% de conversão. Assim, todos os membros adicionados ao programa têm probabilidade de registrar valores, são colocados em segmentos e de acordo com o número de pessoas registradas em cada taxa de conversão de segmento é calculado.

**P: O que significa &quot;Registrado e Superior&quot;?**

A: Qualquer pessoa que esteja listada como registrada, ou qualquer outro status com um número de etapa igual ou superior.

Você pode criar novos status de progressão para um programa de evento, mas mapeamos esses status com status padrão. Considere um caso em que uma pessoa é transferida do convidado para o lembrado, o que é uma etapa mais alta do que o registro. Essa pessoa também será considerada como registrada e mostrada no rastreamento de meta.

![Imagem Dez](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-10.png)

**P: Como são calculados os registros projetados?**

A: Consulte abaixo.

![Imagem Onze](/help/sky/assets/predictive-audiences/understanding-goal-tracking-and-projected-registrations/understanding-goal-tracking-and-projected-registrations-11.png)
