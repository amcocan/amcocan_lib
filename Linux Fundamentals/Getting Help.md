---
tags:
  - HTB
  - Notes
  - Linux
  - Reference
---
___
We will always stumble across tools whose optional parameters we do not know from memory or tools we have never seen before. Therefore it is vital to know how we can help ourselves to get familiar with those tools. The first two ways are the man pages and the help functions. It is always a good idea to familiarize ourselves with the tool we want to try first. We will also learn some possible tricks with some of the tools that we thought were not possible. In the man pages, we will find the detailed manuals with detailed explanations.
#### Syntax:

```shell-session
amcocan@htb[/htb]$ man <tool>
```

Let us have a look at an example:
#### Example:

```shell-session
amcocan@htb[/htb]$ man curl
```

>[!warning]
>Instances of `{...}` were used to shorten the shell output in this example.

```shell-session
curl(1) {...} curl(1)

NAME
       curl - transfer a URL

SYNOPSIS
       curl [options] [URL...]

DESCRIPTION
       curl  is  a tool to transfer data from or to a server, using one of {...}

Manual page curl(1) line 1 (press h for help or q to quit)

```

After looking at some examples, we can also quickly look at the optional parameters without browsing through the complete documentation. We have several ways to do that.
#### Syntax:

```shell-session
amcocan@htb[/htb]$ <tool> --help
```
#### Example:

```shell-session
amcocan@htb[/htb]$ curl --help

Usage: curl [options...] <url>
     --abstract-unix-socket <path> Connect via abstract Unix domain socket
     --anyauth       Pick any authentication method
 -a, --append        Append to target file when uploading
     --basic         Use HTTP Basic Authentication
     --cacert <file> CA certificate to verify peer against
     --capath <dir>  CA directory to verify peer against
 -E, --cert <certificate[:password]> Client certificate file and password
<SNIP>
```

We can also use the short version of it:
#### Syntax:

```shell-session
amcocan@htb[/htb]$ <tool> -h
```
#### Example:

```shell-session
amcocan@htb[/htb]$ curl -h

Usage: curl [options...] <url>
     --abstract-unix-socket <path> Connect via abstract Unix domain socket
     --anyauth       Pick any authentication method
 -a, --append        Append to target file when uploading
     --basic         Use HTTP Basic Authentication
     --cacert <file> CA certificate to verify peer against
     --capath <dir>  CA directory to verify peer against
 -E, --cert <certificate[:password]> Client certificate file and password
<SNIP>
```

As we can see, the results from each other do not differ in this example. Another tool that can be useful in the beginning is `apropos`. Each manual page has a short description available within it. This tool searches the descriptions for instances of a given keyword.
#### Syntax:

```shell-session
amcocan@htb[/htb]$ apropos <keyword>
```
#### Example:

```shell-session
amcocan@htb[/htb]$ apropos sudo

sudo (8)             - execute a command as another user
sudo.conf (5)        - configuration for sudo front end
sudo_plugin (8)      - Sudo Plugin API
sudo_root (8)        - How to run administrative commands
sudoedit (8)         - execute a command as another user
sudoers (5)          - default sudo security policy plugin
sudoreplay (8)       - replay sudo session logs
visudo (8)           - edit the sudoers file
```

Another useful resource to get help if we have issues to understand a long command is: [https://explainshell.com/](https://explainshell.com/)
___