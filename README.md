# nip.io
wildcard DNS for any IP Address

NIP.IO allows you to map any IP Address in the following DNS wildcard entries:

```
10.0.0.1.nip.io maps to 10.0.0.1
app.10.0.0.1.nip.io maps to 10.0.0.1
customer1.app.10.0.0.1.nip.io maps to 10.0.0.1
customer2.app.10.0.0.1.nip.io maps to 10.0.0.1
otherapp.10.0.0.1.nip.io maps to 10.0.0.1
```

NIP.IO maps ```<anything>.<IP Address>.nip.io``` to the corresponding ```<IP Address>```, even 127.0.0.1.nip.io maps to 127.0.0.1

This service is a blatant rip-off of xip.io, with one big difference: NIP.IO is powered by PowerDNS with a simple, custom PipeBackend. So, it actually works :) (no messy, custom DNS server here!)

The custom PipeBackend is a single script written in Python and the source can be found on XP-Dev.com. 
