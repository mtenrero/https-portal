# Useful test commands for testing HTTP(s) connectivity

## TLS Protocol enforcing using cURL

### Fix specific TLS Protocol

```bash
curl -k https://localhost --tlsv1.3 --tls-max 1.3
```

## TLS Protocol enforcing using OpenSSL

```bash
openssl s_client -connect localhost:443 -tls1_2
```