#### gobuster
`Directory/file & DNS busting tool written in Go`

```

```

##### Usage:
`gobuster mode [options]`

> dir
>> Performs brute‑force discovery of directories and files on a web server.

>vhost
>> Attempts to identify virtual hosts by testing hostnames against the target.      
(Different from DNS enumeration.)

>-s string
>> Specifies which HTTP status codes should be treated as valid hits in directory mode.     
(Default: "200,204,301,302,307")

>-u, --url string
>> Target URL to scan.

>-w, --wordlist string
>> Path to the wordlist used for brute‑forcing.

>-k
>> Ignores TLS/SSL certificate validation.

>--append-domain, --ad
>> Adds the main domain from the target URL to each word in the wordlist.       
Without this, the wordlist must contain full domain names.
(Default: false)

---
