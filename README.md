Wysyłanie smsów z poziomu linuxowego terminala
===========

Klient napisany w bashu, pozwalający na wysyłanie wiadomości SMS w serwisie SMSAPI.pl
Wymagania: `curl`  
Opcja --password-plain wymaga zainstalowanego narzędzia `openssl`  

```bash
$ ./smsapi sms send --username LOGIN --password PASS --from Info 48xxxyyyzzz,48zzzyyyxxx "Hello world"
```

```bash
$ ./smsapi 
Usage: smsapi sms send [OPTIONS] <to> <message>
Options:
  --username <string>
  --password <password>  md5 api password
  --password-plain <password>  api password (plain text)

  --from <string>        Sender name
  --encoding <string>    Message encoding (default:utf8)

  -f, --fast <0|1>       Fast

  -n, --normalize <0|1>  Normalize message
  -v                     Verbose
```

Utworzenie hasła md5:
```
echo -n "plain_text_password" | openssl dgst -md5
```

Plik konfiguracyjny ".smsapi.rc" może się znajdowac w katalogu roboczym lub w katalogo domowym użytkownika

=======

