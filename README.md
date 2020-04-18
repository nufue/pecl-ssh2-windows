PECL SSH2 extension compiled for Windows
=================================

This repository contains `php_ssh2` extension compiled for use on Windows.
**You are encouraged to use official PECL build of version 1.2 -** https://pecl.php.net/package/ssh2/1.2/windows


PHP 7.3
--------------------
Based on pecl/ssh2 commit [79371dc05ff34e58f796e6755e25ba91c169ac1a](http://git.php.net/?p=pecl/networking/ssh2.git;a=commit;h=79371dc05ff34e58f796e6755e25ba91c169ac1a) (b/c pecl/ssh2 version 1.1.2 does not build correctly on MSVC15 - compiler error C2088).

Compiler version: VC15

| Architecture | x86 | x64 |
|---|---|---|
| TS (thread-safe) | [php_ssh2.dll](7.3/vc15-x86/php_ssh2.dll) | [php_ssh2.dll](7.3/vc15-x64/php_ssh2.dll) |
| NTS (non-thread-safe) | [php_ssh2_nts.dll](7.3/vc15-x86/php_ssh2_nts.dll) | [php_ssh2_nts.dll](7.3/vc15-x64/php_ssh2_nts.dll) |

PHP 7.2
--------------------
Based on pecl/ssh2 version [1.1.2](http://pecl.php.net/package/ssh2/1.1.2).

Compiler version: VC15

| Architecture | x86 | x64 |
|---|---|---|
| TS (thread-safe) | [php_ssh2.dll](7.2/vc15-x86/php_ssh2.dll) | [php_ssh2.dll](7.2/vc15-x64/php_ssh2.dll) |
| NTS (non-thread-safe) | [php_ssh2_nts.dll](7.2/vc15-x86/php_ssh2_nts.dll) | [php_ssh2_nts.dll](7.2/vc15-x64/php_ssh2_nts.dll) |  

Notes on compiling - commands used
-------------------
TS: `configure --disable-all --enable-cli --with-ssh2=shared --enable-zlib --with-openssl`

NTS: `configure --disable-all --enable-cli --with-ssh2=shared --enable-zlib --with-openssl --disable-zts`
