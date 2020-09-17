---
title: How-to-Import-NK2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780076"
---
# <a name="how-to-import-nk2-files"></a>Cómo importar archivos. NK2 

Al iniciar Microsoft Outlook 2013, Outlook 2016, Outlook 2019 u Outlook para Microsoft 365 por primera vez, la caché de sobrenombres (almacenada en el archivo *ProfileName*. NK2) se importa en un mensaje oculto en el almacén de mensajes predeterminado.

Para importar archivos. NK2 en Outlook 2013, Outlook 2016, Outlook 2019 u Outlook para Microsoft 365, asegúrese de que el archivo. NK2 se encuentra en la siguiente carpeta:%appdata%\Microsoft\Outlook

**Nota**: el archivo. NK2 debe tener el mismo nombre que el perfil actual de Outlook 2013 o Outlook 2016. De forma predeterminada, el nombre del perfil es "Outlook". Para comprobar el nombre del perfil, siga estos pasos: 
1. Haga clic en **Inicio** y en **Panel de control**.
2. Haga doble clic en **correo**.
3. En el cuadro de diálogo Configuración de correo, seleccione **Mostrar perfiles**.
4. Seleccione **iniciar**  >  **ejecución**.
5. En el cuadro **abrir** , escriba *outlook.exe/importnk2*y, después, seleccione **Aceptar**. 

Una vez que haya importado el archivo. NK2, el contenido del archivo se combinará en la memoria caché de sobrenombres existente almacenada en el buzón.

**Nota**: el nombre del archivo. NK2 se cambia por una extensión de nombre de archivo. Old la próxima vez que inicie Outlook 2013, Outlook 2016, Outlook 2019 o Outlook para Microsoft 365. Si desea volver a importar el archivo. NK2, quite primero la extensión de nombre de archivo. old.

Para obtener más información, vea [importar o copiar la lista de autocompletar en otro equipo](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).