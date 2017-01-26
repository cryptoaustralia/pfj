---
title: Threats
metadata:
    author: 'Gabor Szathmari'
    description: 'Threat modeling for journalists to understand what tools they should be using in different scenarios'
    'og:title': 'Threats | Privacy for Journalists'
    'og:type': article
    'og:description': 'Threat modeling for journalists to understand what tools they should be using in different scenarios'
    'og:image': 'https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png'
    'twitter:card': summary_large_image
    'twitter:site': '@PrivacyJournAU'
    'twitter:creator': '@gszathmari'
    'twitter:title': 'Threats | Privacy for Journalists'
    'twitter:description': 'Threat modeling for journalists to understand what tools they should be using in different scenarios'
    'twitter:image': 'https://privacyforjournalists.org.au/user/themes/mytheme/images/social.png'
---

# Threat Modeling

[TOC]

When it comes to the protection of your information sources and the data you already collected, it is paramount to be clear who your adversary is. Depending on the individual or the organisation you are dealing with, their capabilities and willingness varies. Therefore, the tools and practices must match your adversary.

## Advisories and Motives

The selection of the appropriate tools and practices should be based on 'threat modeling'. It is a systematic approach to collect:

1. Who is willing to harm you 
1. What they are after
1. What you can do about it 

Based on this two pieces of information, you can select a set of security and privacy tools, and safe practices to defend yourself and your information source.

## Threat Model for Journalists

The following table attempts to collect the general threat scenarios of a typical journalist in Australia.

!!!! Have some feedback? Feel free to [drop us a line](../community) and we are happy to make corrections

| # | Adversary | What they are after? | What they can do? | How can you defend yourself? |
| -------- | --------- | -------------------- | ----------------- | ---------------------------- |
| **1** | [The Government](https://wiki.privacyforjournalists.org.au/metadata_access) | Name and contact details of a journalist's information sources | Link the journalist and the information source together by using the retained metadata at the ISP and/or service providers | [Link](#scenario-1) |
| **2** | [The Government](https://wiki.privacyforjournalists.org.au/metadata_access) | Name and contact details of a journalist's information sources | Link the journalist and the information source together by targeted surveillance of the journalist | [Link](#scenario-2) |
| **3** | [The Government](https://wiki.privacyforjournalists.org.au/metadata_access) | Name and contact details of a journalist's information sources | Link the journalist and the information source together by seizing the journalist's laptop and mobile phone | [Link](#scenario-3) |
| **4** | [The Government](https://wiki.privacyforjournalists.org.au/metadata_access) | The content of the communication between the journalist and the information source | Monitor the communication on-the-wire with targeted surveillance (a.k.a. wiretapping) | [Link](#scenario-4) |
| **5** | [The Government](https://wiki.privacyforjournalists.org.au/metadata_access) | The content of the communication between the journalist and the information source | Monitor the communication at the journalist's computer using a malware or backdoor (targeted surveillance) | [Link](#scenario-5) |
| **6** | [The Government](https://wiki.privacyforjournalists.org.au/metadata_access) | The content of the communication between the journalist and the information source | Seizing the journalist's devices to read files, chat logs and browsing history from the computer or the mobile phone | [Link](#scenario-6) |
| **7** | Corporate Hacking | Name and contact details of a journalist's information sources. The content of the communication between the journalist and the information source. | Monitor the communication at the journalist's computer using malware or backdoor (targeted surveillance) | [Link](#scenario-7) |
| **8** | Cyber Criminals | The journalist's money, passwords and banking details | Install ransomware or information stealing malware with browser exploits, malicious links or malicious attachments in phishing emails | [Link](#scenario-8) |
| **9** | Casual Eavesdropper | Nothing in particular | Publish any data they stuble upon on things like a lost and found USB drive, or a laptop stolen from the journalist's car | [Link](#scenario-9) |

### Defense Scenarios

The following section details the potential tools and practices matching your threat scenario of the [threat model](#threat-model-for-journalists)

#### Scenario 1

In this scenario, you have to leave as little footprint as possible. Metadata is collected and retained at the ISP and service providers for 2 years. This includes things like email recipients, usernames or dialled phone numbers. For a non-comprehensive list of metadata, refer to the [Attorney-General's Department's Guide](https://www.ag.gov.au/NationalSecurity/DataRetention/Documents/Dataset.pdf?ref=noreferrer) for more details.

The goal of this case is hiding or not leaving as much metadata as possible. Therefore, we recommend using the following tools from [our guides](../guides):

| Use Cases | Recommendations |
| --------- | --------------- |
| Web Browsing | **Using the Tor Browser** _(coming soon)_, **[Choosing a Safe Search Engine](../guides/choosing-a-safe-search-engine)** |
| Email | _Not recommended (even with PGP)_ |
| Instant Messaging | **[Secure Chat With Ricochet](../guides/secure-chat-without-leaving-metadata-ricochet)** |
| Voice Calls | _Tooling doesn't exist_ |
| Video Calls | _Tooling doesn't exist_ |
| Text Messaging (SMS) | _Not recommended_ |
| File Exchange | **[Secure File Exchange With OnionShare](../guides/secure-file-exchange-without-leaving-metadata-onionshare)**, **[Exchanging Files and Messages with GlobaLeaks](../guides/exchanging-files-and-messages-with-globaleaks)** |

#### Scenario 2

In this scenario the Internet traffic and the mobile phone voice and texts of the journalist are actively monitored. The main goal is encrypting the contents of the communication, and leaving as little metadata as possible. 

| Use Cases | Recommendations |
| --------- | --------------- |
| Web Browsing | **Using the Tor Browser** _(coming soon)_ |
| Email | _Not recommended (even with PGP)_ |
| Instant Messaging | **[Secure Chat With Ricochet](../guides/secure-chat-without-leaving-metadata-ricochet)** |
| Voice Calls | _Tooling doesn't exist_ |
| Video Calls | _Tooling doesn't exist_ |
| Text Messaging (SMS) | _Not recommended_ |
| File Exchange | **[Secure File Exchange With OnionShare](../guides/secure-file-exchange-without-leaving-metadata-onionshare)**, **[Exchanging Files and Messages with GlobaLeaks](../guides/exchanging-files-and-messages-with-globaleaks)** |

#### Scenario 3

This scenario is when the devices are seized for the files, chat logs and browser histories on them. Therefore, the goal is to keep the storage space of these encrypted, so these details can only be accessed when the correct passcode is entered.

The suggestions are revolving around physical security:

* [Encrypt your Hard Drive with BitLocker](/guides/encrypt-your-hard-drive-with-bitlocker-windows) on Windows
* [Encrypt your USB Drives with BitLocker](/guides/encrypt-your-usb-drives-with-bitlocker-on-windows) on Windows
* **Encrypting Android phones** _(coming soon)_
* **Setting up a Passcode on the iPhone** _(coming soon)_

#### Scenario 4

In this case, the Internet traffic of the journalist's PC and mobile phone are recorded and analyzed. Voice calls and text messages are also captured. The advisory's aim is to peek into the content of the communication between the journalist and the information source. 

! This scenario assumes that the link between the journalist and the information source is not secret, therefore the metadata retention (as opposed to the data content) is not a concern. The purpose of the listed tools is merely to encrypt communication between the two parties.

| Use Cases | Recommendations |
| --------- | --------------- |
| Web Browsing | **Using the Tor Browser** _(coming soon)_, **Setting up a VPN** _(coming soon)_ |
| Email | **[Encrypting Emails with PGP](../guides#email-security)** |
| Instant Messaging | **Encrypted Voice Calls and Text Messages** _(coming soon)_ |
| Voice Calls | **Encrypted Voice Calls and Text Messages** _(coming soon)_ |
| Video Calls | **[End-to-End Encrypted Video Calls with Wire](../guides/end-to-end-encrypted-video-calls)** |
| Text Messaging (SMS) | **Encrypted Voice Calls and Text Messages** _(coming soon)_ |
| File Exchange | **[Encrypting Emails with PGP](../guides#email-security)** |
| File Storage | **[Storing Files Privately in the Cloud](../guides/storing-files-privately-in-the-cloud)** |
| Team Collaboration | **[Secure Team Chat with Semaphor](../guides/secure-team-chat-with-semaphor)** |

#### Scenario 5

Since the [breaches of the Hacking Team](https://en.wikipedia.org/wiki/Hacking_Team?target=_blank) and [FinFisher](https://en.wikipedia.org/wiki/FinFisher?target=_blank), or [news from the FBI](http://www.newsweek.com/supreme-court-allows-fbi-hack-any-computer-anywhere-if-warrant-454278?target=_blank), we know that certain governmental organisations are willing to exploit computers and smartphones to install backdoors on them.

These backdoors are installed without the individuals knowledge and consent, and monitoring almost any activity of the device. This includes the recording of audio and video, logging keystrokes, taking screenshots, retrieving the browser history and so on. Once the computer or smartphone is backdoored, almost any various encryption technique from the [guide](../guides) is rendered useless.

! If you suspect your device is compromised, always wipe or factory-reset it and reinstall everything from a clean media

| Use Cases | Recommendations |
| --------- | --------------- |
| Web Browsing | Not secret if the computer/smartphone is compromised |
| Email | Not secret if the computer/smartphone is compromised |
| Instant Messaging | Not secret if the computer/smartphone is compromised |
| Voice Calls | Not secret if the computer/smartphone is compromised |
| Video Calls | Not secret if the computer/smartphone is compromised |
| Text Messaging (SMS) | Not secret if the computer/smartphone is compromised |
| File Exchange | Not secret if the computer/smartphone is compromised |

The goals in this scenario are the followings: prevent these types of software from exploiting your devices, compartmentalize your activities so the damage is limited, detect if there is an anomaly on your device. Here is our list of recommended actions:

* ** Using Tails and Qubes OS ** _(coming soon)_
* ** [Protect your PC from Backdoors](https://privacyforjournalists.org.au/guides/protect-your-pc-from-backdoors-windows) **
* ** Compartmentalize Your Work ** _(coming soon)_
* ** Is My Phone Compromised? ** _(coming soon)_

#### Scenario 6

This scenario is when the devices are seized for the files, chat logs and browser histories on them. Therefore, the aim is to keep the storage space of these encrypted, so these details can only be accessed when the correct passcode is entered.

The guides are revoling around physical security:

* [Encrypt your Hard Drive with BitLocker](/guides/encrypt-your-hard-drive-with-bitlocker-windows) on Windows
* [Encrypt your USB Drives with BitLocker](/guides/encrypt-your-usb-drives-with-bitlocker-on-windows) on Windows
* **Encrypted USB drives** _(coming soon)_
* **Encrypting Android phones** _(coming soon)_
* **Setting up a Passcode on the iPhone** _(coming soon)_

#### Scenario 7

This scenario is similar to [Scenario 5](#scenario-5) from earlier. Companies unhappy with your investigative articles may hire hackers to get into your computer to track down your information sources.

Hackers typically will send you specially crafted file attachments and web links. These files contain malware that will install a backdoor on your PC. As these are targeting you, they will not be picked up by traditional anti-malware products.

Backdoors are installed without the individuals knowledge and consent, and monitoring almost any activity of the device. This includes the recording of audio and video, logging keystrokes, taking screenshots, retrieving the browser history and so on. Once the computer or smartphone is backdoored, almost any various encryption technique from the [guide](../guides) is rendered useless.

! If you suspect your device is compromised, always wipe or factory-reset it and reinstall everything from a clean media

| Use Cases | Recommendations |
| --------- | --------------- |
| Web Browsing | Not secret if the computer/smartphone is compromised |
| Email | Not secret if the computer/smartphone is compromised |
| Instant Messaging | Not secret if the computer/smartphone is compromised |
| Voice Calls | Not secret if the computer/smartphone is compromised |
| Video Calls | Not secret if the computer/smartphone is compromised |
| Text Messaging (SMS) | Not secret if the computer/smartphone is compromised |
| File Exchange | Not secret if the computer/smartphone is compromised |

In order to protect yourself, you should compartmentalize your work to limit the damage. Secondly, you should never reuse your passwords across your user accounts. Thirdly, two-factor authentication should be turned on whereever possible. Finally, a more advanced anti-malware product may help to block some of these specially crafted files.

* ** Using Tails and Qubes OS ** _(coming soon)_
* ** [Protect your PC from Backdoors](https://privacyforjournalists.org.au/guides/protect-your-pc-from-backdoors-windows) **
* ** Compartmentalize Your Work ** _(coming soon)_
* ** Is My Phone Compromised? ** _(coming soon)_
* ** Storing Passwords in Password Wallets ** _(coming soon)_
* ** Protect Your Accounts with Two-Factor Authentication ** _(coming soon)_

#### Scenario 8

This scenario is somewhat similar to [Scenario 5](#scenario-5) with a difference that the journalist and the information source is not specifically targeted. Cyber-criminals run a lucrative business of infecting unpatched computers with malware and ransomware, stealing payment details or encrypting the victims' files for a ransom.

Therefore, generic tools like a good anti-malware software can be effective against these types of attacks.

* ** [Protect your PC from Backdoors](https://privacyforjournalists.org.au/guides/protect-your-pc-from-backdoors-windows) **
* **Compartmentalize Your Work** _(coming soon)_
* **Protect Your Accounts with Two-Factor Authentication** _(coming soon)_

#### Scenario 9

This scenario covers use cases when your data gets into the wrong hands, however the journalist and the information source is not specifically targeted. Typical cases are laptops or USB sticks forgotten in cafes and other public spaces, smartphones snatched from your pockets, and electronic devices stolen from your home as part of a break-in.

The aim is to encrypt everything in rest so the casual attacker will not be able to  get access to your data. Therefore, the recommendations are revolving around physical security:

* [Encrypt your Hard Drive with BitLocker](/guides/encrypt-your-hard-drive-with-bitlocker-windows) on Windows
* [Encrypt your USB Drives with BitLocker](/guides/encrypt-your-usb-drives-with-bitlocker-on-windows) on Windows
* **Encrypted USB drives** _(coming soon)_
* **Encrypting Android phones** _(coming soon)_
* **Setting up a Passcode on the iPhone** _(coming soon)_

## Further Reading

* [Why every journalist should have a threat model (with cats)](https://onlinejournalismblog.com/2014/07/16/why-every-journalist-should-have-a-threat-model-with-cats/?target=_blank) - Tongue-in-cheek guide to the basics of threat modeling 

* [Security for Journalists, Part Two: Threat Modeling](https://source.opennews.org/en-US/learning/security-journalists-part-two-threat-modeling/?target=_blank) - Jonathan Stray on how to protect yourself, your sources, and your scoop on sensitive stories

* [An Introduction to Threat Modeling](https://ssd.eff.org/en/playlist/journalist-move#introduction-threat-modeling?target=_blank) from the **EFF's Surveillance Self-Defense Guide**

* [Introduction](http://www.tcij.org/resources/handbooks/infosec/introduction?target=_blank) from the **'Information Security of Journalists'** by The Centre for Investigative Journalism

* [Technology Security](https://cpj.org/reports/2012/04/technology-security.php?target=_blank) from the **'Journalist Security Guide'** by Committee to Protect Journalists