---
unique-page-id: 10099680
description: Importar dados de objeto personalizado - Documentos do Marketo - Documentação do produto
title: Importar dados de objeto personalizado
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# Importar dados de objeto personalizado {#import-custom-object-data}

É fácil importar dados de objetos personalizados para o seu banco de dados. Se você estiver usando objetos personalizados com empresas, consulte [Usando objetos personalizados com empresas](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) para obter mais informações.

1. Em Meu Marketo, vá para **Database**.

   ![](assets/db-1.png)

1. Clique em **Novo** e selecione **Importar dados de objeto personalizados**.

   ![](assets/image2016-4-7-10-6-54.png)

1. Clique em **Procurar** para localizar o ficheiro de dados. Selecione o formato de arquivo (Valores separados por vírgula neste exemplo).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Selecione o objeto personalizado.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Selecione o Modo de depuração no menu suspenso. Clique em **Next**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Use Dedupe campos como identificadores exclusivos quando criar ou atualizar registros de objetos personalizados. Este exemplo usa o campo Dedupe do objeto personalizado **car** - vin (número de ID do veículo). Se você estiver atualizando apenas registros de objetos personalizados, poderá selecionar o Guia do Marketo como o Modo de depuração.

1. Mapeie cada coluna para um campo Marketo , selecionando-o no menu suspenso.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Verifique se os valores no arquivo correspondem ao tipo de campo que está correspondendo a (por exemplo, texto, inteiro, etc.), caso contrário, o arquivo será rejeitado.

1. Clique em **Next**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Clique em **Importar**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >O limite de tamanho para objetos personalizados é de 100 MB.

   >[!TIP]
   >
   >Insira seu endereço de email no campo **Enviar alerta para:** e o Marketo enviará um email para você quando a importação for concluída!

1. No canto superior direito da tela, você verá uma notificação enquanto a importação estiver em execução e os resultados finais quando for concluída.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   Sim!

>[!MORELIKETHIS]
>
>[Como entender objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
