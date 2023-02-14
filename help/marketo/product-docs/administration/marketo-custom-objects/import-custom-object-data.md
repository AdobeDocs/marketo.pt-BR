---
unique-page-id: 10099680
description: Importar dados de objeto personalizado - Documentos do Marketo - Documentação do produto
title: Importar dados de objeto personalizado
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 3%

---

# Importar dados de objeto personalizado {#import-custom-object-data}

É fácil importar dados de objetos personalizados para o seu banco de dados. Se você estiver usando objetos personalizados com empresas, consulte [Uso de objetos personalizados com empresas](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) para obter mais informações.

1. Em Meu Marketo, acesse **Banco de dados**.

   ![](assets/import-custom-object-data-1.png)

1. Clique em **Novo** e selecione **Importar dados de objeto personalizado**.

   ![](assets/import-custom-object-data-2.png)

1. Clique em **Procurar** para localizar o arquivo de dados. Selecione o formato de arquivo (Valores separados por vírgula neste exemplo).

   ![](assets/import-custom-object-data-3.png)

1. Selecione o objeto personalizado.

   ![](assets/import-custom-object-data-4.png)

1. Selecione o Modo de depuração no menu suspenso. Clique em **Próximo**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Use Dedupe campos como identificadores exclusivos quando criar ou atualizar registros de objetos personalizados. Esse exemplo usa o campo Dedupe da variável **carro** objeto personalizado - vin (número de ID do veículo). Se você estiver atualizando apenas registros de objetos personalizados, poderá selecionar o Guia do Marketo como o Modo de depuração.

1. Mapeie cada coluna para um campo Marketo , selecionando-o no menu suspenso.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Verifique se os valores no arquivo correspondem ao tipo de campo que está correspondendo a (por exemplo, texto, inteiro, etc.), caso contrário, o arquivo será rejeitado.

1. Clique em **Próximo**.

   ![](assets/import-custom-object-data-7.png)

1. Clique em **Importar**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >O limite de tamanho para objetos personalizados é de 100 MB.

   >[!TIP]
   >
   >Insira seu endereço de email no **Enviar alerta para:** e o Marketo enviará um email para você quando a importação for concluída!

1. No canto superior direito da tela, você verá uma notificação enquanto a importação estiver em execução e os resultados finais quando for concluída.

   ![](assets/import-custom-object-data-9.png)

   Sim!

>[!MORELIKETHIS]
>
>[Como entender objetos personalizados do Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
