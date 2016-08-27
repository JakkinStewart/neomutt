Requirements
============

- GCC
- curses library (ncurses or slang)
- libiconv
- OpenSSL (if installing --with-ssl)

Installation
============

Installing Mutt only has a few steps.

`./prepare --use-the-arguments-below`

`make`

And if you want it installed.

`make install`

The "prepare" script doesn't enable a lot of useful stuff by default.

The most common arguments are listed below. Keep in mind, these are recommendations. You may need fewer configurations or more, depending on your situation.

  --enable-gpgme          			Enable GPGME support
  --enable-sidebar        			Enable Sidebar support
  --enable-compressed     			Enable compressed folders support
  --enable-notmuch        			Enable NOTMUCH support
  --enable-pop            			Enable POP3 support
  --enable-imap           			Enable IMAP support
  --enable-smtp           			include internal SMTP relay support
  --with-curses=DIR       			Where ncurses is installed (generally under /usr )
  --with-idn=[PFX]        			Use GNU libidn for internationalized domain names
  --with-ssl[=PFX]        			Enable TLS support using OpenSSL
  --with-gnutls[=PFX]     			enable TLS support using gnutls
  --with-sasl[=PFX]       			Use SASL network security library


The rest of the included configuration's are listed here:

  --prefix=PREFIX         			install architecture-independent files in PREFIX [/usr/local]
  --exec-prefix=EPREFIX   			install architecture-dependent files in EPREFIX
  --bindir=DIR            			user executables [EPREFIX/bin]
  --sbindir=DIR           			system admin executables [EPREFIX/sbin]
  --libexecdir=DIR        			program executables [EPREFIX/libexec]
  --sysconfdir=DIR        			read-only single-machine data [PREFIX/etc]
  --sharedstatedir=DIR    			modifiable architecture-independent data [PREFIX/com]
  --localstatedir=DIR     			modifiable single-machine data [PREFIX/var]
  --libdir=DIR            			object code libraries [EPREFIX/lib]
  --includedir=DIR        			C header files [PREFIX/include]
  --oldincludedir=DIR     			C header files for non-gcc [/usr/include]
  --datarootdir=DIR       			read-only arch.-independent data root [PREFIX/share]
  --datadir=DIR           			read-only architecture-independent data [DATAROOTDIR]
  --infodir=DIR           			info documentation [DATAROOTDIR/info]
  --localedir=DIR         			locale-dependent data [DATAROOTDIR/locale]
  --mandir=DIR            			man documentation [DATAROOTDIR/man]
  --docdir=DIR            			documentation root [DATAROOTDIR/doc/neomutt]
  --htmldir=DIR           			html documentation [DOCDIR]
  --dvidir=DIR            			dvi documentation [DOCDIR]
  --pdfdir=DIR            			pdf documentation [DOCDIR]
  --psdir=DIR             			ps documentation [DOCDIR]
  --program-prefix=PREFIX           prepend PREFIX to installed program names
  --program-suffix=SUFFIX           append SUFFIX to installed program names
  --program-transform-name=PROGRAM  run sed PROGRAM on installed program names
  --build=BUILD 					configure for building on BUILD [guessed]
  --host=HOST       				cross-compile to build programs to run on HOST [BUILD]
  --disable-option-checking 		ignore unrecognized --enable/--with options
  --disable-FEATURE       			do not include FEATURE (same as --enable-FEATURE=no)
  --enable-FEATURE[=ARG]  			include FEATURE [ARG=yes]
  --enable-silent-rules   			less verbose build output (undo: "make V=1")
  --disable-silent-rules  			verbose build output (undo: "make V=0")
  --enable-dependency-tracking      do not reject slow dependency extractors
  --disable-dependency-tracking     speeds up one-time build
  --disable-largefile     			omit support for large files
  --disable-pgp           			Disable PGP support
  --disable-smime         			Disable SMIME support
  --enable-external-dotlock 		Force use of an external dotlock program
  --enable-nntp           			Enable NNTP support
  --enable-debug          			Enable debugging support
  --enable-flock          			Use flock() to lock files
  --disable-fcntl         			Do NOT use fcntl() to lock files
  --disable-warnings      			Turn off compiler warnings (not recommended)
  --enable-nfs-fix        			Work around an NFS with broken attributes caching
  --enable-mailtool       			Enable Sun mailtool attachments support
  --enable-locales-fix    			The result of isprint() is unreliable
  --enable-exact-address  			Enable regeneration of email addresses
  --enable-hcache         			Enable header caching
  --disable-iconv         			Disable iconv support
  --disable-nls           			Do not use Native Language Support
  --disable-fmemopen      			Do NOT use fmemopen
  --disable-full-doc      			Omit disabled variables
  --with-PACKAGE[=ARG]    			use PACKAGE [ARG=yes]
  --without-PACKAGE       			do not use PACKAGE (same as --with-PACKAGE=no)
  --with-gpgme-prefix=PFX 			prefix where GPGME is installed (optional)
  --with-mixmaster[=PATH] 			Include Mixmaster support
  --with-slang[=DIR]      			Use S-Lang instead of ncurses
  --with-regex            			Use the GNU regex library
  --with-homespool[=FILE] 			File in user's directory where new mail is spooled
  --with-mailpath=DIR     			Directory where spool mailboxes are located
  --with-docdir=PATH      			Specify where to put the documentation
  --with-domain=DOMAIN    			Specify your DNS domain name
  --with-gss[=PFX]        			Compile in GSSAPI authentication for IMAP
  --with-exec-shell=SHELL 			Specify alternate shell (ONLY if /bin/sh is broken)
  --without-tokyocabinet  			Don't use tokyocabinet even if it is available
  --without-qdbm          			Don't use qdbm even if it is available
  --without-gdbm          			Don't use gdbm even if it is available
  --with-bdb[=DIR]        			Use BerkeleyDB4 if gdbm is not available
  --with-lmdb[=DIR]       			Use LMDB if gdbm is not available
  --with-libiconv-prefix[=DIR] 		Search for libiconv in DIR/include and DIR/lib
  --with-included-gettext 			Use the GNU gettext library included here
  --without-wc-funcs      			Do not use the system's wchar_t functions [PREFIX]

Report bugs to <https://github.com/neomutt/neomutt/issues>.
NeoMutt home page: <http://www.neomutt.org>.
