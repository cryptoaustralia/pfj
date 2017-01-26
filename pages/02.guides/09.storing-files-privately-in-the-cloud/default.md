---
title: 'Storing Files Privately in the Cloud'
metadata:
    author: 'Gabor Szathmari'
    description: 'Not every cloud-based file storage are made equal. Learn to install sync.com that keeps your files private from the prying eyes.'
    'og:title': 'Storing Files Privately in the Cloud'
    'og:type': article
    'og:description': 'Not every cloud-based file storage are made equal. Learn to install sync.com to keep your files private from the prying eyes.'
    'og:image': 'https://privacyforjournalists.org.au/user/pages/02.guides/09.storing-files-privately-in-the-cloud/social-facebook.png'
    'twitter:card': summary_large_image
    'twitter:site': '@PrivacyJournAU'
    'twitter:creator': '@gszathmari'
    'twitter:title': 'Storing Files Privately in the Cloud'
    'twitter:description': 'Not every cloud-based file storage are made equal. Learn to install sync.com that keeps your files private from the prying eyes.'
    'twitter:image': 'https://privacyforjournalists.org.au/user/pages/02.guides/09.storing-files-privately-in-the-cloud/social-twitter.png'
taxonomy:
    tag:
        - windows
        - storage
        - 'end-to-end encryption'
---

# Storing Files Privately in the Cloud

[TOC]

Not every cloud-based file storage solutions are made equal. Although almost each of them uses encryption to transmit and store your files, the devil is in the details. 

Popular file storage services - such as Dropbox and Microsoft OneDrive - have access to the file decryption keys. In other words, their staff can and do access your files for things like [detecting pirated media](http://www.wired.co.uk/article/dropbox-dmca-position?target=_blank) in your folders, or [fulfiling law encforcement requests](#services-without-zero-knowledge-...) when being served with a warrant.

Fortunately, zero-knowledge, end-to-end encryption solves this problem. Your files are encrypted on your computer with an encryption key, before the files are uploaded to the cloud. As the key never leaves your computer, neither the cloud provider nor anyone else may access your files.

## Instructions

The following sections will walk you through the registration and configuration process of [sync.com](https://www.sync.com/?target=_blank). It is an easy-to-use, zero-knowledge file storage solution that keeps your files secure and private.

### Registering an Account

* Visit [sync.com](https://www.sync.com/?target=_blank) and click on the **Free signup** button on the top-right corner

![](sync_main_page.PNG?lightbox&cropResize=800,800)

* Enter your email address and a strong password

![](registering_an_account.PNG?lightbox&cropResize=800,800)

* The account is now ready to use. You should receive a welcome email in your mailbox. Confirm your email address by clicking on the link in that email.

![](registration_complete.PNG?lightbox&cropResize=800,800)

### Setting up the Desktop Client

You can synchornise the contents of a folder on your hard drive with sync.com by installing the client software.

* Navigate to the [download site](https://www.sync.com/install/?target=_blank)

![](downloading_client_1.PNG?lightbox&cropResize=800,800)

* Once the file is downloaded, run it to install the client. Choose the second option and click **Next**

![](logging_into_the_client_1.PNG?lightbox&cropResize=800,800)

* Enter your username and password

![](logging_into_the_client_2.PNG?lightbox&cropResize=800,800)

* Modify the location of the synchorised folder if needed. By default, the installer will create a new folder under **Documents** with the name **Sync**.

![](configuring_client_1.PNG?lightbox&cropResize=800,800)

* Untick the **Send error and debug messages to Sync** and click **Finish** to close the installer

![](configuring_client_2.PNG?lightbox&cropResize=800,800)

* A small icon next to the clock should appear, which shows that the app is running

![](syncing_a_file_1.PNG?lightbox&cropResize=800,800)

### Syncing the First File

Now open the **Sync** folder under your **Documents** folder and drag a file here

![](syncing_a_file_2.PNG?lightbox&cropResize=800,800)

### Accessing Your Files on the Web

* Visit sync.com again and now click on the **Log in** button on the top

![](sync_main_page.PNG?lightbox&cropResize=800,800)

* Enter your username and password

![](web_ui_1.PNG?lightbox&cropResize=800,800)

* Your previously syncronised document should appear on the web interface

![](web_ui_2.PNG?lightbox&cropResize=800,800)

### Enabling Two-factor Authentication

It is always a good idea to protect your important user accounts with two-factor authentication, in case your password is stolen by a [backdoor on your computer](../protect-your-pc-from-backdoors-windows).

In order to make this work, you must have **Google Authenticator** ([Android](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2?target=_blank), [iPhone](https://itunes.apple.com/us/app/google-authenticator/id388497605?target=_blank)) installed on your smartphone.

* While still on the web panel, click on your email address on the top-right menu. Select **Account Settings** from the drop-down menu.

![](configure_2fa_1.PNG?lightbox&cropResize=800,800)

* Click the **Security** tab and select **Enable 2-FA via Google Authenticator**

![](configure_2fa_2.PNG?lightbox&cropResize=800,800)

* Scan the QR code with the Google Authenticator app on your smartphone. Enter the 6 digit PIN and select **Save**.

![](configure_2fa_3.PNG?lightbox&cropResize=800,800)

![](logging_in_with_2fa_1.PNG?lightbox&cropResize=800,800)

* One two-factor authentication is enabled, you will need to provide the 6 digit code from your smartphone when logging into the web panel again.

![](web_ui_1.PNG?lightbox&cropResize=800,800)

![](logging_in_with_2fa_2.PNG?lightbox&cropResize=800,800)

## Alternative Zero-Knowledge Services

* [SpiderOak One](https://spideroak.com/solutions/spideroak-one?target=_blank)
* [Tresorit](https://tresorit.com/?target=_blank)
* [Boxcryptor](https://www.boxcryptor.com/en?target=_blank) - Bolt-on zero-knowledge encryption to Dropbox, OneDrive, Google Drive and Box
* [Resilio](https://www.getsync.com/?target=_blank) - Sync between your devices without a middle-man in the cloud

### Services without Zero-Knowledge Encryption

The following cloud-based file storage solutions are **not** zero-knowledge solutions. Many of them are known to satisfy law enforcement requests as confirmed by the published transparency reports.

* **Dropbox** - [Transparency Report](https://www.dropbox.com/transparency?target=_blank)
* **Microsoft OneDrive** - [Law Enforcement Requests Report](https://www.microsoft.com/about/csr/transparencyhub/lerr/?target=_blank)
* **Google Drive** - [Transparency Report](https://www.google.com/transparencyreport/userdatarequests/AU/?target=_blank)
* **Box**
* **iCloud** - [Government Information Requests](https://www.apple.com/au/privacy/government-information-requests/?target=_blank)

## Further Reading

* [Sync.com Privacy White Paper](https://www.sync.com/pdf/sync-privacy.pdf) 
* [Comparison of online backup services](https://en.wikipedia.org/wiki/Comparison_of_online_backup_services?target=_blank)
* [What is Zero-Knowledge Encryption?](https://tresorit.com/blog/zero-knowledge-encryption/)
* [Fabian M. Suchanek's review of sync.com](https://suchanek.name/texts/reviews/tresorit.html#sync)

_Image courtesy of [Alex Weber](https://www.flickr.com/photos/8123185@N02/3659676928/in/photolist-6zoNs5-kqF23b-E2idm-nmDgh6-8nVMLr-bkL8-i532Po-nmmFK5-4PBfbk-nmmTJV-irVU66-8eMHsK-o54g8R-EQ8MR-cZyLWY-p6b1ry-d363cw-6rZYic-6eLY3J-6FhrpX-aPLo64-bUGofJ-8612dY-fBBjbK-6nBi8g-C8YWQ-fxnRxA-6u1S61-mA679z-4BmBJc-pnxSs-fpWeFp-5ucGwU-8qhkUt-dY2oAN-ffJZqK-5gueQb-5KD4i1-cpSFgN-4EjNsR-6gpV7j-5MDZUX-5fmatB-d36395-573CHc-3FZSQ2-aad8bn-mA5bdZ-7DiA7z-7R8x6j?rel=nofollow)_