---
title: Solución de problemas con Microsoft defender para Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801424"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Solucionar problemas con Office 365 ATP

- ¿Hay **retrasos en la entrega de mensajes de correo electrónico** ? Pruebe a usar la opción de entrega dinámica para las directivas de datos adjuntos seguros de ATP. Esto evitará los retrasos en la entrega de mensajes de correo electrónico al proteger a los destinatarios de archivos malintencionados.
- **¿Desea informar de falsos positivos o falsos negativos** ? Use este vínculo para enviar el archivo para su análisis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **¿Sabía que puede habilitar la protección de vínculos seguros de ATP para el correo electrónico que se envía entre las personas de su organización** ? Siga estos pasos:
    1. Vaya a https://protection.office.com e inicie sesión.
    2. Vaya a **Threat management**  >  **Policy**  >  **vínculos seguros** de la Directiva de administración de amenazas.
    3. En **directivas que se aplican a destinatarios específicos** , edite (o agregue) una directiva.
    4. Seleccione **aplicar vínculos seguros a los mensajes enviados dentro de la organización** .
    5. Guarde la Directiva y espere unos 30 minutos para que los cambios funcionen en el centro de proceso de información.
- Para obtener más ayuda con ATP, consulte [Microsoft defender para Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).