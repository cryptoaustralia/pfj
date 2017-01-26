---
title: 'Generating PGP Keys on Windows'
metadata:
    'author': 'Gabor Szathmari'
    'description': 'The first part of the series shows the installation and PGP key generation procedures on Windows'
    'og:title': 'Generating PGP Keys on Windows'
    'og:type': article
    'og:description': 'The first part of the series shows the installation and PGP key generation procedures on Windows'
    'og:image': https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png
    'twitter:card': 'summary_large_image'
    'twitter:site': @PrivacyJournAU
    'twitter:creator': @gszathmari
    'twitter:title': 'Generating PGP Keys on Windows'
    'twitter:description': 'The first part of the series shows the installation and PGP key generation procedures on Windows'
    'twitter:image': https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png
taxonomy:
    category:
        - pgp
    tag:
        - windows
---

# Generating PGP Keys on Windows

[TOC]

The following guide shows the detailed instructions for generating a PGP key-pair for sending and receiving encrypting emails.

At the end of this session, you will have a PGP public and private key-pair generated on your computer.

## Installing Gpg4Win

* Download **Gpg4Win** from [www.gpg4win.org](https://www.gpg4win.org)

![Gpg4Win home page](gpg-windows-gpg4win-2.png?lightbox=1024&cropResize=600,600)

![Gpg4Win home page](gpg-windows-gpg4win-1.png?lightbox=1024&cropResize=600,600)

* Double-click on the downloaded file to install the application

![Installing Gpg4Win](gpg-windows-gpg4win-3.png?lightbox=1024&cropResize=600,600)

* Now go to the start menu and launch **Kleopatra**

![Launching Kleopatra](kleopatra-start-menu.png?lightbox=1024&cropResize=600,600)

* Kleopatra is a PGP keychain manager application. The main window should look like as below.

![Kleopatra main window](kleopatra-main-window.png?lightbox=1024&cropResize=600,600)

## Generating a PGP Key-pair

One Gpg4Win is installed and Kleopatra is running, we can generate the first PGP key-pair

* Now click on **File => New Certificate**

![Generate new certificate](kleopatra-main-window-new-keychain.png?lightbox=1024&cropResize=600,600)

* Select the _'Create a personal OpenPGP key pair'_ option

![Generate new certificate](kleopatra-main-window-personal.png?lightbox=1024&cropResize=600,600)

* Enter your name and emails address into the following form

![Entering details](kleopatra-enter-details.png?lightbox=1024&cropResize=600,600)

* Review your settings then click on the _'Create Key'_ button if everything is all right

![Reviewing settings](kleopatra-review-details.png?lightbox=1024&cropResize=600,600)

* Now select a strong passphrase. This will protect your private key on your hard disk with encryption.

!! **Warning: Never reuse your passwords**  
!! Choose a brand-new passphrase that you have never used on any other service (e.g. Gmail) before

![Entering a strong passphrase](kleopatra-passphrase.png?lightbox=1024&cropResize=600,600)

* If the key generation was successful, you should be offered with the following options.

![Key generation is ready](kleopatra-key-generated.png?lightbox=1024&cropResize=600,600)

* Click on _'Finish'_ to finish the process

## Setting an Expiry Date on the Key-pair

Now we move forward with setting an expiry date on the keys. It is a good practice because if your key is compromised without your knowledge, the expiry date will limit the lifetime of your public and private keys.

* Open **Kleopatra** again

![Kleopatra main window](kleopatra-main-with-key.png?lightbox=1024&cropResize=600,600)

* Right-click on your PGP key-pair and select _'Change Expiry Date...'_

![Changing expiry date](kleopatra-set-expiry-menu.png?lightbox=1024&cropResize=600,600)

* Set *2 Years* as the expiry period then click _'OK'_

![Setting expiry date](kleopatra-change-expiry-date.png?lightbox=1024&cropResize=600,600)

* Expiry date should be set

![Expiry date is set](kleopatra-expiry-date-successful.png?lightbox=1024&cropResize=600,600)

## Backing up the PGP Key-pair

It is important to create a backup of the keys. It ensures that you can restore the key-pair and access the previously encrypted emails in case your computer is destroyed or gets stolen.

* Right-click on the key-pair and select _'Export Secret Keys...'_

![Exporting Secret Key](kleopatra-export-secret-keys.png?lightbox=1024&cropResize=600,600)

* Enter a filename and path for the backup. Tick the _'ASCII armor'_ box.

![Exporting Secret Key](kleopatra-export-secret-keys-2.png?lightbox=1024&cropResize=600,600)

![Exporting Secret Key](kleopatra-export-secret-keys-3.png?lightbox=1024&cropResize=600,600)

* If everything did go well, the backup secret key should be saved into a file.

Now back up the public key

* Right-click on the key-pair and select _'Export Certificates ...'_

![Exporting Public Key](kleopatra-export-public-keys-1.png?lightbox=1024&cropResize=600,600)

![Exporting Public Key](kleopatra-export-public-keys-2.png?lightbox=1024&cropResize=600,600)

Now take both files (public and the private key) and copy them to an offsite location. It can be an external USB drive, a Dropbox folder or you can even print it out on a piece of paper! 

!!! It is safe to store the private key elsewhere, because the private key is encrypted as we set a strong passphrase on it earlier. In other words, the secret key cannot be retrieved without entering the passphrase first.

Go to the [following step for setting up Thunderbird](../setting-up-thunderbird-and-pgp) for sending and receiving encrypted emails with PGP.
