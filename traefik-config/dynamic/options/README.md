# Cipher Suites
To use other TLS options than default you can specify it by service.
This can be done in two ways:

## Lables:
```
# Following the above configuration
traefik.routers.foo.tls.options=modern # modern | default | legacy 
```

## YAML / YML
```
http:
  routers:
    foo:
      tls:
        options: modern # modern | default | legacy
```
Note:
As you will only need to specify `modern` or `legacy` for the other options,
the `default` will be used when nothing is specified. Alternativly you can
specify `default`, but not needed.
