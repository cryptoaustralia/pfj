---
title: 'Secure File Exchange With OnionShare'
metadata:
    author: 'Gabor Szathmari'
    description: 'This walkthrough guides you through the installation process of OnionShare that shares files in an ad-hoc manner without leaving metadata'
    'og:title': 'Secure File Exchange With OnionShare'
    'og:type': article
    'og:description': 'This walkthrough guides you through the installation process of OnionShare that shares files in an ad-hoc manner without leaving metadata'
    'og:image': 'https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png'
    'twitter:card': summary_large_image
    'twitter:site': '@PrivacyJournAU'
    'twitter:creator': '@gszathmari'
    'twitter:title': 'Secure File Exchange With OnionShare'
    'twitter:description': 'This walkthrough guides you through the installation process of OnionShare that shares files in an ad-hoc manner without leaving metadata'
    'twitter:image': 'https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png'
taxonomy:
    category:
        - 'file exchange'
    tag:
        - windows
        - 'no metadata'
---

## Secure File Exchange With OnionShare

[TOC]

Every time a file is exchanged over the Internet via services like emails, Dropbox or file transfer features of instant messaging applications, metadata is left all over the place that can link the journalist and its information source together.

[OnionShare](https://onionshare.org?target=_blank) has been developed to simplify ad-hoc file exchanges while it leaves as little metadata as possible. It operates over Tor and connects the two parties together without any central server in the middle. This means that once a file is transferred and the application is closed, there are no logs left behind at the ISP or any service provider.

At the end of this guide, you will be able to use OnionShare to share files in a secure manner. Also, you will be able to download files shared with OnionShare.

## Getting OnionShare

* Visit [https://onionshare.org](https://onionshare.org?target=_blank) to download the latest version

![OnionShare Home Page](download-onionshare.png?lightbox=1024&cropResize=600,600)

* Install **OnionShare** as any other application

![Installing OnionShare](install-onionshare-1.png?lightbox=1024&cropResize=600,600)

![Installing OnionShare](install-onionshare-2.png?lightbox=1024&cropResize=600,600)

![Installing OnionShare](install-onionshare-3.png?lightbox=1024&cropResize=600,600)

## Installing Tor Browser

OnionShare requires the **Tor Browser** installed and running. Follow the instructions below to download and install it.

* Download **Tor Browser** from the website of [Tor Project](https://www.torproject.org/projects/torbrowser.html.en?target=_blank)

![Downloading Tor Browser](download-tor-browser-1.png?lightbox=1024&cropResize=600,600)

![Downloading Tor Browser](download-tor-browser-2.png?lightbox=1024&cropResize=600,600)

* Install **Tor Browser** as the following

![Installing Tor Browser](install-tor-browser-1.png?lightbox=1024&cropResize=600,600)

![Installing Tor Browser](install-tor-browser-2.png?lightbox=1024&cropResize=600,600)

![Installing Tor Browser](install-tor-browser-3.png?lightbox=1024&cropResize=600,600)

![Installing Tor Browser](install-tor-browser-4.png?lightbox=1024&cropResize=600,600)

## Running the Tor Browser

* Now launch the **Tor Browser** and leave it running in the background

![Running Tor Browser](tor-connect-1.png?lightbox=1024&cropResize=600,600)

![Running Tor Browser](tor-connect-2.png?lightbox=1024&cropResize=600,600)

![Running Tor Browser](tor-connect-3.png?lightbox=1024&cropResize=600,600)

## Sharing a File with OnionShare

While the **Tor Browser** is still running in the background, launch **OnionShare** to share a dummy file named _'Super Secret File.txt') over the Tor network

* Run **OnionShare** first

![Sharing a File with OnionShare](onionshare-share-file-1.png?lightbox=1024&cropResize=600,600)

* Drag the file (or files) to the main window of **OnionShare**

![Sharing a File with OnionShare](onionshare-share-file-2.png?lightbox=1024&cropResize=600,600)

* Now press the _'Start Sharing'_ button. It takes some time before the file becomes available on Tor.

![Sharing a File with OnionShare](onionshare-share-file-3.png?lightbox=1024&cropResize=600,600)

* Once the file is available, the indicator turns green and a link appears

![Sharing a File with OnionShare](onionshare-share-file-4.png?lightbox=1024&cropResize=600,600)

The shared file is now available on a secret URL. This URL will not work in normal browsers, so the other party must use the **Tor Browser** to access the file.

!!! Share the secret link securely with your partner via encrypted chat or email

## Downloading Files Shared with OnionShare

The following section details how the other party can download the shared file with the secret link

* Run the **Tor Browser**

![Downloading a File with the Tor Browser](tor-download-file-1.png?lightbox=1024&cropResize=600,600)

* Enter the secret URL in the URL bar

![Downloading a File with the Tor Browser](tor-download-file-2.png?lightbox=1024&cropResize=600,600)

* Save the file to the hard disk

![Downloading a File with the Tor Browser](tor-download-file-3.png?lightbox=1024&cropResize=600,600)

![Downloading a File with the Tor Browser](tor-download-file-4.png?lightbox=1024&cropResize=600,600)

![Downloading a File with the Tor Browser](tor-download-file-5.png?lightbox=1024&cropResize=600,600)

* Unpack and open the shared file from the hard disk

![Opening the Downloaded File](tor-open-file-1.png?lightbox=1024&cropResize=600,600)

![Opening the Downloaded File](tor-open-file-2.png?lightbox=1024&cropResize=600,600)

![Opening the Downloaded File](tor-open-file-3.png?lightbox=1024&cropResize=600,600)

![Opening the Downloaded File](tor-open-file-4.png?lightbox=1024&cropResize=600,600)

![Opening the Downloaded File](tor-open-file-5.png?lightbox=1024&cropResize=600,600)

* The other party running **OnionShare** is notified when the file has been downloaded

![Shared File is Downloaded](onionshare-share-file-finished.png?lightbox=1024&cropResize=600,600)

! If metadata is a concern of yours, [follow our guide here](../secure-chat-without-leaving-metadata-ricochet) to share the secret URL with a chat application that leaves no traces behind
