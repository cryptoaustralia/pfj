---
title: 'Protect Your PC from Backdoors'
published: true
metadata:
    author: 'Gabor Szathmari'
    description: 'Installing anti-malware and anti-exploit software to protect your sources from sneaky backdoors on your PC'
    'og:title': 'Protect Your PC from Backdoors'
    'og:type': article
    'og:description': 'Installing anti-malware and anti-exploit software to protect your sources from sneaky backdoors on your PC'
    'og:image': 'https://privacyforjournalists.org.au/user/pages/02.guides/protect-your-pc-from-backdoors-windows/backdoor-social-image.png'
    'twitter:card': summary_large_image
    'twitter:site': '@PrivacyJournAU'
    'twitter:creator': '@gszathmari'
    'twitter:title': 'Protect Your PC from Backdoors'
    'twitter:description': 'Installing anti-malware and anti-exploit software to protect your sources from sneaky backdoors on your PC'
    'twitter:image': 'https://privacyforjournalists.org.au/user/pages/02.guides/protect-your-pc-from-backdoors-windows/backdoor-social-image.png'
taxonomy:
    tag:
        - windows
        - malware
        - backdoor
        - exploit
        - virus
visible: true
---

# Protect Your PC from Backdoors

[TOC]

One method to monitor your activities online as well as your computer is backdoors on your computer.

Software backdoors typically run hidden in the background. They are capable of carrying out the following activities:

* Keystroke logging
* Turning the microphone and camera on
* Taking screenshots of your desktop
* Downloading files from your computer

It is clear from the list that once your computer is compromised with a backdoor, your activity is not secret anymore. It does not matter if you are encrypting your emails with PGP, if your adversary can simply take screenshots of your emails while they are open on the screen.

## How Adversaries Deploy their Backdoors?

It depends on the adversary, but they can utilise one of the following methods:
* **Phishing emails** such as a fake FedEx package notification with a URL pointing to a browser exploit
* **Phishing emails** with a file attachment. For instance, the email is claiming you received an invoice and a PDF file is attached.
* **Phishing emails** with a URL pointing to a malicious file. Same as above, but the file is not attached but downloaded separately.
* **Malvertising**: Browser exploits hidden into advertising banners. The malware is activated if your browser, or its plugins (Java, Flash, Silverlight) are outdated.
* **Drive-by downloads**: Your browser unexpectedly downloads a file claiming it is something important, such as an Adobe Flash update

### Miscellenaous

In addition, law enforcement agencies have additional capabilities to compromise your computer, such as:
* They can inject various browser exploits into your normal web browsing traffic at your Internet Service Provider
* Various agencies may enter your home secretly with a warrant, and tamper with your computer while you are not home

## How Can I Protect Myself?

The bad news is that state sponsored attacks will probably succeed. Well-funded organisations have the budget as well as the talent to develop exploits that will compromise your computer even with all precautions. One type of precaution is to compartmentalize your work in order to limit the damage. 

However, you should still install anti-malware and anti-exploit software on your PC. Both of them have certain capabilities to block unknown and advanced malicious software your adversary may utilise to compromise your PC.

!! Keep in mind that these products can only protect you before any malicious software is installed. If you suspect your computer is compromised, wipe it clean and reinstall everything from a clean media.

### Choosing an Anti-Malware Product

Modern anti-malware (or anti-virus) software sport many advanced features to protect your PC from malicious software to be installed. These capabilities include:
* The detection and blocking of **known** malicious software from running
* The detection and blocking of **unknown** malicious software from running
* Keylogging protection
* Application whitelisting
* System vulnerability scanner

Based on the reports ([1](https://www.mrg-effitas.com/wp-content/uploads/2016/05/MRG-Effitas-360-Assessment-Q1-2016.pdf?target=_blank), [2](http://chart.av-comparatives.org/chart1.php?chart=chart2&year=2016&month=5&sort=1&zoom=3)) of two indendent anti-malware testing companies, we endorse Kaspersky Internet Security. 

! The product is not free, however we are not affiliated with the company in any way

#### Installing Kaspersky Internet Security

* Head on to the website of Kaspersky trials on [www.kaspersky.com/au/trials](http://www.kaspersky.com/au/trials?target=_blank) and select **Kaspersky Internet Security** or **Kaspersky Total Security** from the product list

![](kaspersky-download-1.png?lightbox=1024&cropResize=600,600)

![](kaspersky-download-2.png?lightbox=1024&cropResize=600,600)

* Once the installer is downloaded, run it and follow the instructions. Make sure the participation in _Kaspersky Security Network (KSN)_ box is ticked.

![](kaspersky-install-1.png?lightbox=1024&cropResize=600,600)

![](kaspersky-install-2.png?lightbox=1024&cropResize=600,600)

![](kaspersky-install-3.png?lightbox=1024&cropResize=600,600)

* Please note you have to buy the product after 30 days. Select 'Activate as a trial version of the application' for now.

![](kaspersky-install-4.png?lightbox=1024&cropResize=600,600)

![](kaspersky-install-5.png?lightbox=1024&cropResize=600,600)

Once Kaspersky is installed, the main window should pop up. All is good, but we need to fine tune the application.

![](kaspersky-conf-1.png?lightbox=1024&cropResize=600,600)

* Press the green 'More Tools' button in the middle, which should bring up another screen

![](kaspersky-conf-2.png?lightbox=1024&cropResize=600,600)

* Click on the 'Trusted Applications mode' to configure application whitelisting. The list of trusted applications [is provided by the Kaspersky Security Network](http://support.kaspersky.com/12034?cid=KTS_16.0). More information is available [here](http://media.kaspersky.com/pdf/kaspersky_lab_whitepaper_trusted_applications_mode.pdf).

!!! Application whitelisting is an effective technique that blocks malicious software from running if it has not been seen before. Backdoors tailored against you typically fall into this category. This technique is recommended by many organisations including the [Australian Signals Directorate](http://www.asd.gov.au/publications/protect/top_4_mitigations.htm?rel=noreferrer&target=_blank)) 

![](kaspersky-conf-3.png?lightbox=1024&cropResize=600,600)

* Click on the 'Enable' button. Once it is on, you should see the following screen.

![](kaspersky-conf-4.png?lightbox=1024&cropResize=600,600)

* Now go back to the main menu with the 'Back' button in the top-left corner

![](kaspersky-conf-2.png?lightbox=1024&cropResize=600,600)

* Click on 'Vulnerability Scan'

![](kaspersky-conf-5.png?lightbox=1024&cropResize=600,600)

* Click on 'Run scan' and wait the test to finish. You should see results like the following.

![](kaspersky-conf-6.png?lightbox=1024&cropResize=600,600)

* Select items related to 'Autorun' and press the 'Fix' button

![](kaspersky-conf-7.png?lightbox=1024&cropResize=600,600)

* Now go to the main menu with the 'Back' button again

![](kaspersky-conf-2.png?lightbox=1024&cropResize=600,600)

* Select 'Cloud Protection'. Verify whether you are connected with the Kaspersky Security Network. The green button on the left should display 'Connected'

![](kaspersky-conf-8.png?lightbox=1024&cropResize=600,600)

Your PC is reasonably protected now from both known and unknown malicious software. Keep Kaspersky running in the background all time, and buy the licence before the trial expires.

! Kaspersky may flag Ricochet as malicious. This is a [known problem](https://github.com/ricochet-im/ricochet/issues/424?target=_blank) and you may ignore the warning as it is a false positive. Locate the 'K' icon next to the clock in the bottom-right corner and select 'Pause protection...' while [installing Ricochet](../guides/secure-chat-without-leaving-metadata-ricochet).

### Choosing an Anti-exploit Product

The other major threat to your computer is browser exploits. If your browser or one of its plugins (such as Adobe Flash) is outdated or vulnerable, the adversary can exploit that to deploy their backdoor software.

Anti-exploit kits are special tools that protects your PC from these types of attacks. It is a great companion to your anti-malware product providing an additional layer of defense.

Based on an [independent test](https://www.mrg-effitas.com/wp-content/uploads/2015/04/MRG_Effitas_Real_world_exploit_prevention_test.pdf?target=_blank), we recommend the product named **HitmanPro.Alert**.

! The product is not free, however we are not affiliated with the company in any way

#### Installing HitmanPro.Alert

* Navigate your browser to [www.surfright.nl/en/products](http://www.surfright.nl/en/products?target=_blank)

![](hitman-download-1.png?lightbox=1024&cropResize=600,600)

* Scroll down to the bottom and download **HitmanPro.Alert** (the one on the right side)

![](hitman-download-2.png?lightbox=1024&cropResize=600,600)

* Run the installer and follow the instructions

![](hitman-install-1.png?lightbox=1024&cropResize=600,600)

![](hitman-install-2.png?lightbox=1024&cropResize=600,600)

![](hitman-install-3.png?lightbox=1024&cropResize=600,600)

* When the installation is complete, run your favourite web browser. A message should pop up on the top-right corner indicating that your browser now is protected.

![](hitman-run-1.png?lightbox=1024&cropResize=600,600)

Now your browser is reasonably protected from browser exploits. The software should be running at all time in the background.

! Remember, these software are not bulletproof and will not provide protection from a determined, well-funded adversary. Check out our [guides](/guides) for other safe practices such as compartmentalization.

_Photo courtesy of [Karol Franks](https://www.flickr.com/photos/karolfranks/3930087897/?rel=nofollow)_