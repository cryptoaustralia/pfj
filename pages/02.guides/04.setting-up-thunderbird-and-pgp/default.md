---
title: 'Setting up Thunderbird and PGP'
metadata:
    'author': 'Gabor Szathmari'
    'description': 'The second part of the series guides you to install and configure Mozilla Thunderbird as a mailer for sending and receiving encrypted emails'
    'og:title': 'Setting up Thunderbird and PGP'
    'og:type': article
    'og:description': 'The second part of the series guides you to install and configure Mozilla Thunderbird as a mailer for sending and receiving encrypted emails'
    'og:image': https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png
    'twitter:card': 'summary_large_image'
    'twitter:site': @PrivacyJournAU
    'twitter:creator': @gszathmari
    'twitter:title': 'Setting up Thunderbird and PGP'
    'twitter:description': 'The second part of the series guides you to install and configure Mozilla Thunderbird as a mailer for sending and receiving encrypted emails'
    'twitter:image': https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png
taxonomy:
    category:
        - pgp
    tag:
        - windows
---

# Setting up Thunderbird and PGP

[TOC]

Once you finished [setting up your PGP keys](../generating-pgp-keys-windows), we need to configure an emailer application to fully utilise PGP. 

At the end of this guide, you will be able to send and receive encrypted emails.

## Installing Mozilla Thunderbird

* Navigate your browser to [https://www.mozilla.org/en-GB/thunderbird/](https://www.mozilla.org/en-GB/thunderbird/) to download Mozilla Thunderbird

![Mozilla Thunderbird home page](thunderbird-home.png?lightbox=1024&cropResize=600,600)

* Run the downloaded installer and install the application

![Installing Mozilla Thunderbird](thunderbird-install-1.png?lightbox=1024&cropResize=600,600)

![Installing Mozilla Thunderbird](thunderbird-install-2.png?lightbox=1024&cropResize=600,600)

![Installing Mozilla Thunderbird](thunderbird-install-2.png?lightbox=1024&cropResize=600,600)

![Installing Mozilla Thunderbird](thunderbird-install-2.png?lightbox=1024&cropResize=600,600)

## Configuring Mozilla Thunderbird

Once Thunderbird is installed, click on its icon to launch it. You will have to provide various details of your email provider. Please refer to your provider's documentation for the recommended IMAP and SMTP settings.

* Thunderbird should launch with a Configuration Wizard. Select _'Skip this and use my existing email'_ option.

![Mozilla Thunderbird Configuration Wizard](thunderbird-configure-1.png?lightbox=1024&cropResize=600,600)

* A window should pop up where you can enter your email address and password. Thunderbird will try to guess the required settings.

![Mozilla Thunderbird Configuration Wizard](thunderbird-configure-a.png?lightbox=1024&cropResize=600,600)

* If it does not succeed, you have to enter the configuration parameters manually. In my case I had to enter the depicted details.

![Mozilla Thunderbird Configuration Wizard](thunderbird-configure-2.png?lightbox=1024&cropResize=600,600)

* If everything was correct, Thunderbird should be able to connect to your mailbox and retrieve your emails.

![Mozilla Thunderbird Configuration Wizard](thunderbird-configure-3.png?lightbox=1024&cropResize=600,600)

## Setting up Enigmail

Enigmail is an extension you need to install that "glues" Thunderbird and Gpg4Win together.

* Click on the hamburger icon on the top-right corner first and select _'Add-ons'_

![Opening Thunderbird Add-ons](enigmail-configure-1.png?lightbox=1024&cropResize=600,600)

* Enter _'Enigmail'_ into the search box and press Enter. The first result should be the Enigmail plugin. Click in _'Install'_

![Opening Thunderbird Add-ons](enigmail-configure-2.png?lightbox=1024&cropResize=600,600)

![Installing Enigmail](enigmail-configure-3.png?lightbox=1024&cropResize=600,600)

* Once Enigmail is installed, click on _'Restart Now'_ to activate the plugin

![Installing Enigmail](enigmail-configure-4.png?lightbox=1024&cropResize=600,600)

* When Thunderbird is running again, Enigmail should greet with a configuration wizard. Click _'Next'_ on the first screen.

![Enigmail Wizard](enigmail-wizard-1.png?lightbox=1024&cropResize=600,600)

* Leave on the basic settings and click _'Next'_ again

![Enigmail Wizard](enigmail-wizard-2.png?lightbox=1024&cropResize=600,600)

* The following page should list the PGP key-pair we created earlier. Make sure the correct key is highlighted then click _'Next'_

![Enigmail Wizard](enigmail-wizard-3.png?lightbox=1024&cropResize=600,600)

![Enigmail Wizard](enigmail-wizard-4.png?lightbox=1024&cropResize=600,600)

## Testing PGP

To test if everything works correctly, we send a digitally signed (not encrypted) email.

* Write a new email as usual. Press the pencil icon on the new Enigmail toolbar to sign your message then click _'Send'_

![New Signed Email](thunderbird-signed-1.png?lightbox=1024&cropResize=600,600)

* Enter your passphrase to sign the message

![New Signed Email](thunderbird-signed-2.png?lightbox=1024&cropResize=600,600)

* The recipient's email client will indicate that the message has been digitally signed

![Signed Email at Recipient](thunderbird-signed-3.png?lightbox=1024&cropResize=600,600)

!!! The recipient has to import your public key into his/her email client to verify the authenticity of the digital signature

In the next section, we will publish our public key on the Internet so others can verify our digitally signed emails and send us encrypted messages
