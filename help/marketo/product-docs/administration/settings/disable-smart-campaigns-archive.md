---
description: Saiba como ativar o recurso Desativar campanhas inteligentes no arquivo, que desativa campanhas automaticamente quando uma pasta ou programa é arquivado no Marketo.
title: Desativar campanhas inteligentes no arquivo
feature: Administration
hide: true
source-git-commit: 526d10bb96e059d251a76ca720ff81ab42ee9516
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Desativar campanhas inteligentes no arquivo {#disable-smart-campaigns-on-archive}

Quando esse recurso está ativado, o arquivamento de uma pasta ou programa desativa automaticamente suas campanhas para evitar atividades inesperadas.

Quando uma pasta ou programa é arquivado ou uma Campanha inteligente ativa é movida para uma pasta que já está arquivada, o Marketo Engage impede a execução das campanhas afetadas:

* **Campanhas acionadas** estão desativadas.
* **Campanhas em lote** têm suas execuções pendentes canceladas.
* **Campanhas executáveis** não têm estado de execução, portanto, nenhuma ação foi tomada.

## Como ativar {#how-to-enable}

1. Na seção **Admin**, clique em **Treasure Chest**.

   ![O menu de navegação do Administrador com Treasure Chest realçado](assets/disable-smart-campaigns-on-archive-1.png)

1. Role para _Desabilitar Campanhas inteligentes no Arquivo_ e clique em **Editar**.

   ![Página de configurações do Treasure Chest mostrando a linha Desativar Campanhas Inteligentes no Arquivo com o botão Editar](assets/disable-smart-campaigns-on-archive-2.png)

1. Marque a caixa de seleção **Habilitado** e clique em **Salvar**.

   ![A caixa de diálogo Desabilitar Campanhas Inteligentes no Arquivo Morto mostrando a caixa de seleção Habilitado e o botão Salvar](assets/disable-smart-campaigns-on-archive-3.png)

<table>
  <tr>
    <td><b>Ativado (marcado)</b></td>
    <td>O arquivamento desativa cada campanha, de acordo com as regras acima.</td>
  </tr>
  <tr>
    <td><b>Desativado (desmarcado)</b></td>
    <td>O arquivamento de uma pasta ou programa ainda funciona, mas as campanhas permanecem em execução ou programadas como estão.</td>
  </tr>
</table>

>[!IMPORTANT]
>
>Depois de alternar essa configuração, você deve atualizar o navegador para que a alteração entre em vigor.

## Ações suportadas

As ações a seguir desativam campanhas quando _Desabilitar Campanhas Inteligentes no Arquivo_ está habilitado:

* Arrastando e soltando uma **pasta** contendo campanhas ativas em uma pasta arquivada
* Arrastando e soltando um **programa** (qualquer tipo) contendo campanhas ativas em uma pasta arquivada
* Arrastando e soltando uma **única Campanha Inteligente** em uma pasta arquivada
* Clicar com o botão direito do mouse em **Mover** de uma única Campanha Inteligente para uma pasta arquivada
* Clicando com o botão direito do mouse em **Mover Pasta** em uma pasta que contém campanhas ativas para uma pasta arquivada
* Clicar com o botão direito do mouse em **Mover** em um programa que contém campanhas ativas para uma pasta arquivada
* Clicar com o botão direito do mouse em **Converter em Pasta Arquivada** em uma pasta para arquivá-la no local sem movê-la

>[!NOTE]
>
>Se uma Campanha inteligente dentro da pasta ou do programa que está sendo arquivado for referenciada em outro lugar (por exemplo, por meio de uma etapa de fluxo &quot;Solicitar campanha&quot;), o arquivamento será bloqueado para evitar a interrupção dessa outra campanha.
