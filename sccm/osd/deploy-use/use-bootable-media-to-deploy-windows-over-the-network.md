---
title: Use bootable media to deploy Windows over the network | Configuration Manager
description: "Use bootable media deployments in System Center Configuration Manager to deploy the operating system when the destination computer starts."
ms.custom: na
ms.date: 10/06/2016
ms.prod: configuration-manager
ms.reviewer: na
ms.suite: na
ms.technology:
  - configmgr-osd
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 999b5409-7e72-48d2-8554-4d44427ce383
caps.latest.revision: 5
author: Dougebyms.author: dougebymanager: angrobe

---
# Use bootable media to deploy Windows over the network with System Center Configuration Manager*Applies to: System Center Configuration Manager (Current Branch)*
Bootable media deployments in System Center Configuration Manager let you deploy the operating system when the destination computer starts. When the destination computer starts, it retrieves the task sequence, the operating system image, and any other required content from the network. Because that content is not included on the media, you can update the content without having to re-create the media.  

 You can deploy operating systems over the network by using multicast in the following operating system deployment scenarios:  

-   [Refresh an existing computer with a new version of Windows](refresh-an-existing-computer-with-a-new-version-of-windows.md)  

-   [Install a new version of Windows on a new computer (bare metal)](install-new-windows-version-new-computer-bare-metal.md)  

-   [Replace an existing computer and transfer settings](replace-an-existing-computer-and-transfer-settings.md)  

 Complete the steps in one of the operating system deployment scenarios and then use the following sections to use bootable media to deploy the operating system.  

## Configure deployment settings  
 When you use bootable media to start the operating system deployment process, you must configure the deployment to make the operating system available to media. You can configure this on the **Deployment Settings** page of the Deploy Software Wizard or the **Deployment Settings** tab in the properties for the deployment.  For the **Make available to the following** setting, configure one of the following:  

-   **Configuration Manager clients, media and PXE**  

-   **Only media and PXE**  

-   **Only media and PXE (hidden)**  

## Create the bootable media  
 You can specify whether the  bootable media is a USB flash drive or CD/DVD set. The computer that will start the media must support the option that you choose as  a bootable drive. For more information, see [Create bootable media](create-bootable-media.md).  

##  <a name="BKMK_Deploy"></a> Install the operating system from  bootable media  
 Insert the bootable media in a bootable drive on the computer, and then power it on to install the operating system.  
