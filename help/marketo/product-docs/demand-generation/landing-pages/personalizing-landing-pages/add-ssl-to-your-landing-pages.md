---
unique-page-id: 2359828
description: Adicionar SSL às suas páginas de aterrissagem - Documentação do Marketo - Documentação do produto
title: Adicionar SSL às suas landing pages
exl-id: 8271d9fe-0575-430c-97c7-407e4b78cf1d
feature: Landing Pages
source-git-commit: fddc2f24d9a66146f567c762305ab2825c2f29ae
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 1%

---

# Adicionar SSL às suas landing pages {#add-ssl-to-your-landing-pages}

A criptografia SSL (Secure Socket Layer) permite proteger todas as suas Landing Pages para uma instância do Marketo Engage.

Por padrão, ao preencher um formulário da Web ou visitar uma landing page hospedada pela Marketo Engage, as informações são enviadas por protocolo não seguro (HTTP). De acordo com a política da empresa, talvez você queira proteger as informações enviadas à Marketo no (HTTPS). Por exemplo, quando você visitar `http://info.mydomain.com/`, agora será `https://info.mydomain.com/`.

O Marketo Engage rastreia &quot;Página da Web visitada&quot; e &quot;Clique no link na página da Web&quot; por padrão por protocolo HTTP não seguro. Para ter os links de rastreamento protegidos com seu próprio certificado, o Marketo precisa criar um servidor não compartilhado separado para habilitá-lo. Proteger todos os aspectos da interação de um contato com você normalmente significa proteger tanto as páginas de aterrissagem quanto os links de rastreamento.

## Habilitar certificação SSL {#enable-ssl-certification}

Adicione SSL automaticamente para todos os aliases de domínio criados como parte das regras de página inicial.

1. Vá para a área **Administrador**.

   ![](assets/add-ssl-to-your-landing-pages-1.png)

1. Selecione **Páginas de aterrissagem** na árvore. Na guia **Regras**, clique no menu suspenso **Novo** e selecione **Novo Alias de Domínio**.

   ![](assets/add-ssl-to-your-landing-pages-2.png)

1. Insira seu _Alias de Domínio_ e _Página Padrão_. Marque a caixa de seleção **Gerar certificado SSL**. Clique em **Criar** quando terminar.

   ![](assets/add-ssl-to-your-landing-pages-3.png)

Isso adiciona automaticamente um certificado SSL a esse domínio.

## Habilitar SSL para o domínio padrão {#enable-ssl-default-domain}

Siga as etapas abaixo para ativar o SSL para seu domínio padrão.

1. Ainda na seção **Admin**, selecione **Landing Pages**. Clique no botão laranja **Editar** ao lado de _Configurações_.

   ![](assets/add-ssl-to-your-landing-pages-4.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Se desejar, também é possível modificar o nome do domínio aqui (é necessário um domínio válido).

1. Marque a caixa de seleção &quot;Gerar certificado SSL&quot; e clique em Salvar.

   ![](assets/add-ssl-to-your-landing-pages-5.png)

>[!NOTE]
>
>* A coluna Certificado SSL na lista mostra o status de certificado de todos os aliases de domínio criados após o lançamento desse recurso (25 de abril de 2025). Se o SSL estiver habilitado para um domínio por meio do Suporte da Marketo, o certificado continuará a existir, mas não aparecerá na tabela. Essa tabela reflete somente os certificados SSL para domínios adicionados usando as etapas deste artigo.
>
>* Pode levar até três minutos para que o SSL esteja no estado PRONTO. Você deve atualizar a página para que as alterações sejam exibidas.

## Mensagens de erro {#error-messages}

Abaixo você encontrará mensagens de erro que poderá receber junto com suas definições.

<table><thead>
  <tr>
    <th>Erro</th>
    <th>Detalhes</th>
  </tr></thead>
<tbody>
  <tr>
    <td><i>Erro inesperado encontrado ao criar um domínio. Entre em contato com o Suporte para obter assistência.</i></td>
    <td>Ocorreu um erro inesperado. Colete registros e detalhes de erros e encaminhe o problema para o suporte.</td>
  </tr>
  <tr>
    <td><i>O domínio padrão não foi encontrado. Entre em contato com o Suporte para obter assistência.</i></td>
    <td>Ocorreu um problema ao tentar localizar o domínio padrão. Entre em contato com o Suporte para que possam investigar.</td>
  </tr>
  <tr>
    <td><i>O certificado SSL já foi emitido.</i></td>
    <td>Já existe um certificado SSL para este domínio personalizado. Nenhuma ação adicional é necessária, a menos que o certificado tenha expirado ou precise ser reemitido.</td>
  </tr>
  <tr>
    <td><i>O domínio não está mapeado para o domínio padrão.</i></td>
    <td>O domínio personalizado não está mapeado corretamente para o domínio padrão. Verifique as configurações de mapeamento de domínio e certifique-se de que a configuração DNS aponte para o domínio padrão correto.</td>
  </tr>
  <tr>
    <td><i>O domínio já existe.</i></td>
    <td>Já existe um domínio com o mesmo nome.</td>
  </tr>
  <tr>
    <td><i>Uma configuração de IP único é necessária antes de adicionar mais domínios. Entre em contato com o Suporte para concluir a configuração e tentar adicionar outro domínio novamente.</i></td>
    <td>O primeiro domínio personalizado após o domínio padrão precisa de uma configuração única para ser iniciada por você. Crie um tíquete de Suporte para concluir a configuração e adicione o domínio depois que terminar.</td>
  </tr>
</tbody></table>

## Itens a Observar {#things-to-note}

* **Mapeamento de DNS para o domínio para o Marketo Engage**: antes de adicionar domínios na interface do usuário, você deve [mapear CNAMEs para um domínio fornecido pelo Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **SSLs personalizados**: se você precisar de um SSL personalizado, envie um [Tíquete de suporte](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Não use a caixa de seleção de autoatendimento para criação de SSL.

* **SSLs pré-existentes**: ao adicionar um domínio, o sistema verifica se há SSLs pré-existentes, que podem ter sido criados manualmente antes. Se encontrar essa validação, crie seu domínio sem selecionar a criação de SSL e nós os conectaremos para você. [Contate o Suporte](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para obter mais detalhes/opções.

* **Domínio de rastreamento pela primeira vez**: a criação pela primeira vez de domínios de link de rastreamento de email exigirá a intervenção manual do [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. A criação subsequente de subdomínio no mesmo domínio é permitida na interface do usuário.

* **Somente no local do Marketo**: no momento, esse recurso está disponível somente no local. O Marketo Engage no Cloud Services precisará configurar o SSL entrando em contato com o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* **Adicionando certificados a domínios existentes**: não há suporte no momento para adicionar certificados a domínios existentes. Para domínios pré-existentes ou casos em que você não marcou a caixa do certificado SSL, entre em contato com o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para adicionar o certificado.

* **Exclusão de domínios**: a exclusão de um domínio não exclui automaticamente o certificado SSL no momento. Isso será abordado em uma versão futura.
