# varnish-bad-bot-detection
A Varnish 4.0 subroutine for blocking bad bots (from http://omninoggin.com/web-development/block-unwanted-spam-bots-using-varnish-vcl/)

Example:

```vcl
include "/etc/varnish/conf.d/bad_bot_detection.vcl";

sub vcl_recv {

    call bad_bot_detection;
}    
```
