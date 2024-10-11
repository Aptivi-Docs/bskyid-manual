---
description: How do you use BskyId?
icon: question
---

# How to use

This script is easy to use. Just get your BlueSky handle from your BlueSky account that you can find over the [BlueSky](https://bsky.app/) website, and pass it to the script. This ID is a unique identifier for your BlueSky account and can't be edited.

## Usage

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

Both scripts return just a BlueSky ID associated with your BlueSky account. Replace the `$handle` variable with your BlueSky handle linked above. The following switches are supported:

* `-plain`: Outputs the BlueSky ID handle in a plain JSON response instead of just the ID.
* `-nocolor`: Don't use colors on success or failure.

{% hint style="warning" %}
You must write your handle before any switch can be used.
{% endhint %}
