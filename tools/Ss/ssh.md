#### ssh
`OpenSSH client for remote shell access`

```

```

##### Usage:
`ssh [-p port] [-i identityfile] [-L forward] [user@]hostname [command_]`

> -i identity_file
>> Specifies which private key file to use for authentication.    
If the matching private key isn’t stored locally, SSH uses the corresponding key loaded in ssh-agent.        
Defaults include: ~/.ssh/id_rsa, id_ecdsa, id_ecdsa_sk, id_ed25519, and id_ed25519_sk.      
Multiple -i options may be provided, and per‑host identity settings can also be defined in the SSH config.      
If no certificate is explicitly set, SSH will automatically look for a *-cert.pub file matching the identity.

---
