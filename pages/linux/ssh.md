---
title: SSHing into your workstation
tags: [ssh]
sidebar: mydoc_sidebar
permalink: ssh.html
summary: "SSHing into your workstation"
folder: linux
---

### Installing Duke's VPN

[Download Duke's VPN Client](https://software.duke.edu/node/193)
Once installed set the connection address to `vpn.duke.edu`
You'll need to be connected to this VPN to connect to your workstation while off campus.

### Grabbing your IP

In the ubuntu terminal type

```bash
hostname -I
```

This will output your local IP Address

```bash
$ hostname -I
xx.xxx.xx.xxxx
```

### Connecting to your workstation

Now from any client that has `ssh` installed, just connect to your IP

```bash
ssh xx.xxx.xx.xxxx
```

### Setting up an SSH Key (Optional)

Add an ssh key to bypass the password prompt when connecting to your workstation.

[Follow these steps to generate a ssh key on the client you will be connecting to your workstation from.](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

Once generated, go back to your workstation and navigate to `~/.ssh`(if this folder does not exist create it).

Edit your `authorized_keys` folder (again create it if it does not exist) and add the public key you just created to your authorized keys.
