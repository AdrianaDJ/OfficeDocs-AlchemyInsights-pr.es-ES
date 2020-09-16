---
title: Problemas con MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755148"
---
# <a name="issues-with-azure-mfa"></a>Problemas con Azure MFA
Hay un par de cosas para comprobar si los usuarios no pueden iniciar sesión con la autenticación multifactor (MFA)

1. Es posible que el usuario afectado esté bloqueado en el portal de Azure Active Directory. Si ese es el caso, los intentos de autenticación para ese usuario específico se denegarán automáticamente. [Siga los pasos de este artículo para desbloquearlos.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Si el proceso de desbloqueo del usuario no es de ayuda o el usuario no está bloqueado, puede intentar restablecer la MFA para el usuario y se volverá a pasar por el proceso de inscripción. [Siga los pasos descritos en este artículo.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Si esta es la primera vez que habilita la MFA y los usuarios no pueden iniciar sesión en clientes que no sean exploradores como Outlook, Skype, etc., quizá ADAL (biblioteca de autenticación de Active Directory) no está habilitado en su suscripción de O365. En este caso, deberá conectarse a Exchange Online PowerShell y ejecutar este cmdlet:  *set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*