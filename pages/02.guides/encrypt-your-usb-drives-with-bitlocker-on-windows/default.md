---
title: 'Encrypt your USB Drives with BitLocker'
published: true
metadata:
    author: 'Gabor Szathmari'
    description: 'Protect your data from physical theft. Use BitLocker on your Windows PC to encrypt your portable USB drives.'
    'og:title': 'Encrypt your USB Drives with BitLocker'
    'og:type': article
    'og:description': 'Protect your data from physical theft. Use BitLocker on your Windows PC to encrypt your portable USB drives.'
    'og:image': 'https://privacyforjournalists.org.au/user/pages/02.guides/encrypt-your-usb-drives-with-bitlocker-on-windows/social.png'
    'twitter:card': summary_large_image
    'twitter:site': '@PrivacyJournAU'
    'twitter:creator': '@gszathmari'
    'twitter:title': 'Encrypt your USB Drives with BitLocker'
    'twitter:description': 'Protect your data from physical theft. Use BitLocker to encrypt your portable USB drives.'
    'twitter:image': 'https://privacyforjournalists.org.au/user/pages/02.guides/encrypt-your-usb-drives-with-bitlocker-on-windows/social.png'
taxonomy:
    tag:
        - windows
        - disk
visible: true
---

# Encrypt your USB Drives with BitLocker

[TOC]

The purpose of encrypting your external USB drives and memory sticks is similar to [full-disk encryption](../encrypt-your-hard-drive-with-bitlocker-windows). It ensures that your files remain secure in case the USB drive is lost or stolen.

There are many situations these could happen:

* You are staying in a hotel and the USB drive is left in your room unattended
* Someone breaks into your apartment or office
* The USB stick is left in the trunk of the car and someone breaks into it
* Someone snatches drive from your purse or backpack
* You are deliberately put into a situation that separates you from your device. For example a thorough security check at the airport

Full disk encryption is an effective practice to protect yourself and your sources in these situations. Read on to configure BitLocker to protect your external drives. At the end of this article, you will learn to encrypt and use a USB drive for storing your sensitive documents.

## Checking Windows Release

BitLocker is the built-in full disk encryption software in Windows. Unfortunately, not every edition of Windows features this tool. Firstly, check whether you have Windows Pro or Enterprise edition on your device.

![](check-os-release-1.png?lightbox=1024&cropResize=600,600)

![](check-os-release-3.png?lightbox=1024&cropResize=600,600)

If you have another version than Pro or Enterprise, you must buy an upgrade from Microsoft. The good news is that you don't need to reinstall everything, the upgrade happens automatically in the background once you purchased a new product key. Follow [these instructions](https://support.microsoft.com/en-us/help/12384/windows-10-upgrading-home-to-pro?target=_blank) to upgrade your system.

## Configuring BitLocker

* Once you confirmed that your operating system supports BitLocker, right-click on the external drive you wish to encrypt. Select **Turn BitLocker on** from the menu.

![](bitlocker-1.png?lightbox=1024&cropResize=600,600)

* Select **Use a password to unlock the drive** option. Choose a password you never used anywhere else and enter it twice.

![](bitlocker-2.png?lightbox=1024&cropResize=600,600)

* You must save the recovery key somewhere. You can save the recovery key into a file.

![](bitlocker-3.png?lightbox=1024&cropResize=600,600)

![](bitlocker-4.png?lightbox=1024&cropResize=600,600)

* Open the file you just saved, and either save your recovery key in a password wallet, or write it down on a piece of paper and lock it up somewhere.

!! If you choose to write your backup recovery key down, never store it along with your laptop (e.g. laptop bag, your wallet)

* Now delete the text file you save earlier, and empty the **Recycle Bin** if necessary

!!! Be careful. If you forget your password and lose the backup recover key, the contents of your hard disk is lost forever

* Click **Next** to continue the configuration process

![](bitlocker-6.png?lightbox=1024&cropResize=600,600)

* Choose the second option to encrypt the entire device instead of the used space

![](bitlocker-8.png?lightbox=1024&cropResize=600,600)

* Select the **Compatible mode** if you wish to use the external drive on Windows 7 or 8 machines. Otherwise, choose the **New encryption mode**

![](bitlocker-9.png?lightbox=1024&cropResize=600,600)

* Click **Next**

![](bitlocker-10.png?lightbox=1024&cropResize=600,600)

* The encryption process should start running

![](bitlocker-11.png?lightbox=1024&cropResize=600,600)

* Once the encryption process is ready, click **Close**. Your USB stick is now encrypted.

![](bitlocker-12.png?lightbox=1024&cropResize=600,600)

## Ejecting the Encrypted USB Drive

From now on, the drive can be ejected as any other unencrypted drive. Simply right-click on the icon of the device, and select **Eject**.

![](unmount-drive-1.png?lightbox=1024&cropResize=600,600)

## Mounting the Encrypted USB Drive

When you pop the encrypted USB stick into your laptop, Windows will prompt your for the password to unclock the drive

* Click on the notification in the bottom-right corner to enter your password

![](mount-drive-1.png?lightbox=1024&cropResize=600,600)

* Key in the unlock password

![](mount-drive-2.png?lightbox=1024&cropResize=600,600)

![](mount-drive-3.png?lightbox=1024&cropResize=600,600)

* If your hard disk is encrypted, it is safe to save your password. This enables Windows to mount your encrypted USB stick without prompting for the password again.

![](mount-drive-4.png?lightbox=1024&cropResize=600,600)

* Once the encrypted drive is mounted, you can use it as any other unencrypted USB stick

![](mount-drive-5.png?lightbox=1024&cropResize=600,600)

## Further Reading

* [Encrypt your Hard Drive with Bitlocker](../encrypt-your-hard-drive-with-bitlocker-windows) on Windows

_Photo courtesy of [William Hook](https://www.flickr.com/photos/williamhook/3468484351/in/photolist-6huTyk-959hYV-6vCGR7-GaSBix-doB3zn-eMma9J-aQ4eg-5LtjoZ-5rgbKN-y1GPL-8Es2xt-65ae1u-61EpY7-48vv5w-8FvSqR-5Lxu61-2mLSK6-5owhpA-614eXo-6iMxve-6fE9Re-6iRHuY-5Lxu7G-6teu4j-48dBDS-6uT36D-7Dr5cQ-6R41Y7-4kKP24-5ZZ3iK-8hkNUX-okhy56-614g5y-5Lxu57-5LxzR5-8DNFZb-5ZZ3hz-5ZZ3W8-5ZZ4at-FMS7s-dfbk9R-61E6wo-6vCGEq-8DNG4L-doBaLh-99yD5H-8FvSNt-5LtjW4-8fRVuF-5hrRvx?rel=nofollow)_