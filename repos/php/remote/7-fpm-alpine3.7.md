## `php:7-fpm-alpine3.7`

```console
$ docker pull php@sha256:8969cfe1fdd634c0e93342feaaa57c317421a6d73337c4be9d62e33ef37377b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `php:7-fpm-alpine3.7` - linux; amd64

```console
$ docker pull php@sha256:843bee4a8c14023a3423b96729b00900bd6ab4b406684aef013a3721c1221ea4
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30865907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f693f8f8b6dd18ed1a8363d08475491b7226a05eec55d46e7de8651f02aa718`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 01 Dec 2017 18:48:48 GMT
ADD file:2b00f26f6004576e2f8faeb3fb0517a14f79ea89a059fe096b54cbecf5da512e in / 
# Fri, 01 Dec 2017 18:48:48 GMT
CMD ["/bin/sh"]
# Wed, 13 Dec 2017 22:59:39 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 13 Dec 2017 22:59:43 GMT
RUN apk add --no-cache --virtual .persistent-deps 		ca-certificates 		curl 		tar 		xz 		libressl
# Wed, 13 Dec 2017 22:59:43 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Wed, 13 Dec 2017 22:59:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 13 Dec 2017 22:59:44 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Wed, 13 Dec 2017 23:12:25 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
# Wed, 13 Dec 2017 23:12:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Wed, 13 Dec 2017 23:12:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Wed, 13 Dec 2017 23:12:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 13 Dec 2017 23:12:26 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Wed, 13 Dec 2017 23:12:26 GMT
ENV PHP_VERSION=7.2.0
# Wed, 13 Dec 2017 23:12:33 GMT
ENV PHP_URL=https://secure.php.net/get/php-7.2.0.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-7.2.0.tar.xz.asc/from/this/mirror
# Wed, 13 Dec 2017 23:12:33 GMT
ENV PHP_SHA256=87572a6b924670a5d4aac276aaa4a94321936283df391d702c845ffc112db095 PHP_MD5=
# Wed, 13 Dec 2017 23:12:44 GMT
RUN set -xe; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del .fetch-deps
# Wed, 13 Dec 2017 23:12:49 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Wed, 13 Dec 2017 23:18:10 GMT
RUN set -xe 	&& apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		coreutils 		curl-dev 		libedit-dev 		libressl-dev 		libxml2-dev 		sqlite-dev 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .php-rundeps $runDeps 		&& apk del .build-deps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Thu, 04 Jan 2018 02:16:06 GMT
COPY multi:f9544e5c6b9d1d1292fca43464fe1e77b631547ac2baa8503de318853c0536d0 in /usr/local/bin/ 
# Thu, 04 Jan 2018 02:16:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Jan 2018 02:16:06 GMT
WORKDIR /var/www/html
# Thu, 04 Jan 2018 02:16:07 GMT
RUN set -ex 	&& cd /usr/local/etc 	&& if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi 	&& { 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf 	&& { 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = [::]:9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Jan 2018 02:16:15 GMT
EXPOSE 9000/tcp
# Thu, 04 Jan 2018 02:16:15 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2fdfe1cd78c20d05774f0919be19bc1a3e4729bce219968e4188e7e0f1af679d`  
		Last Modified: Fri, 01 Dec 2017 18:50:32 GMT  
		Size: 2.1 MB (2064911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db55124b382d0b037bfed2cad221c41eba0ab3b65991fdfdbeff7be2ccabf44`  
		Last Modified: Wed, 13 Dec 2017 23:42:01 GMT  
		Size: 1.3 MB (1261292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d2f8b7e6800365c78fe668b070929c105ffadc1e0b0d5055d15764f539fb6e`  
		Last Modified: Wed, 13 Dec 2017 23:42:00 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4db64004ca852ece7d3ba8a96345347177f96a07aa94c467eb8d1f0fccd9d`  
		Last Modified: Wed, 13 Dec 2017 23:41:59 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a2bc0c092b91059b3d72e65b31c368c212d39decd5fe8cf57565290ad80280`  
		Last Modified: Wed, 13 Dec 2017 23:43:23 GMT  
		Size: 12.0 MB (12033754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ef649733838cddc1f6c05f46c862cb07b8ad4338b0308eba72291fd7e563fe`  
		Last Modified: Wed, 13 Dec 2017 23:43:20 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b061f92948f05ab564a022d3b643da019def987a60bbe4e6350f770c949e8fb`  
		Last Modified: Wed, 13 Dec 2017 23:43:24 GMT  
		Size: 15.5 MB (15494033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f18c9d580e583f95303f62ede09d4c56a48b140f38ea3f68e528ba406c80cf4`  
		Last Modified: Thu, 04 Jan 2018 04:47:50 GMT  
		Size: 2.2 KB (2171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02afaaec09480542ad2fb8b62da98859b376cee601876215b7dca9af14e5e287`  
		Last Modified: Thu, 04 Jan 2018 04:47:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45da14d1e4d6cc4300cf386a2400b00ec3779e87bdea6062ae806aaf034bae37`  
		Last Modified: Thu, 04 Jan 2018 04:47:50 GMT  
		Size: 7.7 KB (7703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-fpm-alpine3.7` - linux; arm variant v6

```console
$ docker pull php@sha256:eb59f625cda729783bd42e85cdda97aa2ab8140391fdd64d595b2e9f3d1d296f
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29894177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5993b10aa504b55cf54e3d600777f903cc766dfafe4ec02bf70060676fe50949`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 01 Dec 2017 18:41:45 GMT
ADD file:966d84204dc4860e9281f7c93c792137c88298edb284f267def4b38a11b79a1f in / 
# Fri, 01 Dec 2017 18:41:45 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Fri, 01 Dec 2017 18:41:46 GMT
CMD ["/bin/sh"]
# Thu, 14 Dec 2017 06:16:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 14 Dec 2017 06:16:25 GMT
RUN apk add --no-cache --virtual .persistent-deps 		ca-certificates 		curl 		tar 		xz 		libressl
# Thu, 14 Dec 2017 06:16:26 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Thu, 14 Dec 2017 06:16:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 Dec 2017 06:16:27 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Thu, 14 Dec 2017 06:20:03 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
# Thu, 14 Dec 2017 06:20:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Thu, 14 Dec 2017 06:20:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Thu, 14 Dec 2017 06:20:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 14 Dec 2017 06:20:04 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 Dec 2017 06:20:05 GMT
ENV PHP_VERSION=7.2.0
# Thu, 14 Dec 2017 06:20:05 GMT
ENV PHP_URL=https://secure.php.net/get/php-7.2.0.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-7.2.0.tar.xz.asc/from/this/mirror
# Thu, 14 Dec 2017 06:20:05 GMT
ENV PHP_SHA256=87572a6b924670a5d4aac276aaa4a94321936283df391d702c845ffc112db095 PHP_MD5=
# Thu, 14 Dec 2017 06:20:21 GMT
RUN set -xe; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del .fetch-deps
# Thu, 14 Dec 2017 06:20:21 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Thu, 14 Dec 2017 06:23:19 GMT
RUN set -xe 	&& apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		coreutils 		curl-dev 		libedit-dev 		libressl-dev 		libxml2-dev 		sqlite-dev 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .php-rundeps $runDeps 		&& apk del .build-deps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Thu, 14 Dec 2017 06:23:20 GMT
COPY multi:2e4df9268ce870f9ed83b38a2784f3778f2c2468c3e7ee600220221534e4e247 in /usr/local/bin/ 
# Thu, 14 Dec 2017 06:23:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Dec 2017 06:23:20 GMT
WORKDIR /var/www/html
# Thu, 14 Dec 2017 06:23:21 GMT
RUN set -ex 	&& cd /usr/local/etc 	&& if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi 	&& { 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf 	&& { 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = [::]:9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 Dec 2017 06:23:21 GMT
EXPOSE 9000/tcp
# Thu, 14 Dec 2017 06:23:21 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:95d54dd4bdadebb53f9b91b25aa7dc5fcb83c534eb1d196eb0814aa1e16f3db2`  
		Last Modified: Fri, 01 Dec 2017 18:41:57 GMT  
		Size: 2.0 MB (2038298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bf7d76c39215a547858ef9260990b9b80c0e679bb2f6ceef942d7b6d0eeec3`  
		Last Modified: Fri, 01 Dec 2017 18:41:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8880c938078dc480cffb8bc5ca4e39f1b89405b7aea82998f3afae2e153b1d59`  
		Last Modified: Thu, 14 Dec 2017 06:27:25 GMT  
		Size: 1.3 MB (1251598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7de397e5174d91e4feaa94cd69316536a5ae6aea59880ed3bf8ca3500c4505c`  
		Last Modified: Thu, 14 Dec 2017 06:27:25 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b165a53a41e58e057e0b14778ae42782822d356e2a5bc0ce236a815bbdec0dd`  
		Last Modified: Thu, 14 Dec 2017 06:27:24 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0085b29261f2e6492f69d69ade80baca365e298ae5a38e0be924119684f83e`  
		Last Modified: Thu, 14 Dec 2017 06:27:47 GMT  
		Size: 12.0 MB (12033758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa837938f253a84edc8080417f5bccd97c3c96568f2cd02d9ada29825a24f105`  
		Last Modified: Thu, 14 Dec 2017 06:27:45 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac61d0d63599c0632f029f56605b1c3a0cfe8b8cf3dac1a6822d31edd65f618b`  
		Last Modified: Thu, 14 Dec 2017 06:27:50 GMT  
		Size: 14.6 MB (14558351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d189be04cc037cacf3f8611b51f058c9063f1ff779576003326e9f80511d8d`  
		Last Modified: Thu, 14 Dec 2017 06:27:44 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b51461e4f824e1a77764aadc8ae38cc65c87a856a18afcdc74135d25413ecd6`  
		Last Modified: Thu, 14 Dec 2017 06:27:45 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef96209e66de1a0c2e3a5581733eab8f3d8bdc7b183ec36ae5fe243fdcce09f`  
		Last Modified: Thu, 14 Dec 2017 06:27:44 GMT  
		Size: 7.7 KB (7697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-fpm-alpine3.7` - linux; arm64 variant v8

```console
$ docker pull php@sha256:8d23f1730b7015c3d22e80b25e29e4e6e8bf9d28861d604694806ee324df0ede
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29697906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d96b5f243513e5be3a7f338be3d2f8d1a017b85b6566f53e83062406abbefe`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 01 Dec 2017 18:42:42 GMT
ADD file:a6ef3cbbb1c0e5dfc6c3e41d70fd93e548594d9cb42c067e52df46d418c10a79 in / 
# Fri, 01 Dec 2017 18:42:42 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Fri, 01 Dec 2017 18:42:43 GMT
CMD ["/bin/sh"]
# Thu, 14 Dec 2017 03:34:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 14 Dec 2017 03:34:29 GMT
RUN apk add --no-cache --virtual .persistent-deps 		ca-certificates 		curl 		tar 		xz 		libressl
# Thu, 14 Dec 2017 03:34:31 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Thu, 14 Dec 2017 03:34:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 Dec 2017 03:34:34 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Thu, 14 Dec 2017 03:43:56 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
# Thu, 14 Dec 2017 03:43:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Thu, 14 Dec 2017 03:43:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Thu, 14 Dec 2017 03:43:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 14 Dec 2017 03:43:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 Dec 2017 03:44:00 GMT
ENV PHP_VERSION=7.2.0
# Thu, 14 Dec 2017 03:44:00 GMT
ENV PHP_URL=https://secure.php.net/get/php-7.2.0.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-7.2.0.tar.xz.asc/from/this/mirror
# Thu, 14 Dec 2017 03:44:01 GMT
ENV PHP_SHA256=87572a6b924670a5d4aac276aaa4a94321936283df391d702c845ffc112db095 PHP_MD5=
# Thu, 14 Dec 2017 03:44:15 GMT
RUN set -xe; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del .fetch-deps
# Thu, 14 Dec 2017 03:44:16 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Thu, 14 Dec 2017 03:51:58 GMT
RUN set -xe 	&& apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		coreutils 		curl-dev 		libedit-dev 		libressl-dev 		libxml2-dev 		sqlite-dev 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .php-rundeps $runDeps 		&& apk del .build-deps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Thu, 04 Jan 2018 03:32:58 GMT
COPY multi:f9544e5c6b9d1d1292fca43464fe1e77b631547ac2baa8503de318853c0536d0 in /usr/local/bin/ 
# Thu, 04 Jan 2018 03:32:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Jan 2018 03:32:59 GMT
WORKDIR /var/www/html
# Thu, 04 Jan 2018 03:33:01 GMT
RUN set -ex 	&& cd /usr/local/etc 	&& if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi 	&& { 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf 	&& { 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = [::]:9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Jan 2018 03:33:02 GMT
EXPOSE 9000/tcp
# Thu, 04 Jan 2018 03:33:03 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b78042c299ad99d1e646b18762d4bc22a84c4f88e5bb491ea6293a10f53ddf79`  
		Last Modified: Fri, 01 Dec 2017 18:43:42 GMT  
		Size: 2.0 MB (1988857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd45b97b6c2a3ac869ae5c99e087e97bc29714b165180e06f0c9116f400f2dd`  
		Last Modified: Fri, 01 Dec 2017 18:43:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fd85926acf4e07a36e9605843329449387bbfc1c1550485a341b4f87bfe40c`  
		Last Modified: Sat, 16 Dec 2017 16:37:16 GMT  
		Size: 1.2 MB (1214054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbd52b402d6ede87c727a4c39eca929bb27c7d5873fadd61ad1fc86752cc164`  
		Last Modified: Sat, 16 Dec 2017 16:37:15 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1ea5fa010452e4ef78628eebe6459b693eee1ec67ce04afd2ef50a2edee5fb`  
		Last Modified: Sat, 16 Dec 2017 16:37:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec12d4c8bcf505bfff2c9f18c525340f9d16cc7d538282108b65e7f087ea07f9`  
		Last Modified: Sat, 16 Dec 2017 16:38:11 GMT  
		Size: 12.0 MB (12033729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d729fe9c8e2918b30a6e6681bb5dbb41c3d26eb7f55f6c90a00f46da35a4e2`  
		Last Modified: Sat, 16 Dec 2017 16:38:08 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525c666c00a2fee1c991be787a6eb84cdebe9b3ea65e88fa7b76b063d8035cd1`  
		Last Modified: Sat, 16 Dec 2017 16:38:15 GMT  
		Size: 14.4 MB (14449175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8590a63a936b91ce8238a2ae3c410bcc47a97bf7c1367b580b163f54a3d1c5`  
		Last Modified: Thu, 04 Jan 2018 05:12:42 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650b9d7b367357a49cb69ae48fe4499740e9ca8b00dd80c406e4d42b9b2e86e6`  
		Last Modified: Thu, 04 Jan 2018 05:12:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dc40ae5f8d06cb7cbd247aa0684a4f23ee03a66a8d1c428803c17200f894f8`  
		Last Modified: Thu, 04 Jan 2018 05:12:43 GMT  
		Size: 7.7 KB (7702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-fpm-alpine3.7` - linux; 386

```console
$ docker pull php@sha256:23d431f99b91cd9cf3588107e05b919181a9d426c0b3f88dae00fcf677df8d86
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31476039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b6b189eec2dc7f5312505b1bcd33230d7634ea0f2b11b3cca3a5cfd54b7aa0a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 01 Dec 2017 18:46:48 GMT
ADD file:614c07101e677db9a4118a71c852a2be45a337d94c5bedfb48ae8c4cad21d625 in / 
# Fri, 01 Dec 2017 18:46:48 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Fri, 01 Dec 2017 18:46:48 GMT
CMD ["/bin/sh"]
# Thu, 14 Dec 2017 09:37:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 14 Dec 2017 09:37:56 GMT
RUN apk add --no-cache --virtual .persistent-deps 		ca-certificates 		curl 		tar 		xz 		libressl
# Thu, 14 Dec 2017 09:37:57 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Thu, 14 Dec 2017 09:37:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 Dec 2017 09:37:58 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Thu, 14 Dec 2017 09:52:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
# Thu, 14 Dec 2017 09:52:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Thu, 14 Dec 2017 09:52:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Thu, 14 Dec 2017 09:52:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 14 Dec 2017 09:52:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 Dec 2017 09:52:24 GMT
ENV PHP_VERSION=7.2.0
# Thu, 14 Dec 2017 09:52:24 GMT
ENV PHP_URL=https://secure.php.net/get/php-7.2.0.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-7.2.0.tar.xz.asc/from/this/mirror
# Thu, 14 Dec 2017 09:52:25 GMT
ENV PHP_SHA256=87572a6b924670a5d4aac276aaa4a94321936283df391d702c845ffc112db095 PHP_MD5=
# Thu, 14 Dec 2017 09:52:36 GMT
RUN set -xe; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del .fetch-deps
# Thu, 14 Dec 2017 09:52:36 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Thu, 14 Dec 2017 09:57:34 GMT
RUN set -xe 	&& apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		coreutils 		curl-dev 		libedit-dev 		libressl-dev 		libxml2-dev 		sqlite-dev 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .php-rundeps $runDeps 		&& apk del .build-deps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Thu, 14 Dec 2017 09:57:35 GMT
COPY multi:2e4df9268ce870f9ed83b38a2784f3778f2c2468c3e7ee600220221534e4e247 in /usr/local/bin/ 
# Thu, 14 Dec 2017 09:57:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Dec 2017 09:57:36 GMT
WORKDIR /var/www/html
# Thu, 14 Dec 2017 09:57:37 GMT
RUN set -ex 	&& cd /usr/local/etc 	&& if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi 	&& { 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf 	&& { 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = [::]:9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 Dec 2017 09:57:37 GMT
EXPOSE 9000/tcp
# Thu, 14 Dec 2017 09:57:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:381c1d4107a4401d75b916e6dc4331efddc01adac41f49eeaa711ab898606a1a`  
		Last Modified: Fri, 01 Dec 2017 18:47:24 GMT  
		Size: 2.1 MB (2126217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29cce73050e1b58c218a1c94cd8c9f719d38530500ab97333eac5fdaf385dbc`  
		Last Modified: Fri, 01 Dec 2017 18:47:24 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009841b1dd0b8a51b9063bfde115a677e8a792b7abe206fc0ff90e38a1ab96cf`  
		Last Modified: Thu, 14 Dec 2017 10:30:05 GMT  
		Size: 1.4 MB (1358856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45df78249718146d7dc2a61b02ee84aae71835fcf910a2096e6aa61818bb2cda`  
		Last Modified: Thu, 14 Dec 2017 10:30:04 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60be3451b72481126ebb2c5b6549d1b7148228dac44bf5ade7c7f36c332bef1c`  
		Last Modified: Thu, 14 Dec 2017 10:30:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe7881a2b3c77697ee831adcfed83a2525a92e1aab32860532329233d3e938f`  
		Last Modified: Thu, 14 Dec 2017 10:31:40 GMT  
		Size: 12.0 MB (12033753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d76bd651cb306495337b3c0718a6db5df6ab37041e97d98dd49f9feea62159e`  
		Last Modified: Thu, 14 Dec 2017 10:31:39 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7041bad9f143c5023f127ec6e4d0428fe53eb9b50354d38923dfff7331c2b42`  
		Last Modified: Thu, 14 Dec 2017 10:31:45 GMT  
		Size: 15.9 MB (15945130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f8300d0b2862cf9247d99aeb8d2ded4043dd0987d81d1c6181302a965523a0`  
		Last Modified: Thu, 14 Dec 2017 10:31:39 GMT  
		Size: 2.2 KB (2169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4f80538afadaba4ecf93c35f50b82705ca3791fb783bbe73ecc4e92a6c39ea`  
		Last Modified: Thu, 14 Dec 2017 10:31:39 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b20ac8866cbcebbbb80b83ec42a704dd64ddaff441bc04af1893f90f676b03`  
		Last Modified: Thu, 14 Dec 2017 10:31:39 GMT  
		Size: 7.7 KB (7695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-fpm-alpine3.7` - linux; ppc64le

```console
$ docker pull php@sha256:532c88b385d1e8c86e14d0a3aad4685d943021fa58e5653b37ec1f83d10e1e28
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30652443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d710a20cae2a6d89124f718baf34309a63f6b2493957a7a1d57e9fac47b211`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 01 Dec 2017 18:41:54 GMT
ADD file:791370adae5cfa8feec749693f5a995a01f58f0462b7aa675fc5bf991e1282b5 in / 
# Fri, 01 Dec 2017 18:41:55 GMT
COPY file:0f1d36dd7d8d53613b275660a88c5bf9b608ea8aa73a8054cb8bdbd73fd971ac in /etc/localtime 
# Fri, 01 Dec 2017 18:41:57 GMT
CMD ["/bin/sh"]
# Thu, 14 Dec 2017 09:49:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 14 Dec 2017 09:50:02 GMT
RUN apk add --no-cache --virtual .persistent-deps 		ca-certificates 		curl 		tar 		xz 		libressl
# Thu, 14 Dec 2017 09:50:06 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Thu, 14 Dec 2017 09:50:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 Dec 2017 09:50:10 GMT
RUN mkdir -p $PHP_INI_DIR/conf.d
# Thu, 14 Dec 2017 09:55:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data
# Thu, 14 Dec 2017 09:55:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Thu, 14 Dec 2017 09:55:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2
# Thu, 14 Dec 2017 09:55:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 14 Dec 2017 09:55:06 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 Dec 2017 09:55:09 GMT
ENV PHP_VERSION=7.2.0
# Thu, 14 Dec 2017 09:55:10 GMT
ENV PHP_URL=https://secure.php.net/get/php-7.2.0.tar.xz/from/this/mirror PHP_ASC_URL=https://secure.php.net/get/php-7.2.0.tar.xz.asc/from/this/mirror
# Thu, 14 Dec 2017 09:55:11 GMT
ENV PHP_SHA256=87572a6b924670a5d4aac276aaa4a94321936283df391d702c845ffc112db095 PHP_MD5=
# Thu, 14 Dec 2017 09:55:26 GMT
RUN set -xe; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		mkdir -p /usr/src; 	cd /usr/src; 		wget -O php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		wget -O php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del .fetch-deps
# Thu, 14 Dec 2017 09:55:27 GMT
COPY file:207c686e3fed4f71f8a7b245d8dcae9c9048d276a326d82b553c12a90af0c0ca in /usr/local/bin/ 
# Thu, 14 Dec 2017 09:59:06 GMT
RUN set -xe 	&& apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		coreutils 		curl-dev 		libedit-dev 		libressl-dev 		libxml2-dev 		sqlite-dev 		&& export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	&& docker-php-source extract 	&& cd /usr/src/php 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& ./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--disable-cgi 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 				$PHP_EXTRA_CONFIGURE_ARGS 	&& make -j "$(nproc)" 	&& make install 	&& { find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; } 	&& make clean 	&& cd / 	&& docker-php-source delete 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .php-rundeps $runDeps 		&& apk del .build-deps 		&& pecl update-channels 	&& rm -rf /tmp/pear ~/.pearrc
# Thu, 14 Dec 2017 09:59:08 GMT
COPY multi:2e4df9268ce870f9ed83b38a2784f3778f2c2468c3e7ee600220221534e4e247 in /usr/local/bin/ 
# Thu, 14 Dec 2017 09:59:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Dec 2017 09:59:11 GMT
WORKDIR /var/www/html
# Thu, 14 Dec 2017 09:59:15 GMT
RUN set -ex 	&& cd /usr/local/etc 	&& if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi 	&& { 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf 	&& { 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = [::]:9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 Dec 2017 09:59:17 GMT
EXPOSE 9000/tcp
# Thu, 14 Dec 2017 09:59:18 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0da653ea85b50d280ec56ca2eafb7e8b37590630356e043fa9ff162d55732a23`  
		Last Modified: Fri, 01 Dec 2017 18:42:14 GMT  
		Size: 2.1 MB (2081469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd90b777cc38b5b6ca1b2407e647fdc22ef31b57ef98e924e7e0635adffc385`  
		Last Modified: Fri, 01 Dec 2017 18:42:15 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcb39b8c697dd02c12a952dcc63b609d7c7bf9d66e93e5e4913d2eeeaf894d3`  
		Last Modified: Thu, 14 Dec 2017 10:14:08 GMT  
		Size: 1.3 MB (1256438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a484a708d295b3464c467d2a9bd8343046d4f4905c5776958832b3f6754c2f6`  
		Last Modified: Thu, 14 Dec 2017 10:14:07 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b360613871987866ea7defe9eb40283e850669f1475e97eb519e25f1f522df28`  
		Last Modified: Thu, 14 Dec 2017 10:14:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94925ceb9c0bbeacb0918f180267c33ce1c31e15df27765423ea022ee1fa6c5`  
		Last Modified: Thu, 14 Dec 2017 10:15:10 GMT  
		Size: 12.0 MB (12033782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fc6bd91a0ead0604a7295c7563bbcf4bee489d122e574ef9fe3c35f5fcc16d`  
		Last Modified: Thu, 14 Dec 2017 10:15:01 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8cb28279e990161dc8452267d6561177dbd51234e60e0fa8cbacf18e9301acd`  
		Last Modified: Thu, 14 Dec 2017 10:15:06 GMT  
		Size: 15.3 MB (15268579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a015065bf6901688f5bc40e6d34420aa37130c8fec09379dd5b3e75757338092`  
		Last Modified: Thu, 14 Dec 2017 10:15:02 GMT  
		Size: 2.2 KB (2170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cff4edebed212d40069c54189a913f55bd77adf51c7bbb906a6233735f83cb`  
		Last Modified: Thu, 14 Dec 2017 10:15:01 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ff97542b4bb7e23d82703a7661eaa5859537b56c4893a78533fb305826cf9`  
		Last Modified: Thu, 14 Dec 2017 10:15:02 GMT  
		Size: 7.7 KB (7697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
