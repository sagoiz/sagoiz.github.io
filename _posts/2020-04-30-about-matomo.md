---
layout: post
title:  "Blog built via Jekyll!"
date: 2020-04-30 12:05:00 +0300
tags: [blog, matomo, web, analytics, open source]
author: Serafin
---

# About Matomo
First things first, so you can find information about Matomo (here)[https://matomo.org/].

In a nutshell, Matomo is an **Open Source web analytics platform.**

I decided to give it a try and used the Bitnami (installer)[https://bitnami.com/stack/matomo/installer].
I deployed at GCP.
As expected, the deployment was a one-click process, simple and quick.
Once the machines is up, you can login and check the installation, processes, etc..
I use the command line, no UI tools, so:
```shell
$ installdir/ctlscript.sh status
```
Check this (link)[https://docs.bitnami.com/installer/apps/matomo/administration/control-services-linux/] for further information.

I was trying to get all configured regarding the website, editing the apache configuration file, etc.
And it's all good, but you have an easier way if you do have a custom domain to use.
Simply use:
```shell
$ sudo installdir/bncert-tool
```
You'll have everything configured by the script, including the apache virtualhost configuration, certificates for HTTPS,...
And, even if you touched those configuration files manually (as I did), the script will back them up, do the magic and it will simply work.
Link to the documentation page (here)[https://docs.bitnami.com/installer/apps/matomo/administration/generate-configure-certificate-letsencrypt/]
Title is a bit misleading as the script will not only take care of the "Let's Encrypt" certificate.

So, give it a try.
