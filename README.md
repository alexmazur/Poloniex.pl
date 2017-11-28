Poloniex API wrapper
============================

Just run the code and install the dependencies.

```perl
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

```perl
 my ( $api_key, $api_secret ) = @_;
```

The methods and their parameters are fairly easy to read in the code.

```perl
sub get_ticker($pair) {}

sub get_trade_history($pair) {}

sub get_order_book($pair) {}

sub get_volume($pair) {}

sub get_trading_pairs() {}

sub get_balances() {}

sub get_open_orders($pair) {}

sub get_my_trade_history($pair) {}

sub buy($pair, $rate, $amount) {}

sub sell($pair, $rate, $amount) {}
```
