---
title: 'Encrypt your Hard Drive with BitLocker'
published: true
metadata:
    author: 'Gabor Szathmari'
    description: 'Protect your data from physical theft. Activate BitLocker on your Windows PC to enable full-disk encryption on your hard drives.'
    'og:title': 'Encrypt your Hard Drive with BitLocker'
    'og:type': article
    'og:description': 'Protect your data from physical theft. Activate BitLocker on your Windows PC to enable full-disk encryption on your hard drives.'
    'og:image': 'https://privacyforjournalists.org.au/user/pages/02.guides/encrypt-your-hard-drive-with-bitlocker-windows/social.png'
    'twitter:card': summary_large_image
    'twitter:site': '@PrivacyJournAU'
    'twitter:creator': '@gszathmari'
    'twitter:title': 'Encrypt your Hard Drive with BitLocker'
    'twitter:description': 'Activate BitLocker on your Windows PC to enable full-disk encryption on your hard drives'
    'twitter:image': 'https://privacyforjournalists.org.au/user/pages/02.guides/encrypt-your-hard-drive-with-bitlocker-windows/social.png'
taxonomy:
    tag:
        - windows
        - disk
visible: true
---

# Encrypt your Hard Drive with BitLocker

[TOC]

Hard drive encryption protects from two things. Firstly, nobody can tamper with your computer (e.g. install backdoors) if you leave it unattended. Secondly, your files remain secure in case the laptop is stolen.

There are many situations these could happen:

* You are staying in a hotel and the laptop is left in your room unattended
* Someone breaks into your apartment or office
* The laptop is left in the trunk of the car and someone breaks into it
* Someone snatches the device from your hands, or robs you
* You are deliberately put into a situation that separates you from your device. For example a thorough security check at the airport

Full disk encryption is a very effective way to protect yourself and your sources in these situations. Read on to configure BitLocker full disk encryption on Windows 10.

## Checking Windows Release

BitLocker is the built-in full disk encryption software in Windows. Unfortunately, not every edition of Windows features this tool. Firstly, check whether you have Windows Pro or Enterprise edition on your device.

![](check-os-release-1.png?lightbox=1024&cropResize=600,600)

![](check-os-release-3.png?lightbox=1024&cropResize=600,600)

If you have another version than Pro or Enterprise, you must buy an upgrade from Microsoft. The good news is that you don't need to reinstall everything, the upgrade happens automatically in the background once you purchased a new product key. Follow [these instructions](https://support.microsoft.com/en-us/help/12384/windows-10-upgrading-home-to-pro?target=_blank) to upgrade your system.

## Configuring BitLocker

* Once you confirmed that your operating system supports BitLocker, run it from the Start menu

![](run-bitlocker-1.png?lightbox=1024&cropResize=600,600)

* Click on the **Turn BitLocker on** link

![](run-bitlocker-2.png?lightbox=1024&cropResize=600,600)

If you are presented with the following error, follow the instructions in the _Using BitLocker without a TPM chip_ section. Otherwise, scroll-down to the _Using BitLocker with a TPM chip_ section.

### Using BitLocker without a TPM chip

![](tpm-config-1.png?lightbox=1024&cropResize=600,600)

The error means that a thing called [TPM chip](http://www.howtogeek.com/237232/what-is-a-tpm-and-why-does-windows-need-one-for-disk-encryption/?target=_blank) is missing from your laptop. This chip is normally used to store the disk decryption key in a secure manner. In case the chip was not installed by the manufacturer of your computer, you can still use BitLocker and unlock your disk with a password instead.

* Open the Start menu and run the *Edit Group Policy* application (enter the word 'group' in the search field)

![](tpm-config-2.png?lightbox=1024&cropResize=600,600)

* Now go to **Local Computer Policy -> Computer Configuration -> Administrative Templates -> Windows Components -> BitLocker Drive Encryption -> Operating System Drives**. Double-click on **Require additional authentication at startup**

![](tpm-config-3.png?lightbox=1024&cropResize=600,600)

* In the new window, select the **Enabled** radio button and make sure the rest of the settings looks like the ones from the screenshot

![](tpm-config-5.png?lightbox=1024&cropResize=600,600)

* Click **OK**. The 'State' of **Require additional authentication at startup** should be **Enabled**

![](tpm-config-6.png?lightbox=1024&cropResize=600,600)

* Run **BitLocker** again from the start menu and continue with the configuration

![](run-bitlocker-1.png?lightbox=1024&cropResize=600,600)

* If you do not have a TPM chip, you are presented with the following options. Select **Enter a password** option.

![](run-bitlocker-4.png?lightbox=1024&cropResize=600,600)

* Now enter a password. You should not reuse any of your passwords here.

![](run-bitlocker-5.png?lightbox=1024&cropResize=600,600)

* Now you need to save your backup recovery key. The password or the backup recovery key are the two things that can unlock your hard drive. 

!!! Be careful. If you forget your password and lose the backup recover key, the contents of your hard disk is lost forever

* Choose **Print the recovery key** option

![](run-bitlocker-6.png?lightbox=1024&cropResize=600,600)

* Choose the **Microsoft Print to PDF** option 

![](run-bitlocker-8.png?lightbox=1024&cropResize=600,600)

* Save the PDF file with your recovery key in it to the Desktop

![](run-bitlocker-9.png?lightbox=1024&cropResize=600,600)

* Double-click the PDF file to open it. Your recovery key is the long block of digits near the bottom. Write it down to a piece of paper and store in a secure location, or save the key into a password wallet.

!! If you choose to write your backup recovery key down, never store it along with your laptop (e.g. laptop bag, your wallet)

![](run-bitlocker-10.png?lightbox=1024&cropResize=600,600)

* Once you wrote key recovery key down, delete the PDF file. Empty the **Recycle Bin** if necessary.

* Now click **Next** and select the **Encrypt entire drive** option

![](run-bitlocker-12.png?lightbox=1024&cropResize=600,600)

* Select the **New encryption mode** option

![](run-bitlocker-13.png?lightbox=1024&cropResize=600,600)

* Click **Next** again

![](run-bitlocker-14.png?lightbox=1024&cropResize=600,600)

* Restart your PC to start encrypting your drive

![](run-bitlocker-15.png?lightbox=1024&cropResize=600,600)

![](run-bitlocker-16.png?lightbox=1024&cropResize=600,600)

* Once your computer is restarted, you are presented with a window. Enter your password you chose earlier to unlock the hard disk.

!!! You will need to supply your password every time the computer is restarted

![](run-bitlocker-17.png?lightbox=1024&cropResize=600,600)

* You can continue working on your laptop while it is being encrypted. You can track the progress by double-clicking on the BitLocker icon next to your clock.

![](run-bitlocker-18.png?lightbox=1024&cropResize=600,600)

![](run-bitlocker-19.png?lightbox=1024&cropResize=600,600)

![](run-bitlocker-20.png?lightbox=1024&cropResize=600,600)

* Once the process finishes, you should see a padlock next to your **C:** drive indicating that it is encrypted

![](run-bitlocker-21.png?lightbox=1024&cropResize=600,600)

* You can verify the encryption by right-clicking on the **C:** drive and selecting **Manage BitLocker**

![](run-bitlocker-22.png?lightbox=1024&cropResize=600,600)

![](run-bitlocker-23.png?lightbox=1024&cropResize=600,600)

Your main hard drive is encrypted. Good job! Do not forget that all your portable drives and USB sticks should also be encrypted. Go back to our [guides](/guides) and read more about the encryption of portable drives.

### Using BitLocker with a TPM chip

If your computer has a TPM chip, the configuration should be very straightforward. Unfortunately, I do not have access to a computer with a TPM chip there is no guide on this one. Until then, follow the instructions on the [this site](https://countuponsecurity.com/2014/06/23/bitlocker-with-tpm-in-10-steps/?target=_blank).

!!!! Please help us expanding this guide by contributing. Check out the [community](/community) section to get in touch with us!

## Enabling Screen Auto-lock

To complete the process, you must enable auto-lock on your screen. In case your computer is unattended for a couple of minutes, the PC will lock itself. You will need to re-enter your user password (not the BitLocker password) to continue your work.

* Right-click on the desktop and select **Personalise**

![](screen-lock-1.png?lightbox=1024&cropResize=600,600)

* Select **Lock Screen** from the left and scroll down. Click on the **Screen saver settings**

![](screen-lock-2.png?lightbox=1024&cropResize=600,600)

* Select your favourite screen saver. Select a reasonably low amount of minutes to activate. Tick the **On resume, display log-on screen** box.

![](screen-lock-3.png?lightbox=1024&cropResize=600,600)

* If the screen saver is activated properly, it should ask for your password before you can use your PC again

![](screensaver-1.png?lightbox=1024&cropResize=600,600)

![](screen-lock-4.png?lightbox=1024&cropResize=600,600)

![](screen-lock-5.png?lightbox=1024&cropResize=600,600)

## Further Reading

* [Encrypting your laptop like you mean it](https://theintercept.com/2015/04/27/encrypting-laptop-like-mean/?target=_blank) - Micah Lee's article in The Intercept

_Photo courtesy of [Jeff Kubina](https://www.flickr.com/photos/kubina/326628676/in/photolist-uS4jU-RuRJQ-pSNtAB-5K5E2k-8barTQ-uS4aw-8fgZ8a-cUqxm9-6SCgsW-5K5DbM-9WT2xB-dZa5QS-7dVtAy-f3qh8-bQSyVv-sESH1N-kHnXz-eawrQf-9mKCgk-D93MfU-8VdPPg-iJXpA4-sERPxC-jVg7DH-9BLgz-6vywui-c4g6G5-4HTgd1-rLsqRa-99Pj8a-aC3AqV-fuMvt3-66eN63-a2iA6W-9d9JB2-uS4us-dFLgaj-nAbCjW-f33vU-cQoPPY-cpba8h-BGJap-uS4zk-uS4J9-hbXubC-cZYsqf-8fkg2m-5t3dPH-8kcpkK-uS4cz?rel=nofollow)_