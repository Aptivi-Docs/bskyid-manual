---
description: Welcome to BskyId!
icon: hand-wave
---

# Welcome!

This project, written in Bash and PowerShell, is a simple tool that gives you your BlueSky ID that is unique to your username. Just get your BlueSky handle from your BlueSky account that you can find over the [BlueSky](https://bsky.app/) website, and pass it to the script. This ID is a unique identifier for your BlueSky account and can't be edited.

To use this script, you can just use:

{% code title="Windows" %}
```powershell
Set-ExecutionPolicy Bypass -Scope Process
./bskyid.ps1 $handle [-plain/-nocolor]
```
{% endcode %}

{% code title="Linux" %}
```shell-session
$ ./bskyid $handle [-plain/-nocolor] # Local installation
$ bskyid $handle [-plain/-nocolor]   # Global installation
```
{% endcode %}

To learn how to use this script, go to any link in the left side of your screen.
