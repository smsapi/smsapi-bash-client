Send message using linux terminal
===========

SMSAPI bash client that allows you to send messages from your SMSAPI.pl or SMSAPI.com account

## Send message using smsapi.pl service
```bash
$ ./smsapi sms send --service SMSAPI_PL --oauth TOKEN --from Info PhoneNumber1,PhoneNumber2 "Hello world"
```

## Send message using smsapi.com service
```bash
$ ./smsapi sms send --service SMSAPI_COM --oauth TOKEN --from Info PhoneNumber1,PhoneNumber2 "Hello world"
```

## Send message using configuration file
```bash
$ ./smsapi 
Usage: smsapi sms send [OPTIONS] <to> <message>
Options:
  --service <SMSAPI_PL or SMSAPI_COM>
  --oauth <OAuth token>
  --from <string>        Sender name
  --encoding <string>    Message encoding (default:utf8)
  -f, --fast <0|1>       Fast
  -n, --normalize <0|1>  Normalize message
  -v                     Verbose"
```

you have to create .smsapi.rc file using example.smsapi.rc
