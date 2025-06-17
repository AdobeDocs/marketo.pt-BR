---
unique-page-id: 11377395
description: Adicionar um domínio de marca adicional - Documentação do Marketo - Documentação do produto
title: Adicionar outro domínio de marca
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: dafac137a6c626794f3b9b2bfaa2fc2de9f2cb75
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 3%

---

# Adicionar outro domínio de marca {#add-an-additional-branding-domain}

Adicione outro domínio de marca ao executar várias marcas em uma única instância do Marketo e quiser que cada uma tenha seus próprios links de rastreamento de marca.

>[!PREREQUISITES]
>
>Você deve [substituir o link de rastreamento genérico](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"} por um domínio com marca antes de adicionar outros domínios com marca.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/add-an-additional-branding-domain-1.png)

1. Clique em **[!UICONTROL Email]**.

   ![](assets/add-an-additional-branding-domain-2.png)

1. Clique em **[!UICONTROL Adicionar]** para adicionar outro domínio de marca.

   ![](assets/add-an-additional-branding-domain-3.png)

1. Insira o nome do novo domínio de marca, selecione _Tornar Domínio Primário_ e/ou _Gerar Certificado SSL_ (ambos opcionais) e clique em **[!UICONTROL Salvar]**.

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _Tornar Domínio Primário_: Transforme este domínio em seu domínio primário. Todos os emails não enviados existentes definidos como &quot;Padrão&quot; e todos os emails recém-criados serão padronizados para o domínio primário. Você pode [substituir isto por email](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}.
>
>* _Gerar Certificado SSL_: você pode criar uma SSL (Secure Sockets Layer) com a criação do domínio. O primeiro domínio de rastreamento iniciará uma configuração única de infraestrutura que pode levar algumas horas. Você será notificado após a conclusão e poderá configurar o primeiro domínio. Para adicionar SSL aos seus domínios existentes, entre em contato com o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

## Mensagens de erro {#error-messages}

<table><thead>
  <tr>
    <th>Erro</th>
    <th>Detalhes</th>
  </tr></thead>
<tbody>
  <tr>
    <td><i>Erro inesperado encontrado ao criar um domínio. Entre em contato com o Suporte para obter assistência.</i></td>
    <td>Ocorreu um erro inesperado. Colete logs e detalhes de erros e encaminhe o problema para o <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Suporte da Marketo</a>.</td>
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
    <td><i>A configuração do Cloudflare foi iniciada. Tente novamente mais tarde.</i></td>
    <td>Ao criar o primeiro domínio de rastreamento para a instância, ocorre uma configuração de infraestrutura única no Cloudfare. Esta mensagem indica que a configuração foi iniciada e pode levar até três horas.</td>
  </tr>
  <tr>
    <td><i>A configuração do Cloudflare ainda está em andamento. Tente novamente mais tarde.</i></td>
    <td>veja acima</td>
  </tr>
  <tr>
    <td><i>A configuração do Cloud Flare falhou devido a um erro inesperado. Entre em contato com o suporte ao cliente.</i></td>
    <td>A configuração inicial da infraestrutura do Cloudfare falhou. Entre em contato com o <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Suporte da Marketo</a> para obter assistência.</td>
  </tr>
</tbody></table>

## Itens a Observar {#things-to-note}

* **Mapeamento de DNS para o domínio para o Marketo Engage**: antes de adicionar domínios na interface do usuário, você deve [mapear CNAMEs para um domínio fornecido pelo Marketo](https://experienceleague.adobe.com/pt-br/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **SSLs personalizados**: se você precisar de um SSL personalizado, envie um [Tíquete de suporte](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Não use a caixa de seleção de autoatendimento para criação de SSL.

* **SSLs pré-existentes**: ao adicionar um domínio, o sistema verifica se há SSLs pré-existentes, que podem ter sido criados manualmente antes. Se encontrar essa validação, crie seu domínio sem selecionar a criação de SSL e nós os conectaremos para você. [Contate o Suporte](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para obter mais detalhes/opções.

* **Domínio de rastreamento pela primeira vez**: a criação pela primeira vez de domínios de link de rastreamento de email exigirá a intervenção manual do [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. A criação subsequente de subdomínio no mesmo domínio é permitida na interface do usuário.

* **Adicionando certificados a domínios existentes**: não há suporte no momento para adicionar certificados a domínios existentes. Para domínios pré-existentes ou casos em que você não marcou a caixa do certificado SSL, entre em contato com o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para adicionar o certificado.

* **Editar ou remover certificados em domínios existentes**: se precisar atualizar ou remover um SSL existente, entre em contato com o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* **Exclusão de domínios**: a exclusão de um domínio não exclui automaticamente o certificado SSL no momento. Isso será abordado em uma versão futura.

>[!MORELIKETHIS]
>
>[Editar Seu Domínio De Identidade Visual Padrão](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
