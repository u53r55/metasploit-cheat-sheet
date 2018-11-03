#### Metasploit Cheat Sheet

<p align="center">
<img src="/image/rapid7.png" height="100px" width="100px"><img src="/image/metasploit.png" height="100px" width="100px"><img src="/image/rapid7.png" height="100px" width="100px">
</p>

The Metasploit Project is a computer security project that provides information on vulnerabilities, helping in the development of penetration tests and IDS signatures.


##### Metasploit :

###### Search for module:

```
msf > search [regex]
```

###### Specify and exploit to use:

```
msf > use exploit/[ExploitPath]
```

###### Specify a Payload to use:

```
msf > set PAYLOAD [PayloadPath]
```

###### Show options for the current modules:

```
msf > show options
```

###### Set options:

```
msf > set [Option] [Value]
```

###### Start exploit:

```
msf > exploit 
```

##### Useful Auxiliary Modules


###### Port Scanner:

```
msf > use auxiliary/scanner/portscan/tcp
msf > set RHOSTS 10.10.10.0/24
msf > run
```

###### DNS Enumeration:

```
msf > use auxiliary/gather/dns_enum
msf > set DOMAIN target.tgt
msf > run
```

###### FTP Server:

```
msf > use auxiliary/server/ftp
msf > set FTPROOT /tmp/ftproot
msf > run
```

###### Proxy Server:

```
msf > use auxiliary/server/socks4
msf > run 
```
