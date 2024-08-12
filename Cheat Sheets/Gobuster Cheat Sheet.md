---
tags:
  - Tools
  - Cybersecurity
  - Notes
---
___
#### Syntax:
```bash
gobuster [Mode] [URL] [Wordlist]
```
#### Example:
```bash
gobuster dir -u http://example.com -w wordlist.txt
```
#### Options/Flags:

| Options & Flags: | Description:                          |
| ---------------- | ------------------------------------- |
| `dir`            | Directory brute-force mode            |
| `dns`            | DNS subdomain brute-force mode        |
| `-u`             | Target URL                            |
| `-w`             | Wordlist for directory and file names |
| `-t`             | Number of concurrent threads          |
| `-x`             | File extensions to check              |
| `-o`             | Output file                           |
| `-q`             | Quiet mode                            |
| `-h`             | Help                                  |
___