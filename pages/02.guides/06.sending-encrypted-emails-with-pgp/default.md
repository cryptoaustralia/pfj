---
title: 'Sending Encrypted Emails With PGP'
metadata:
    'author': 'Gabor Szathmari'
    'description': 'The last part of the series helps you with sending and receiving your first encrypted email'
    'og:title': 'Sending Encrypted Emails With PGP'
    'og:type': article
    'og:description': 'The last part of the series helps you with sending and receiving your first encrypted email'
    'og:image': https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png
    'twitter:card': 'summary_large_image'
    'twitter:site': @PrivacyJournAU
    'twitter:creator': @gszathmari
    'twitter:title': 'Sending Encrypted Emails With PGP'
    'twitter:description': 'The last part of the series helps you with sending and receiving your first encrypted email'
    'twitter:image': https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png
taxonomy:
    category:
        - pgp
    tag:
        - windows
---

# Sending Encrypted Emails With PGP

The final step is importing someone else's public key so we can send them encrypted emails. At the end of this guide, you will be able to send an encrypted email to someone else.

## Retrieve Someone's Public Key

The first step is retrieving someone else's public key from the Internet. In my case, I am downloading the key from **https://keybase.io/gszathmari/key.asc**

![Retrieve Public Key](retrieve-public-key.png?lightbox=1024&cropResize=600,600)

* Save the public key into a text file

![Save Public Key](save-public-key-in-text-file.png?lightbox=1024&cropResize=600,600)

* Open **Kleopatra** and click on the _'Import Certificates'_ button

![Kleopatra Import Certificates](kleopatra-main-window.png?lightbox=1024&cropResize=600,600)

* Select the text file we saved earlier

![Kleopatra Select Public Key](kleopatra-import-public-key.png?lightbox=1024&cropResize=600,600)

![Kleopatra Select Public Key](kleopatra-import-successful.png?lightbox=1024&cropResize=600,600)

* Now go back to the main window of **Kleopatra** and make sure you have the _'Imported Certificates'_ tab open

![Kleopatra Imported Certificates](kleopatra-main-window-2.png?lightbox=1024&cropResize=600,600)

* Double-click the certificate to open its preferences. Select _'Trust Certifications Made by This Certificate ...'_

![Kleopatra Trusts](kleopatra-key-properties.png?lightbox=1024&cropResize=600,600)

* Change the trust level from _'I do not know'_ to _'I believe checks are casual'_

![Kleopatra Change Trust Level](kleopatra-set-trust-level.png?lightbox=1024&cropResize=600,600)

![Kleopatra Change Trust Level](kleopatra-set-trust-level-1.png?lightbox=1024&cropResize=600,600)

![Kleopatra Change Trust Level](kleopatra-set-trust-level-2.png?lightbox=1024&cropResize=600,600)

## Write an Encrypted Email

As you now have the recipient's public key, you can write the first encrypted email to them!

* Write an email as usual and click on the padlock on the top to encrypt the email

![Kleopatra Change Trust Level](thunderbird-encrypt-email.png?lightbox=1024&cropResize=600,600)

* You are required to enter your passphrase before the email is encrypted and sent

![Kleopatra Change Trust Level](thunderbird-encrypt-email-2.png?lightbox=1024&cropResize=600,600)

* The email should be successfully sent in an encrypted format. The raw email should be looking like the following.

![The Encrypted Email](encrypted-email.png?lightbox=1024&cropResize=600,600)

* You recipient will have the following indicators if they have your public key imported

![Email Recipient](recipient-side-2.png?lightbox=1024&cropResize=600,600)

* If your partner does not have your public key imported, they are still able to open and read the encrypted email

![Email Recipient](recipient-side-1.png?lightbox=1024&cropResize=600,600)

Well done! You are ready to send and receive encrypted emails

! Keep in mind that metadata is retained for 2 years in Australia. It means that the IP addresses, the size of the message (attachments!), the sender and the recipient's email addresses will all be stored. **In other words, you can be linked to your information sources.** If you metadata is a concern for you, check out our other guides.
