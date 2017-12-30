On Opensuse 42.3 we have perl-IO-Socket-SSL at version 1.962.
Script `analyze-ssl.pl` (https://github.com/noxxi/p5-ssl-tools/blob/master/analyze-ssl.pl) require 1.984

This repo contain files after download `IO-Socket-SSL` and ran
```
perl Makefile.PL INSTALL_BASE=/home/marcin/.local/analyze-ssl
make
make test
make install
```

I can clone this repo somewhere and set alias
```
analyze-ssl.pl is aliased to `PERL5LIB=/home/marcin/.local/analyze-ssl/lib/perl5/ analyze-ssl.pl'
```

And now analyze-ssl.pl works
