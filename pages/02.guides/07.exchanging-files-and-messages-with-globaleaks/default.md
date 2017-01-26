---
title: 'Exchanging Files and Messages with GlobaLeaks'
---

# Exchanging Files and Messages with GlobaLeaks

Every time a file is exchanged over the Internet via services like emails, Dropbox or file transfer features of instant messaging applications, metadata is left all over the place that can link the journalist and its information source together.

We wrote about [OnionShare](../secure-file-exchange-without-leaving-metadata-onionshare), which is a simple solution for ad-hoc file transfers. As OnionShare does not have any chat feature, you have to run [Ricochet](../secure-chat-without-leaving-metadata-ricochet) in parallel. However, both parties needs to be online at the same time in both cases.

[GlobaLeaks](https://www.globaleaks.org/?target=_blank) is a secure platform that simplifies the process. It runs as a Tor hidden service, where it connects the information source and the journalist together. The server is self-hosted, therefore the uploaded data and messages are only accessible to you. Also, files are encrypted with [PGP](/guides#email-security), so nobody can open the files except for you and only you.

GlobaLeaks, along with the other popular platform [SecureDrop](https://securedrop.org/?target=_blank), is currently used by [numerous media organisations](https://en.wikipedia.org/wiki/GlobaLeaks#Implementations?target=_blank) across the globe.

The following guide demonstrates how an information source can upload files and send messages with the service as well as how the journalist can retrieve them.

!!! Need some help with hosting GlobaLeaks? [Contact us](../community) to discuss

## Uploading Files as an Information Source

* The information source visits the **.onion** URL with the Tor browser. The URL should be published on your web site. For example, ours is listed in the [community](../community) section.

![Visiting the .onion URL as a source](submission-1.png?lightbox=1024&cropResize=700,700)

* The source presses the button on the middle and the following screen is shown where the files and messages can be added

![Adding files and messages](submission-2.png?lightbox=1024&cropResize=700,700)

![Adding files and messages](submission-3.png?lightbox=1024&cropResize=700,700)

* The source presses the _'Submit'_ button to send the files to the journalist

## Retrieving Files as the Journalist

Once the files are submitted, the journalist receives an optional, PGP encrypted email of the submission.

![Email notification](reporter-1.png?lightbox=1024&cropResize=700,700)

* The journalist logs in where he or she can list and open the submissions

![Submissions](reporter-2.png?lightbox=1024&cropResize=700,700)

* The reporter can retrieve the files and send messages to the information source. The files are encrypted with PGP, so they have to be decrypted once the files are downloaded to the local hard disk.

![Submission](reporter-3.png?lightbox=1024&cropResize=700,700)

![Writing a message](reporter-4.png?lightbox=1024&cropResize=700,700)

## Adding More Messages

The information can log back in any time to add more files, or read and write messages. 

* The source logs back in with the key code to read and write messages

![Logging in](logging-in.png?lightbox=1024&cropResize=700,700)

* The information source responds to the message of the journalist

![Replying to a message](submission-5.png?lightbox=1024&cropResize=700,700)

* The reporter receives an optional, PGP encrypted email about the arrival of the new comment

![Email notification](reporter-5.png?lightbox=1024&cropResize=700,700)