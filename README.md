# univention-postfix-catchall

Inspired by https://gist.github.com/Mario-F/15e43f39a6363bc2c890e1c2775fbc1f

Adds configurable catchall adress for all mail domains.
 Just set ucr variable mail/catchall/prefix to the desired prefix
 and assign a corresponding alternative mail addresses to a user who
 should receive the mails.
 
 E.g.:
 . 
  * prefix is set to "catchall"
  * assign "catchall@your.tld" to one or more users
  * all emails sent to non-existing addresses of @your.tld will be redirected to catchall@your.tld
 .

## Howto use
1. Clone repo
2. Install debhelper and univention-config-dev
3. Build package 'dpkg-buildpackage -b'
4. Install package.
