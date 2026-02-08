## Tools Used

---
#### enum4linux

`Enumerate information from Windows and Samba systems`

```
```

> -S
>> Enumerate shared resources (shares) on the target.

---

#### gobuster
`gobuster - Directory/file & DNS busting tool written in Go`
```

```
> dir - the classic directory brute-forcing mode

>vhost - virtual host brute-forcing mode - not the same as DNS

>-s string
>>Positive status codes (dir mode only) (default "200,204,301,302,307")

>-u, --url string  

>-w, --wordlist string

>-k
>> Skip TLS certificate verification

>--append-domain, --ad
>> Append main domain from URL to words from wordlist. Otherwise the fully qualified domains need to be specified in the wordlist. (default : false)

---

#### hashcat
`Crack password hashes using various methods`

```

```


> -m, --hash-type=NUM
>> Hash-type ID (see hashcat --help for 350+ types like 0=MD5, 1000=NTLM)

> -r, --rules-file=FILE
>> Load rules from FILE for mutations

---

#### hydra
`hydra - a very fast network logon cracker which supports many different services`
```

```

> -l LOGIN or -L FILE  
>>login with LOGIN name, or load several logins from FILE

>-p PASS
>>or -P FILE try password PASS, or load several passwords from FILE

---

#### netcat

`nc - TCP/IP swiss army knife`
```

```
> -l    listen mode, for inbound connects

> -v     verbose [use twice to be more verbose]

> -n     numeric‐only IP addresses, no DNS

> -p    port    local port number (port numbers can be individual or ranges: lo‐hi [inclusive])

---

#### nmap

`nmap - Network exploration tool and security / port scanner`
```

```

>-p (port_range)
>> Port specification: Specifies which ports to scan (e.g., -p 80,443, -p 1-1024, -p- for all ports).

>-sC: equivalent to --script=default

>-sV: Probe open ports to determine service/version info

> --script <script_name|category|directory>
>> Nmap Scripting Engine: Runs specific Nmap scripts or categories of scripts (e.g., --script http-enum, --script default, --script vuln).

---

#### radare2
`Reverse engineer and analyze binaries`

```

```

> aaa 
>> preform deeper analysis, most common use

> aaaa
>> same as aaa but adds a bunch of experimental iterations

> afl
>> list funcions

> axt
>> find data/code rferences to this address

> pdf
>> disassmeble function in a linear way (see pdfr)

> s < addr>
>> seek to address

---

#### ssh

`ssh — OpenSSH remote login client`

```

```

> -i identity_file
>> Selects a file from which the identity (private key) for public key authentication is read. You can also specify a public key file to use the corresponding private key that is loaded in ssh-agent(1) when the private key file is not present locally.     
The default is ~/.ssh/id_rsa, ~/.ssh/id_ecdsa, ~/.ssh/id_ecdsa_sk, ~/.ssh/id_ed25519 and ~/.ssh/id_ed25519_sk.      
Identity files may also be specified on a per-host basis in the configuration file. It is possible to have multiple -i options (and multiple identities specified in configuration files).      
If no certificates have been explicitly specified by the CertificateFile directive, ssh will also try to load certificate information from the filename obtained by appending -cert.pub to identity filenames.

---

#### searchploit

`SearchSploit ‐ Exploit Database Archive Search`

```
```

>-m, --mirror
>> Copies (mirrors) the selected exploit file to the current working directory.

---

#### stegcracker
`stegcracker -  steganography brute-force tool`
```

```

---

#### steghide
`steghide - a steganography program
`
```

```
>‐sf, ‐‐stegofile filename

---

#### wget
`Wget - The non-interactive network downloader.`
```

```
>Syntax: wget [option]... [URL]...

---
