---
title: 1065 desuso de la dirección IP saliente de EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806812"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Desuso de los intervalos de direcciones IP salientes de EOP

Hemos detectado un posible problema con su organización que (si no se ha corregido antes del 26 de octubre de 2018) podría romper el flujo de correo a sus destinos locales o externos. Como se comunicó anteriormente, para simplificar la administración del intervalo de direcciones IP, estamos consolidando los intervalos de direcciones IP de Exchange Online Protection (EOP) que se usan para enviar y recibir correo electrónico fuera de Microsoft 365. Nuestro análisis indica que uno o varios de los orígenes de correo electrónico externos o destinos que ha configurado en conectores de flujo de correo no aceptan conexiones de los intervalos de direcciones IP que se muestran [aquí](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Act antes del 26 de octubre para garantizar que estos orígenes y destinos acepten conexiones a y desde todas [las direcciones IP de EOP publicadas](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Para obtener más información acerca de este cambio, consulte publicaciones del centro de mensajes [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)o [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Nota**: si anteriormente usó la publicación de direcciones IP o URL a través de HTML, XML y RSS para las actualizaciones de extremos, deberá migrar también a los nuevos servicios web para automatizar estos tipos de actualizaciones. Para obtener más información, vea [categorías de extremos de microsoft 365 y el servicio Web de direcciones IP y URL de microsoft 365](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
