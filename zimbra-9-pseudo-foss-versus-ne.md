# Zimbra 9.0.0 has been released

[zimbra 9.0.0 GA](https://wiki.zimbra.com/wiki/Zimbra_Releases/9.0.0) is here and it does not have an open source edition.
However this statement is done by Zimbra:

*Zimbra Collaboration 8.8 remains the Open Source Edition, and all security updates will be provided as patches to 8.8.15.
There are no Open Source repositories specific to Zimbra 9.*

That means that OSE version will be associated with Zimbra 8 and the NE version will be the brand new Zimbra 9.

# What if Zimbra 9.0.0 had a FOSS release

We can study the debian package repositories for Zimbra 9 (In this case Ubuntu 18.04 (bionic) ones in order to grasp what functionalities will be present in a FOSS release of Zimbra 9.0.0 (Fetched at April 17th 2020).


* [https://repo.zimbra.com/apt/90-ne/dists/bionic/zimbra/binary-amd64/Packages.gz](zimbra9-resources/packages-90-ne.txt)
* [https://repo.zimbra.com/apt/90/dists/bionic/zimbra/binary-amd64/Packages.gz](zimbra9-resources/packages-90.txt)
* [https://repo.zimbra.com/apt/87/dists/bionic/zimbra/binary-amd64/Packages.gz](zimbra9-resources/packages-87.txt)

## Packages extract example script

```
cat packages-87.txt | grep -E '^Package: ' | sed -e 's/Package: /* /g' | sort | uniq
```

## 90-ne packages

* zimbra-connect
* zimbra-connect-modern
* zimbra-docs
* zimbra-docs-modern
* zimbra-drive-modern
* zimbra-drive-ng
* zimbra-modern-ui
* zimbra-modern-zimlets
* zimbra-network-modules-ng
* zimbra-patch
* zimbra-talk
* zimbra-zimlet-calendar-subscription
* zimbra-zimlet-date
* zimbra-zimlet-dropbox
* zimbra-zimlet-duplicate-contacts
* zimbra-zimlet-google-drive
* zimbra-zimlet-install-pwa
* zimbra-zimlet-onedrive
* zimbra-zimlet-restore-contacts
* zimbra-zimlet-set-default-client
* zimbra-zimlet-sideloader
* zimbra-zimlet-slack
* zimbra-zimlet-zoom

## 90 packages


* zimbra-apache-components
* zimbra-chat
* zimbra-clamav
* zimbra-clamav-dbg
* zimbra-clamav-dev
* zimbra-clamav-lib
* zimbra-clamav-lib-dbg
* zimbra-core-components
* zimbra-drive
* zimbra-httpd
* zimbra-httpd-dbg
* zimbra-httpd-dev
* zimbra-jetty-distribution
* zimbra-ldap-components
* zimbra-libxml2
* zimbra-libxml2-dbg
* zimbra-libxml2-dev
* zimbra-libxml2-lib
* zimbra-libxml2-lib-dbg
* zimbra-lmdb
* zimbra-lmdb-dbg
* zimbra-lmdb-dev
* zimbra-lmdb-lib
* zimbra-lmdb-lib-dbg
* zimbra-mta-components
* zimbra-mta-patch
* zimbra-nginx
* zimbra-nginx-dbg
* zimbra-openjdk
* zimbra-openjdk-dbg
* zimbra-openldap-client
* zimbra-openldap-client-dbg
* zimbra-openldap-dev
* zimbra-openldap-lib
* zimbra-openldap-lib-dbg
* zimbra-openldap-server
* zimbra-openldap-server-dbg
* zimbra-openssl
* zimbra-openssl-dbg
* zimbra-openssl-dev
* zimbra-openssl-lib
* zimbra-openssl-lib-dbg
* zimbra-osl
* zimbra-patch
* zimbra-perl-mail-spamassassin
* zimbra-php
* zimbra-php-dbg
* zimbra-proxy-components
* zimbra-proxy-patch
* zimbra-spamassassin-rules
* zimbra-spell-components
* zimbra-timezone-data

## 87 packages

* zimbra-altermime
* zimbra-altermime-dbg
* zimbra-amavisd
* zimbra-amavis-logwatch
* zimbra-apache-base
* zimbra-apache-components
* zimbra-apr-dev
* zimbra-apr-lib
* zimbra-apr-lib-dbg
* zimbra-apr-util-dev
* zimbra-apr-util-lib
* zimbra-apr-util-lib-dbg
* zimbra-aspell
* zimbra-aspell-ar
* zimbra-aspell-da
* zimbra-aspell-dbg
* zimbra-aspell-de
* zimbra-aspell-dev
* zimbra-aspell-en
* zimbra-aspell-es
* zimbra-aspell-fr
* zimbra-aspell-hi
* zimbra-aspell-hu
* zimbra-aspell-it
* zimbra-aspell-lib
* zimbra-aspell-lib-dbg
* zimbra-aspell-nl
* zimbra-aspell-pl
* zimbra-aspell-pt-br
* zimbra-aspell-ru
* zimbra-aspell-sv
* zimbra-aspell-zimbra
* zimbra-base
* zimbra-bdb
* zimbra-bdb-dbg
* zimbra-bdb-dev
* zimbra-bdb-lib
* zimbra-bdb-lib-dbg
* zimbra-clamav
* zimbra-clamav-db
* zimbra-clamav-dbg
* zimbra-clamav-dev
* zimbra-clamav-lib
* zimbra-clamav-lib-dbg
* zimbra-cluebringer
* zimbra-core-components
* zimbra-curl
* zimbra-curl-dbg
* zimbra-curl-dev
* zimbra-curl-lib
* zimbra-curl-lib-dbg
* zimbra-cyrus-sasl
* zimbra-cyrus-sasl-dbg
* zimbra-cyrus-sasl-dev
* zimbra-cyrus-sasl-lib
* zimbra-cyrus-sasl-lib-dbg
* zimbra-dnscache-base
* zimbra-dnscache-components
* zimbra-freetype-dev
* zimbra-freetype-lib
* zimbra-freetype-lib-dbg
* zimbra-heimdal
* zimbra-heimdal-dbg
* zimbra-heimdal-dev
* zimbra-heimdal-lib
* zimbra-heimdal-lib-dbg
* zimbra-httpd
* zimbra-httpd-dbg
* zimbra-httpd-dev
* zimbra-jetty-distribution
* zimbra-ldap-base
* zimbra-ldap-components
* zimbra-libart-dev
* zimbra-libart-lib
* zimbra-libart-lib-dbg
* zimbra-libbsd-dev
* zimbra-libbsd-lib
* zimbra-libevent-dev
* zimbra-libevent-lib
* zimbra-libevent-lib-dbg
* zimbra-libltdl-dev
* zimbra-libltdl-lib
* zimbra-libltdl-lib-dbg
* zimbra-libmilter-dev
* zimbra-libpng-dev
* zimbra-libpng-lib
* zimbra-libpng-lib-dbg
* zimbra-libsodium-dev
* zimbra-libsodium-lib
* zimbra-libsodium-lib-dbg
* zimbra-libxml2
* zimbra-libxml2-dbg
* zimbra-libxml2-dev
* zimbra-libxml2-lib
* zimbra-libxml2-lib-dbg
* zimbra-lmdb
* zimbra-lmdb-dbg
* zimbra-lmdb-dev
* zimbra-lmdb-lib
* zimbra-lmdb-lib-dbg
* zimbra-mariadb
* zimbra-mariadb-dbg
* zimbra-mariadb-dev
* zimbra-mariadb-lib
* zimbra-mariadb-lib-dbg
* zimbra-memcached
* zimbra-memcached-base
* zimbra-memcached-dbg
* zimbra-memcached-dev
* zimbra-mta-base
* zimbra-mta-components
* zimbra-net-snmp
* zimbra-net-snmp-dbg
* zimbra-net-snmp-dev
* zimbra-net-snmp-lib
* zimbra-net-snmp-lib-dbg
* zimbra-nginx
* zimbra-nginx-dbg
* zimbra-opendkim
* zimbra-opendkim-dev
* zimbra-opendkim-lib
* zimbra-openjdk-cacerts
* zimbra-openjdk-dbg
* zimbra-openldap-client
* zimbra-openldap-client-dbg
* zimbra-openldap-dev
* zimbra-openldap-lib
* zimbra-openldap-lib-dbg
* zimbra-openldap-server
* zimbra-openldap-server-dbg
* zimbra-openssl
* zimbra-openssl-dbg
* zimbra-openssl-dev
* zimbra-openssl-lib
* zimbra-openssl-lib-dbg
* zimbra-osl
* zimbra-os-requirements
* zimbra-perl
* zimbra-perl-archive-zip
* zimbra-perl-base
* zimbra-perl-berkeleydb
* zimbra-perl-bit-vector
* zimbra-perl-cache-fastmmap
* zimbra-perl-canary-stability
* zimbra-perl-carp-clan
* zimbra-perl-class-inspector
* zimbra-perl-compress-raw-bzip2
* zimbra-perl-compress-raw-zlib
* zimbra-perl-config-inifiles
* zimbra-perl-convert-asn1
* zimbra-perl-convert-binhex
* zimbra-perl-convert-tnef
* zimbra-perl-convert-uulib
* zimbra-perl-crypt-openssl-random
* zimbra-perl-crypt-openssl-rsa
* zimbra-perl-crypt-saltedhash
* zimbra-perl-data-uuid
* zimbra-perl-date-calc
* zimbra-perl-date-manip
* zimbra-perl-dbd-mysql
* zimbra-perl-dbd-sqlite
* zimbra-perl-db-file
* zimbra-perl-dbi
* zimbra-perl-digest-hmac
* zimbra-perl-digest-sha1
* zimbra-perl-email-date-format
* zimbra-perl-encode-detect
* zimbra-perl-encode-locale
* zimbra-perl-error
* zimbra-perl-exporter-tiny
* zimbra-perl-file-grep
* zimbra-perl-file-libmagic
* zimbra-perl-file-listing
* zimbra-perl-filesys-df
* zimbra-perl-file-tail
* zimbra-perl-geography-countries
* zimbra-perl-html-parser
* zimbra-perl-http-cookies
* zimbra-perl-http-daemon
* zimbra-perl-http-date
* zimbra-perl-http-message
* zimbra-perl-http-negotiate
* zimbra-perl-innotop
* zimbra-perl-io-compress
* zimbra-perl-io-html
* zimbra-perl-io-sessiondata
* zimbra-perl-io-socket-inet6
* zimbra-perl-io-socket-ip
* zimbra-perl-io-socket-ssl
* zimbra-perl-io-stringy
* zimbra-perl-ip-country
* zimbra-perl-json-pp
* zimbra-perl-libwww
* zimbra-perl-list-moreutils
* zimbra-perl-lwp-mediatypes
* zimbra-perl-lwp-protocol-https
* zimbra-perl-mail-dkim
* zimbra-perl-mail-spamassassin
* zimbra-perl-mail-spf
* zimbra-perl-mailtools
* zimbra-perl-math-bigint
* zimbra-perl-mime-lite
* zimbra-perl-mime-tools
* zimbra-perl-mime-types
* zimbra-perl-mozilla-ca
* zimbra-perl-netaddr-ip
* zimbra-perl-net-cidr
* zimbra-perl-net-cidr-lite
* zimbra-perl-net-dns
* zimbra-perl-net-dns-resolver-programmable
* zimbra-perl-net-http
* zimbra-perl-net-ldap
* zimbra-perl-net-ldapapi
* zimbra-perl-net-libidn
* zimbra-perl-net-server
* zimbra-perl-net-ssleay
* zimbra-perl-parent
* zimbra-perl-proc-processtable
* zimbra-perl-soap-lite
* zimbra-perl-socket
* zimbra-perl-socket-linux
* zimbra-perl-swatchdog
* zimbra-perl-task-weaken
* zimbra-perl-term-readkey
* zimbra-perl-timedate
* zimbra-perl-unix-getrusage
* zimbra-perl-unix-syslog
* zimbra-perl-uri
* zimbra-perl-www-robotrules
* zimbra-perl-xml-namespacesupport
* zimbra-perl-xml-parser
* zimbra-perl-xml-parser-lite
* zimbra-perl-xml-sax
* zimbra-perl-xml-sax-base
* zimbra-perl-xml-sax-expat
* zimbra-perl-xml-simple
* zimbra-perl-zmq-constants
* zimbra-perl-zmq-libzmq3
* zimbra-pflogsumm
* zimbra-php
* zimbra-php-dbg
* zimbra-postfix
* zimbra-postfix-dbg
* zimbra-postfix-logwatch
* zimbra-prepflog
* zimbra-proxy-base
* zimbra-proxy-components
* zimbra-rrdtool
* zimbra-rrdtool-dbg
* zimbra-rrdtool-dev
* zimbra-rrdtool-lib
* zimbra-rrdtool-lib-dbg
* zimbra-rsync
* zimbra-rsync-dbg
* zimbra-snmp-base
* zimbra-snmp-components
* zimbra-spamassassin-rules
* zimbra-spell-base
* zimbra-spell-components
* zimbra-store-base
* zimbra-store-components
* zimbra-tcmalloc-dev
* zimbra-tcmalloc-lib
* zimbra-tcmalloc-lib-dbg
* zimbra-unbound
* zimbra-unbound-dbg
* zimbra-unbound-dev
* zimbra-unbound-lib
* zimbra-unbound-lib-dbg
* zimbra-zeromq
* zimbra-zeromq-dbg
* zimbra-zeromq-dev
* zimbra-zeromq-lib
* zimbra-zeromq-lib-dbg


# About Zimbra NE 9 exclusive packages

As you can see above the usual suspects appear:

* zimbra-connect : Video conferencing based on ZeXtras
* zimbra-docs : Rich document editing based on Collabora
* zimbra-drive-ng : New Zimbra Drive which does not connect to Nextcloud servers any more
* zimbra-network-modules-ng : ZeXtras full package under the Zimbra trademark
* zimbra-patch : Updated patches for some packages
* zimbra-talk : Chat substitute

Zimbra connect, docs and drive have been improved to be not only accessed by the classic UI but with the modern ui:

* zimbra-connect-modern
* zimbra-docs-modern
* zimbra-drive-modern

The brand new modern uni with zimlets support is unveiled:

* zimbra-modern-ui
* zimbra-modern-zimlets

which offers out of the box integrations for: Calendar, dropbox, google drive, pwa, onedrive, slack and zoom.


* zimbra-zimlet-dropbox
* zimbra-zimlet-google-drive
* zimbra-zimlet-onedrive
* zimbra-zimlet-slack
* zimbra-zimlet-zoom

Finally more straight-forward zimlets are available for the modern UI:

* zimbra-zimlet-calendar-subscription
* zimbra-zimlet-date
* zimbra-zimlet-duplicate-contacts
* zimbra-zimlet-install-pwa
* zimbra-zimlet-restore-contacts
* zimbra-zimlet-set-default-client
* zimbra-zimlet-sideloader

.

# About Zimbra 9 modern ui

We can take a closer look at the Zimbra 9 modern ui package:

```
Package: zimbra-modern-ui
Version: 3.2.0.1585823037-1.u18
Architecture: amd64
Maintainer: Zimbra Packaging Services <build@zimbra.com>
Installed-Size: 38754
Depends: zimbra-network-store (>= 8.8.15)
Replaces: zimbra-store
Priority: optional
Section: mail
Filename: pool/zimbra/z/zimbra-modern-ui/zimbra-modern-ui_3.2.0.1585823037-1.u18_amd64.deb
Size: 7161976
SHA256: 34ba71af67925672ed01e8a22a2270a4012123d04ef192509342006049516727
SHA1: 77a0cd2b5674a600c9a3a7542b7d164f06fdc848
MD5sum: a802d144b13faa5e161b7aadafa9e738
Description: Zimbra X Web
```

The description unveils that this is related to Zimbra X. Zimbra X needs a web interface.
It seems it will be the same one as Zimbra 9 and it makes sense from an engineering point of view.

This packages depend on zimbra-network-store to work.
This means that zimbra-modern-ui despite being a core component designed to replace the classic UI in the mid term is not open source.

You can also check for zimbra github team page. There is not zimbra-modern-ui repo there. And the zimbra-x-ui repo does not have anything interesting.

# Synacor Zimbra tears up Zimbra OSE

Not only Synacor Zimbra is associating Zimbra OSE with the (now) old Zimbra 8 but it's also refusing to open source its modern ui.

# Zimbra 9.0 Pseudo FOSS

If you were able to choose Zimbra 9 OSE packages (see above *90 packages* section) you would get:
zimbra chat and zimbra drive. Everything else would be software you already find on Zimbra 8.7 OSE packages: Clamav, Apache, Jetty, Lmdb, mta, nginx, ldap, openssl, spamassassin, spell and a few more others.

No modern ui.

# Enjoy Zimbra 9.0 Pseudo FOSS right now

Disclaimer: This procedure has not been tested and it does not mean that what you install on your system would be 100% open source. Someone would need to double check it.

```
wget "https://files.zimbra.com/downloads/9.0.0_GA/zcs-NETWORK-9.0.0_GA_3924.UBUNTU18_64.20200331010312.tgz"
tar xzf zcs-NETWORK-9.0.0_GA_3924.UBUNTU18_64.20200331010312.tgz
cd zcs-NETWORK-9.0.0_GA_3924.UBUNTU18_64.20200331010312.tgz
cp .BUILD_TYPE dotBUILD_TYPE-ORIGINAL-20200417
echo "FOSS" > .BUILD_TYPE
sudo ./install.sh
```

This procedure might be used to experience what a 9.0 FOSS edition would have been. And also to check the changes since ZCS 8.8.15 to the Zimbra FOSS core.