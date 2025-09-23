---
unique-page-id: 11377395
description: Adicionar um domínio de marca adicional - Documentação do Marketo - Documentação do produto
title: Adicionar um novo domínio de marca
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 3%

---

# Adicionar um novo domínio de marca {#add-an-additional-branding-domain}

Adicione outro domínio de marca ao executar várias marcas em uma única instância do Marketo e quiser que cada uma tenha seus próprios links de rastreamento de marca.

>[!PREREQUISITES]
>
>Você deve [substituir o link de rastreamento genérico](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"} por um domínio com marca antes de adicionar outros domínios com marca.

1. Vá para a área **[!UICONTROL Administrador]**.

   ![](assets/add-an-additional-branding-domain-1.png)

1. Clique em **[!UICONTROL Email]**.

   ![](assets/add-an-additional-branding-domain-2.png)

1. Clique em **[!UICONTROL Adicionar]** para adicionar outro domínio de marca.

   ![](assets/add-an-additional-branding-domain-3.png){width="600"}

1. Insira o nome do novo domínio de marca, selecione _Tornar Domínio Primário_ e/ou _Gerar Certificado SSL_ (ambos opcionais) e clique em **[!UICONTROL Salvar]**.

   ![](assets/add-an-additional-branding-domain-4.png)

>[!NOTE]
>
>* _Tornar Domínio Primário_: Transforme este domínio em seu domínio primário. Todos os emails não enviados existentes definidos como &quot;Padrão&quot; e todos os emails recém-criados serão padronizados para o domínio primário. Você pode [substituir isto por email](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/overwrite-primary-domain-for-emails.md){target="_blank"}.
>
>* _Gerar Certificado SSL_: você pode criar uma SSL (Secure Sockets Layer) com a criação do domínio. O primeiro domínio de rastreamento iniciará uma configuração única de infraestrutura que pode levar algumas horas. Você será notificado após a conclusão e poderá configurar o primeiro domínio. Para adicionar SSL aos seus domínios existentes, entre em contato com o [Suporte da Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

## Editar SSLs para domínios existentes

Siga estas etapas para habilitar o SSL nos domínios existentes.

1. Na área _[!UICONTROL Administrador]_, selecione **[!UICONTROL Email]**.

1. Na guia _[!UICONTROL Domínio]_, selecione a linha de domínio e clique em **[!UICONTROL Adicionar SSL]**.

   ![Administrador - Email - Domínio - Adicionar SSL](./assets/admin-email-branding-domain-add-ssl.png){width="600"}

1. Na caixa de diálogo, clique em **[!UICONTROL Confirmar]**.

   ![Adicionar SSL - Confirmar](./assets/generate-ssl-cert-confirm.png){width="400"}

## Mensagens de erro {#error-messages}

<table><thead>
  <tr>
    <th>Erro</th>
    <th>Detalhes</th>
  </tr></thead>
<tbody>
<tr>
    <td><i>O domínio já existe.</i></td>
    <td>Já existe um domínio com o mesmo nome.</td>
  </tr>
  <tr>
    <td><i>O domínio não está mapeado para o domínio padrão.</i></td>
    <td>O domínio personalizado não está mapeado corretamente para o domínio padrão. Verifique as configurações de mapeamento de domínio e certifique-se de que a configuração DNS aponte para o domínio padrão correto.</td>
  </tr>
  <tr>
    <td><i>Não foi possível emitir certificados SSL devido a registros CAA sem suporte. Solicite que a equipe de TI atualize seus registros de CAA.</i></td>
    <td>Os registros CAA não estão atualizados. Para aqueles que usam certificados SSL gerenciados pela Marketo Engage, os registros CAA precisam ser atualizados para certificados recomendados pelo fornecedor. Entre em contato com o departamento de TI para atualizar os registros de CAA. Consulte <a href="https://nation.marketo.com/t5/product-blogs/changes-to-marketo-engage-secured-domains-platform/ba-p/329305#M2246">esta página</a> para obter detalhes adicionais.</td>
  </tr>
  <tr>
    <td><i>O certificado SSL já foi emitido.</i></td>
    <td>Já existe um certificado SSL para este domínio personalizado. Nenhuma ação adicional é necessária, a menos que o certificado tenha expirado ou precise ser reemitido.</td>
  </tr>
  <tr>
    <td><i>O domínio padrão não foi encontrado. Entre em contato com o Suporte para obter assistência.</i></td>
    <td>Ocorreu um problema ao tentar localizar o domínio padrão. Entre em contato com o Suporte para que possam investigar.</td>
  </tr>
  <tr>
    <td><i>Erro inesperado encontrado ao criar um domínio. Entre em contato com o Suporte para obter assistência.</i></td>
    <td>Ocorreu um erro inesperado. Colete logs e detalhes de erros e encaminhe o problema para o <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Suporte da Marketo</a>.</td>
  </tr>
</tbody></table>

## Itens a Observar {#things-to-note}

* **Mapeamento de DNS para o domínio para o Marketo Engage**: antes de adicionar domínios na interface do usuário, você deve [mapear CNAMEs para um domínio fornecido pelo Marketo](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **SSLs personalizados**: se você precisar de um SSL personalizado, envie um [Tíquete de suporte](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Não use a caixa de seleção de autoatendimento para criação de SSL.

* **SSLs pré-existentes**: ao adicionar um domínio, o sistema verifica se há SSLs pré-existentes, que podem ter sido criados manualmente antes. Se encontrar essa validação, crie seu domínio sem selecionar a criação de SSL e nós os conectaremos para você. [Contate o Suporte](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} para obter mais detalhes/opções.

* **Exclusão de domínios**: a exclusão automática de um domínio **não** exclui o certificado SSL. Essa proteção evita erros de usuário que resultam na ausência de certificados SSL em um site. Se você deseja remover os certificados SSL, [contate o Suporte](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

>[!MORELIKETHIS]
>
>[Editar Seu Domínio De Identidade Visual Padrão](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
