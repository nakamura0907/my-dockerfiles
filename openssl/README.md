```bash
$ docker build . -t openssl
$ docker run --rm -v $(pwd)/certs:/certs openssl req -x509 -out /certs/mycert.crt -keyout /certs/mycert.key -newkey rsa:2048 -nodes -sha256 -subj '/C=JP'
```
