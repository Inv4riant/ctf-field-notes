#### nmap
`Network discovery utility and port scanner`

```

```

##### Usage:
`nmap [options] targets`

>-p (port_range)
>> Defines which ports to scan. Accepts single ports, comma‑separated lists, ranges (e.g., 1–1024), or -p- for all ports.

> -Pn
>> Treats every host as reachable by skipping the host‑discovery phase.

>-sC
>> Runs the default script set (same as --script=default).

>-sV
>> Examines open ports to identify the service and version running on them.

> --script <script_name|category|directory>
>>Executes specific NSE scripts, script groups, or all scripts in a directory (e.g., http-enum, default, vuln).

---
