---
title: No se ha configurado el certificado de inserción de Apple MDM
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716874"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>No se ha configurado el certificado de inserción de Apple MDM

No se ha configurado un certificado de inserción de MDM de Apple (también conocido como certificado de servicio de notificaciones push de Apple o APNs) en su suscripción. Si no se ha configurado un certificado de inserción de MDM de Apple, no podrá inscribir y administrar los dispositivos iOS y MacOS. Después de agregar el certificado a Intune, los usuarios pueden instalar la aplicación del portal de la empresa para inscribir sus dispositivos iOS.

1. Seleccione **"Acepto".** para conceder permiso a Microsoft para enviar datos a Apple.

2. Seleccione **Descargar al CSR** la solicitud de firma de certificado Intune necesaria para crear un certificado de inserción de Apple MDM. El archivo se usa para solicitar un certificado de relación de confianza del portal de certificados de inserción de Apple.

3. Seleccione **Crear el certificado de inserción de MDM** ir al portal de certificados de inserción de Apple. Inicie sesión con el ID. de Apple de su empresa y, a continuación, seleccione **Crear un certificado**. Seleccione **Elegir archivo**, desplácese hasta el archivo de solicitud de firma de certificado y elija **Cargar**. En la página de confirmación, elija **Descargar** para descargar el archivo de certificado (.pem) y guardar el archivo localmente.
 
**Tenga en cuenta**: el certificado está asociado con el ID. de Apple usado para crearlo. Se recomienda usar un ID de Apple de empresa para las tareas de administración y asegurarse de que el buzón lo supervisa más de una persona o una lista de distribución. Nunca use un ID. de Apple personal. Use el mismo ID. de Apple para renovar el certificado de inserción de Apple cada 12 meses.
 
4. Escriba el ID. de Apple usado para crear el certificado de inserción de Apple MDM. Registre este identificador como un aviso para cuando necesite renovar el certificado.

5. Vaya al archivo de certificado (.pem), elija **Abrir**y elija **Cargar**. Con el certificado de inserción, Intune puede inscribir y administrar dispositivos Apple.