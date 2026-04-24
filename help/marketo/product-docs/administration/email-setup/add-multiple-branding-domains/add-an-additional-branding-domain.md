---
unique-page-id: 11377395
description: Adicione domínios de marca extras para várias marcas em uma instância, de modo que cada uma tenha seus próprios links de rastreamento com marca.
title: Adicionar um novo domínio de marca
exl-id: df6e5afe-dbb0-4fbe-bf06-79d92a91b986
feature: Email Setup
source-git-commit: 6638f4a24aac6cf828f443d17b896a9dec9bca16
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 21%

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
    <td><i>SSL certificate has already been issued.</i></td>
    <td>Já existe um certificado SSL para este domínio personalizado. No further action is needed unless the certificate has expired or needs to be reissued.</td>
  </tr>
  <tr>
    <td><i>The default domain was not found. Please contact Support for assistance.</i></td>
    <td>Ocorreu um problema ao tentar localizar o domínio padrão. Please reach out to Support so they can investigate.</td>
  </tr>
  <tr>
    <td><i>Unexpected error encountered while creating a domain. Please contact Support for assistance.</i></td>
    <td>An unexpected error has occurred. Please gather logs and error details, and escalate the issue to <a href="https://nation.marketo.com/t5/support/ct-p/Support" target="_blank">Marketo Support</a>.</td>
  </tr>
</tbody></table>

## Things to Note {#things-to-note}

* **DNS mapping for domain to Marketo Engage**: Before adding adding domains in the UI, you must [map CNAMEs to a Marketo-provided domain](https://experienceleague.adobe.com/pt-br/docs/marketo/using/getting-started/initial-setup/setup-steps#customize-your-landing-page-urls-with-a-cname){target="_blank"}.

* **Custom SSLs**: If you need a custom SSL, please submit a [Support ticket](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}. Do not use the self-service checkbox for SSL creation.

* **Pre-existing SSLs**: While adding a domain, the system checks for pre-existing SSLs, which may have been manually created prior. If you encounter this validation, create your domain without selecting SSL creation, and we will connect them for you. [Contact Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} more additional details/options.

* **Deletion of domains**: Automatically deleting a domain **does not** delete the SSL certificate. Essa proteção evita erros de usuário que resultam na ausência de certificados SSL em um site. If you do want to remove the SSL certificates, [contact Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* If the domain you add is listed as anything other than a CNAME, the ability to add further branded tracking domains will be locked out. You will need to edit any existing domain and ensure it is a CNAME record and not, say, an A record. The Add button dynamically checks for CNAMES and CNAMES only.

>[!MORELIKETHIS]
>
>[Edit Your Default Branding Domain](/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md){target="_blank"}
