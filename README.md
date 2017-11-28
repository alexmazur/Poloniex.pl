Poloniex API wrapper
============================

Just run the code and install the dependencies. I could have used non but I was in a hurrter.

```
Time::HiRes qw(time);
POSIX qw(strftime);
PHP::HTTPBuildQuery qw(http_build_query);
Digest::SHA qw(hmac_sha512_hex);
LWP::UserAgent;
JSON::XS;
WWW::Curl::Easy;
Test::JSON;
Scalar::Util 'blessed';
```


The constructor takes 2 parameters, your key and secret. 

The methods and their parameters are fairly easy to read in the code.
