---
description: How to install?
icon: compact-disc
---

# Installing

Installing this script is easy. To install it, follow these steps, assuming that you have either `CURL` or `wget` installed on your Linux system:

{% hint style="info" %}
You'll have to install `curl`, irrespective of what method you prefer, since this script internally uses `curl`.
{% endhint %}

## Windows

Just use this command in your PowerShell command prompt:

```powershell
Invoke-WebRequest -Uri https://raw.githubusercontent.com/Aptivi/bskyid/main/src/bskyid.ps1 -OutFile bskyid.ps1
```

## Linux

Installation on Linux systems can be done in two ways.

### Local and System-wide

There are two ways to install this script on your system. If you want to make this script available to all the users on your Linux system, be sure to install it on your home directory like this:

```shell-session
$ curl -fsSL https://raw.githubusercontent.com/Aptivi/bskyid/main/src/bskyid > $HOME/bskyid
$ chmod +x $HOME/bskyid
```

If you want to make this script available to all of the users installed, follow these two scripts as root (`sudo`):

```shell-session
$ curl -fsSL https://raw.githubusercontent.com/Aptivi/bskyid/main/src/bskyid | sudo tee /usr/local/bin/bskyid
$ sudo chmod +x /usr/local/bin/bskyid
```

If you prefer using wget to install the script, follow these steps:

* For local installs

```shell-session
$ wget -O$HOME/bskyid https://raw.githubusercontent.com/Aptivi/bskyid/main/src/bskyid
$ chmod +x $HOME/bskyid
```

* For system-wide installs

```shell-session
$ sudo wget -O/usr/local/bin/bskyid https://raw.githubusercontent.com/Aptivi/bskyid/main/src/bskyid
$ sudo chmod +x /usr/local/bin/bskyid
```

{% hint style="warning" %}
For MinGW, WSL, and Git Bash installs, only the local install is supported.
{% endhint %}
