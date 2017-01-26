---
title: 'Publishing the Public Key on the Internet'
metadata:
    'author': 'Gabor Szathmari'
    'description': 'The third part of the series shows how you can publish your public key on the Internet including your Twitter account'
    'og:title': 'Publishing the Public Key on the Internet'
    'og:type': article
    'og:description': 'The third part of the series shows how you can publish your public key on the Internet including your Twitter account'
    'og:image': https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png
    'twitter:card': 'summary_large_image'
    'twitter:site': @PrivacyJournAU
    'twitter:creator': @gszathmari
    'twitter:title': 'Publishing the Public Key on the Internet'
    'twitter:description': 'The third part of the series shows how you can publish your public key on the Internet including your Twitter account'
    'twitter:image': https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png
taxonomy:
    category:
        - pgp
    tag:
        - windows
---

# Publishing the Public Key on the Internet

[TOC]

The following step is uploading your PGP public key to a public location, so others will be able to send you encrypted messages. Also, we need to publicise the download URL, so others will be able to find and verify your key easily.

At the end of this guide, you will have your PGP key publicly available on the Internet. In addition, your Twitter profile and email signature will both feature the public URL pointing to your public key.

## Exporting the PGP Fingerprint

The first step is exporting the fingerprint of your PGP key. The fingerprint allows anyone to verify the authenticity of your published public PGP key.

* Open **Kleopatra** from the Start menu

![Kleopatra Main Window](kleopatra-main-window.png?lightbox=1024&cropResize=600,600)

* Right-click your key-pair and select _'Certificate Details'_

![Kleopatra Getting Info](kleopatra-getting-info.png?lightbox=1024&cropResize=600,600)

* Select your fingerprint (the long string of characters and numbers) and copy it onto the pasteboard

![Copy Fingerprint to Pasteboard](kleopatra-copy-fingerprint.png?lightbox=1024&cropResize=600,600)

* Open **Notepad** and paste the string there

![Fingerprint in Notepad](notepad-copy-paste-fingerprint-no-spaces.png?lightbox=1024&cropResize=600,600)

* Add some extra spaces after every fourth character to make the fingerprint more readable

![Fingerprint in Notepad](notepad-copy-paste-fingerprint.png?lightbox=1024&cropResize=600,600)

## Exporting the PGP Public Key

Although we already exported the public key in an earlier guide, but I detail these steps for the sake of completeness. Feel free to jump to the next section if your public key is already exported.

* Now go back to **Kleopatra** and right-click the key again. Select _'Export Certificates'_ and save your public key on the desktop.

![Public Key in Notepad](kleopatra-export-public-key-1.png?lightbox=1024&cropResize=600,600)

![Public Key in Notepad](kleopatra-export-public-key-2.png?lightbox=1024&cropResize=600,600)

## Upload PGP Public Key to Public Keyserver

The following steps detail how you can upload the public key to a public server. Your sources will be able to retrieve your public key from these servers.

* Open the PGP public key we exported earlier with **Notepad**

![Public Key in Notepad](kleopatra-export-public-key-3.png?lightbox=1024&cropResize=600,600)

* Visit [https://sks-keyservers.net/i](https://sks-keyservers.net/i). Select the _'Submit a Key to the Server'_ option.

![SKS Website](sks-upload-public-key-1.png?lightbox=1024&cropResize=600,600)

* Paste the public key from Notepad into the box as shown. Click on the _'Submit this key to the keyserver!'_ button.

![SKS Paste Public Key](sks-upload-public-key-2.png?lightbox=1024&cropResize=600,600)

* If everything did go well, you should see the following message

![SKS Upload Successful](sks-upload-public-key-3.png?lightbox=1024&cropResize=600,600)

## Verify your PGP Public Key on the Public Keyserver

Wait a few minutes before you move on to the following steps. We will extract the URL where your information sources can retrieve your public key.

* Visit [https://sks-keyservers.net/i](https://sks-keyservers.net/i) again and now select the _'Extract a Key from the Server'_ option. Enter your email address in the search box.

![SKS Search for PGP Public Key by Email](sks-verify-public-key-1.png?lightbox=1024&cropResize=600,600)

* Your PGP key should be listed on the results page. Verify whether the fingerprints match with the one in **Kleopatra**

![SKS Search Results](sks-verify-public-key-2.png?lightbox=1024&cropResize=600,600)

* Click on the link on the results page, which should retrieve the full public key

![SKS Retrieve Public Key](sks-verify-public-key-3.png?lightbox=1024&cropResize=600,600)

Copy the URL from the URL bar (**https://sks-keyservers.net/pks/lookup?op=get&search=0x72975CBAC94D4ED5** in my case)

## Publishing Download URL and Fingerprint on Twitter

Visit your Twitter profile to publish the URL and the fingerprint in your Twitter Bio.

* Add the URL to the Bio as shown first

![Twitter Add URL to Bio](twatter-add-sks-url.png?lightbox=1024&cropResize=600,600)

* Now copy the last 16 digits of your fingerprint and add them to the Bio as well

![Twitter Add Fingerprint to Bio](twatter-add-fingerprint.png?lightbox=1024&cropResize=600,600)

* Save the results, your Twitter profile now should feature the necessary details to retrieve and verify your PGP public key

![Twitter URL and Fingerprint in Bio](twatter-finished-result.png?lightbox=1024&cropResize=600,600)

![Twitter URL and Fingerprint in Bio](twatter-published-profile.png?lightbox=1024&cropResize=600,600)

## Publishing Download URL and Fingerprint in your Email Signature

Edit your email signature to feature both the download URL and your PGP fingerprint. In my case, I added them to Thunderbird.

![Thunderbird Email Signature](thunderbird-signature.png?lightbox=1024&cropResize=600,600)

## Publishing Download URL and Fingerprint Elsewhere

Feel free to publish the URL and the fingerprint at the end of your articles, so your readers will know how to contact you in a secure manner.
