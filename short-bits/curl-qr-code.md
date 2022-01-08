---
layout: layouts/base.njk
title: Create a QR code with curl
description: <pre>curl qrenco.de/:[CONTENT]</pre><pre>curl qrenco.de/https://piraces.dev</pre>
image: ../../img/short-bits/default.png
short: true
date: 2022-01-08
templateClass: tmpl-post
---

If you are already familiar or you just feels comfy with the terminal, there are [lots of services you can use with curl](https://github.com/chubin/awesome-console-services).

In this case, we can create a QR code with curl using the service in [qrenco.de](https://qrenco.de):

```bash
curl qrenco.de/https://piraces.dev # Replace after the first slash with the content you want
```

***Note:** you can also make use of this service directly in your web browser since its a simple HTTP GET request.*

An example of this execution is the following:

```bash
█████████████████████████████████
█████████████████████████████████
████ ▄▄▄▄▄ ██▀▄██▀  ██ ▄▄▄▄▄ ████
████ █   █ █▄▀█▄▀█▀▀██ █   █ ████
████ █▄▄▄█ ██▄▀▀ █▀ ██ █▄▄▄█ ████
████▄▄▄▄▄▄▄█ █▄▀▄▀▄█ █▄▄▄▄▄▄▄████
████  ▄█▄▄▄  ▀█▀ █▄▄▄  ███▄█▀████
████▀█▀▀▄▄▄▄▀▀ ▄  ▄████▀▄█▄ ▄████
████▄ ▄▀ ▄▄▄▀█  ██▄█▀▄ ▄█ █▄ ████
████▄▀ ▀ ▄▄▀▄  ▀█▄█▀▀▀ ▄▀█▄ ▄████
████▄███▄▄▄█ ██▀ ▀█▀ ▄▄▄  █▀▀████
████ ▄▄▄▄▄ █ █ ▄ ▀ ▄ █▄█  █ ▄████
████ █   █ █▄█  ██ █ ▄▄   ▀▄▄████
████ █▄▄▄█ █ ▄ ▀█▄█▀ ▀██ ▀█▀▄████
████▄▄▄▄▄▄▄█▄█▄█▄██▄▄▄▄▄███▄▄████
█████████████████████████████████
█████████████████████████████████
```

A very cool ASCII QR Code 😎
