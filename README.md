Wysyłanie smsów z poziomu linuxowego terminala
===========

Klient napisany w bashu, pozwalający na wysyłanie wiadomości SMS w serwisie SMSAPI.pl

```bash
$ ./smsapi sms send --username LOGIN --password PASS 48xxxyyyzzz,48zzzyyyxxx "Hello world"
```

```bash
$ ./smsapi 
Usage: smsapi sms send [OPTIONS] <to> <message>
Options:
  --username <string>
  --password <password>

  --from <string>        Sender name
  --encoding <string>    Message encoding (default:utf8)

  -f, --fast <0|1>       Fast

  -n, --normalize <0|1>  Normalize message
  -v                     Verbose
```

plik konfiguracyjny ".smsapi.rc" może się znajdowac w katalogu roboczym lub w katalogo domowym użytkownika

=======

