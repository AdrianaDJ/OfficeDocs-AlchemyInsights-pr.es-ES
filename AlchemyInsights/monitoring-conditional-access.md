---
title: Supervisión del acceso condicional
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702920"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Supervisión del acceso condicional para Exchange

Los usuarios con acceso condicional recibirán un correo electrónico de notificación si no cumplen los requisitos de acceso de la organización. Para solucionarlo, recomendamos una o varias de las siguientes soluciones:
  
- Si se supone que el dispositivo está inscrito, aconseje al usuario que vaya a la aplicación portal de empresa y compruebe que aparece en el portal de empresa. Si no lo hace, el usuario debería inscribir el dispositivo.
    
- En el portal de Azure, vaya a **Intune \> Compliance Device Compliance**. En **supervisión** , haga clic en **cumplimiento del dispositivo**. Vea el informe de cumplimiento de dispositivos para comprobar que el dispositivo del usuario está marcado como compatible. 
    
- En el portal de Azure, vaya a **Intune \> Compliance Device Compliance**. En **administrar**, haga clic en **directivas**. En la lista de directivas de cumplimiento, compruebe que haya un perfil asignado al dispositivo del usuario. Si no hay ningún perfil asignado, Intune no podrá confirmar el estado de cumplimiento del dispositivo. 
    
- Edite la asignación de acceso condicional del usuario.
    
1. En el portal de Azure, vaya a **Intune \> \> policies de acceso condicional**
    
2. Seleccionar una directiva de la lista
    
3. Haga clic en **usuarios y grupos**
    
4. Para dirigir una determinada Directiva a una persona, agréguela a la lista **incluir** . Para asegurarse de que se omite una persona de la Directiva, agréguela a la lista de **exclusión** . 
    
Más información: [cómo supervisar los dispositivos de acceso condicional](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

