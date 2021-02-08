### 1.) Install git & repoman

Install git via portage:

    gentoo /home/vagrant # emerge -pv dev-vcs/git
    
    These are the packages that would be merged, in order:
    
    Calculating dependencies... done!
    [ebuild  N     ] virtual/perl-Digest-MD5-2.550.0-r2::gentoo  0 KiB
    [ebuild  N     ] dev-perl/TimeDate-2.300.0::gentoo  31 KiB
    [ebuild  N     ] virtual/perl-IO-1.400.0::gentoo  0 KiB
    [ebuild  N     ] virtual/perl-libnet-3.110.0-r3::gentoo  0 KiB
    [ebuild  N     ] virtual/perl-Digest-SHA-6.20.0-r1::gentoo  0 KiB
    [ebuild  N     ] dev-perl/MailTools-2.190.0::gentoo  USE="-examples -test" 55 KiB
    [ebuild  N     ] dev-perl/Digest-HMAC-1.30.0-r1::gentoo  8 KiB
    [ebuild  N     ] dev-perl/Authen-SASL-2.160.0-r2::gentoo  USE="-kerberos -test" 45 KiB
    [ebuild  N     ] dev-perl/Error-0.170.250::gentoo  USE="-test" 32 KiB
    [ebuild  N     ] dev-vcs/git-2.26.2::gentoo  USE="blksha1 curl gpg iconv nls pcre pcre-jit perl threads webdav -cgi -cvs -doc -emacs -gnome-keyring -highlight (-libressl) -mediawiki -mediawiki-experimental -perforce (-ppcsha1) -subversion -test -tk -xinetd" PYTHON_SINGLE_TARGET="python3_8 -python3_7" 6,319 KiB
    
    Total: 10 packages (10 new), Size of downloads: 6,486 KiB

Install repoman via portage:

    gentoo /home/vagrant # emerge -pv app-portage/repoman
    
    These are the packages that would be merged, in order:
    
    Calculating dependencies... done!
    [ebuild  N     ] dev-python/cython-0.29.21-r1::gentoo  USE="-doc -emacs -test" PYTHON_TARGETS="python3_7 (-pypy3) -python3_8 -python3_9" 2,040 KiB
    [ebuild  N     ] dev-python/lxml-4.6.2-r1::gentoo  USE="threads -doc -examples -test" PYTHON_TARGETS="python3_7 (-pypy3) -python3_8 -python3_9" 927 KiB
    [ebuild  N     ] dev-libs/libyaml-0.2.5::gentoo  USE="-doc -static-libs -test" 84 KiB
    [ebuild  N     ] dev-python/pyyaml-5.4.1::gentoo  USE="libyaml -examples -test" PYTHON_TARGETS="python3_7 (-pypy3) -python3_8 -python3_9" 170 KiB
    [ebuild  N     ] app-portage/repoman-3.0.2::gentoo  PYTHON_TARGETS="python3_7 (-pypy3) -python3_8 -python3_9" 87 KiB
    
    Total: 5 packages (5 new), Size of downloads: 3,305 KiB

### 2.) Clone localrepo

Use git clone to download the repo structure into **/var/db/repos**:

    gentoo /var/db/repos # git clone https://github.com/mygentoo/localrepo.git
    Cloning into 'localrepo'...
    remote: Enumerating objects: 5, done.
    remote: Counting objects: 100% (5/5), done.
    remote: Compressing objects: 100% (3/3), done.
    remote: Total 5 (delta 0), reused 5 (delta 0), pack-reused 0
    Receiving objects: 100% (5/5), done.
    gentoo /var/db/repos # ls
    localrepo

