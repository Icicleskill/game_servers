# Pangolin

### [Docs](https://docs.pangolin.net/)

### Notes

When creating the stack in komodo ensure the API key variable is set in the Environment section of the stack. Ensure the key is configured in komodo settings variables.
```
    DREAMHOST_API_KEY = [[DREAMHOST_API_KEY]]
```

Use DreamHost DNS API [https://github.com/acmesh-official/acme.sh/wiki/dnsapi#40-use-dreamhost-dns-api]
DNS API keys may be created at https://panel.dreamhost.com/?tree=home.api. Ensure the created key has add and remove privileges.

    export DH_API_KEY="<api key>"
    ./acme.sh --issue --dns dns_dreamhost -d example.com -d *.example.com