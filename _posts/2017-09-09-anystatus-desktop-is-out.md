---
layout: post
title:  AnyStatus Desktop is out!
date:   2017-07-02 12:00
author: AlonAm
tags: [New Releases]
redirect_from: "/2017/05/05/anystatus-desktop-release-1.4.html"
---

It has been a while since I have released a new version and I'm excited to announce that AnyStatus Desktop is now signed
with an official code signing certificate as part of its automated continuous integration pipeline.

That was not easy, first I had to find a certificate that is available for individuals, then figure out how to activate the certificate
using a cryptographic smart card and then find a way to sign the installer on a physicall machine that have the smart card connected
while the other tasks in the CI process runs on virtual VSTS agents on Azure.

Thanks to new VSTS deployment groups feature, I was able to run that specific task on a phisical machine.

If you have previously installed AnyStatus Desktop, you may have been warned by Windows that it is not safe to install this software.
I expect the certificate to elimate that warning once the app gets enough reputation.

You can download AnyStatus Desktop from our [downloads page](https://www.anystat.us/downloads).
