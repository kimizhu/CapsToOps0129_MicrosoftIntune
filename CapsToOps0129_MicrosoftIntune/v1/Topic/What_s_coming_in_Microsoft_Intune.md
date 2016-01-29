---
description: na
keywords: na
title: What&#39;s coming in Microsoft Intune
search: na
ms.date: 2016-01-26
ms.service: microsoft-intune
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: f49650f4-31fa-406c-a4da-d8c9a4a8384d
ms.author: lindavr@microsoft.com
robots: noindex,nofollow
---
# What&#39;s coming in Microsoft Intune
This information is provided under NDA on an extremely limited basis and is subject to change. Some features listed here are at risk of not making the cutoff dates and may be delayed until a future release. Other features are being tested in a pilot (flighting) to ensure they're customer-ready. Please reach out to your Intune/PM buddy if you have any questions or concerns.
## New in service
The following changes are under development for Intune:
### App management
- **Take advantage of iOS "Open-in" Management for devices that are not enrolled in Intune.** Intune administrators can use their 3rd-party mobile device management (MDM) vendor to take advantage of iOS "Open-In" management. You can send an App Config setting to the app to tell it what work account is required.  

	This approach has two main benefits:

	1. Users are required to log in with their Work account before they get access to any corporate data from Cloud Services or other apps. This ensures that MAM policies are in place when the data is accessed.

	2. Managed native email profiles and other iOS-managed apps can share files and data with the Intune MAM-managed apps. 

	The way this works is the MAM SDK inside the Office app detects the presence of the app config setting and determines that it means the device is managed and uses iOS Managed "Open-In". The SDK then categorizes any incoming data or files as "corporate" and treats them accordingly.  

- **Mobile app configuration policies give you more flexibility to specify user details for iOS apps.** Intune administrators can supply user settings that an iOS app might need when it is opened. For example, you can supply a network port, or a user name. For details, see [Configure apps with mobile app configuration policies in Microsoft Intune](https://technet.microsoft.com/library/mt481447.aspx). ***Not sure you should link to topic in WG; will it have been revised?***

- **Deploy and manage Windows Store for Business apps from the Intune administrator console.** The Intune processes supports "online licensed apps". This means that the content of the app, and app licensing is still managed by the Windows Store for Business. ***I don't get this. What's the customer benefit? Why are we talking about this?***

- **The RMS Sharing app is supported for Android.** IT administrators can deploy mobile application management policies so end users can view images, AV, and PDF files more securely, whether or not IT uses Intune to manage the devices. 

### Device management
- **PFX certificates distribution for iOS devices.** Intune administrators can create iOS PFX certificates for Wi-Fi, email, and VPN authentication on iOS devices. This feature is already available for Android and Windows 10 devices.

## Changes and updates to Microsoft Company Portal
The following changes are under development for the company portal apps:

### iOS
- **New iOS enrollment flow checklist design for end users.** The enrollment flow has been improved to a checklist style design with descriptive screens to provide information about the enrollment process. (link to notice board alert)
- **Improved end-user experience when when they open managed apps.**  When users open a managed app, they will get a message with options to learn more about app management and can also choose to dismiss the notification permanently. This feature is currently supported in Outlook and will appear in other MAM-enabled apps in the coming months. Read more on the [Intune blog](http://blogs.technet.com/b/microsoftintune/archive/2016/01/12/new-end-user-experience-mobile-application-management-for-ios.aspx).
