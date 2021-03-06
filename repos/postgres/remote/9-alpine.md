## `postgres:9-alpine`

```console
$ docker pull postgres@sha256:02b8d708a3cfc0bc9f6bd955daba2e8d36d460f68789dbe4e04c31878735684d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `postgres:9-alpine` - linux; amd64

```console
$ docker pull postgres@sha256:db0fad337a95d178350169549e0ac1874af430bd77a8533a5b03542aa31cdd12
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14691783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23c1fbd604c024134f41e291293e645f1ab692088953be06121d6e8077f87e4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 01 Dec 2017 18:49:59 GMT
ADD file:5595f8b7042388f1c3d5642b8581698548f99ea2f0b9324f797d2396e03e00cb in / 
# Fri, 01 Dec 2017 18:49:59 GMT
CMD ["/bin/sh"]
# Mon, 04 Dec 2017 16:10:18 GMT
RUN set -ex; 	postgresHome="$(getent passwd postgres)"; 	postgresHome="$(echo "$postgresHome" | cut -d: -f6)"; 	[ "$postgresHome" = '/var/lib/postgresql' ]; 	mkdir -p "$postgresHome"; 	chown -R postgres:postgres "$postgresHome"
# Mon, 04 Dec 2017 16:10:19 GMT
ENV LANG=en_US.utf8
# Mon, 04 Dec 2017 16:10:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 04 Dec 2017 16:10:20 GMT
ENV PG_MAJOR=9.6
# Mon, 04 Dec 2017 16:10:20 GMT
ENV PG_VERSION=9.6.6
# Mon, 04 Dec 2017 16:10:20 GMT
ENV PG_SHA256=399cdffcb872f785ba67e25d275463d74521566318cfef8fe219050d063c8154
# Mon, 04 Dec 2017 16:12:57 GMT
RUN set -ex 		&& apk add --no-cache --virtual .fetch-deps 		ca-certificates 		openssl 		tar 		&& wget -O postgresql.tar.bz2 "https://ftp.postgresql.org/pub/source/v$PG_VERSION/postgresql-$PG_VERSION.tar.bz2" 	&& echo "$PG_SHA256 *postgresql.tar.bz2" | sha256sum -c - 	&& mkdir -p /usr/src/postgresql 	&& tar 		--extract 		--file postgresql.tar.bz2 		--directory /usr/src/postgresql 		--strip-components 1 	&& rm postgresql.tar.bz2 		&& apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		flex 		gcc 		libc-dev 		libedit-dev 		libxml2-dev 		libxslt-dev 		make 		openssl-dev 		perl 		perl-ipc-run 		util-linux-dev 		zlib-dev 		&& cd /usr/src/postgresql 	&& awk '$1 == "#define" && $2 == "DEFAULT_PGSOCKET_DIR" && $3 == "\"/tmp\"" { $3 = "\"/var/run/postgresql\""; print; next } { print }' src/include/pg_config_manual.h > src/include/pg_config_manual.h.new 	&& grep '/var/run/postgresql' src/include/pg_config_manual.h.new 	&& mv src/include/pg_config_manual.h.new src/include/pg_config_manual.h 	&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& wget -O config/config.guess 'https://git.savannah.gnu.org/cgit/config.git/plain/config.guess?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& wget -O config/config.sub 'https://git.savannah.gnu.org/cgit/config.git/plain/config.sub?id=7d3d27baf8107b630586c962c057e22149653deb' 	&& ./configure 		--build="$gnuArch" 		--enable-integer-datetimes 		--enable-thread-safety 		--enable-tap-tests 		--disable-rpath 		--with-uuid=e2fs 		--with-gnu-ld 		--with-pgport=5432 		--with-system-tzdata=/usr/share/zoneinfo 		--prefix=/usr/local 		--with-includes=/usr/local/include 		--with-libraries=/usr/local/lib 				--with-openssl 		--with-libxml 		--with-libxslt 	&& make -j "$(nproc)" world 	&& make install-world 	&& make -C contrib install 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-cache --virtual .postgresql-rundeps 		$runDeps 		bash 		su-exec 		tzdata 	&& apk del .fetch-deps .build-deps 	&& cd / 	&& rm -rf 		/usr/src/postgresql 		/usr/local/share/doc 		/usr/local/share/man 	&& find /usr/local -name '*.a' -delete
# Mon, 04 Dec 2017 16:12:57 GMT
RUN sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/local/share/postgresql/postgresql.conf.sample
# Mon, 04 Dec 2017 16:13:03 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 04 Dec 2017 16:13:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 04 Dec 2017 16:13:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # this 777 will be replaced by 700 at runtime (allows semi-arbitrary "--user" values)
# Mon, 04 Dec 2017 16:13:08 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 04 Dec 2017 16:13:09 GMT
COPY file:d5038a27fbcfa2f7c3a5e92ffdbfda1676a7a65ecb52a9b377a6041a59e1c1d7 in /usr/local/bin/ 
# Mon, 04 Dec 2017 16:13:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 04 Dec 2017 16:13:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2017 16:13:10 GMT
EXPOSE 5432/tcp
# Mon, 04 Dec 2017 16:13:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:128191993b8a5e9d949346160926359ad02df93bde62f5af8a7bc3573f53553e`  
		Last Modified: Fri, 01 Dec 2017 18:58:25 GMT  
		Size: 2.0 MB (1970107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f0449cfc1a8855b4b35387faf3a181e8cfe4c8c2bb985abc4169ce9ced2e7`  
		Last Modified: Mon, 04 Dec 2017 16:23:41 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1af663c14438cb6f70c996b08c05e850621c235d0cb810888802bf5650edb7`  
		Last Modified: Mon, 04 Dec 2017 16:23:41 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51085086e4e33f4bb80b0cf8c54e53e96f349926b770c0aeb8b6675d64250c5`  
		Last Modified: Mon, 04 Dec 2017 16:23:46 GMT  
		Size: 12.7 MB (12712099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8064a0d2f685aab0debb53d323539dc6f523b9a2319f1822ca3f54450fd9258b`  
		Last Modified: Mon, 04 Dec 2017 16:23:38 GMT  
		Size: 7.1 KB (7071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d17009f2aaf09ba4c64dbdfe0c0622e839469d60cd1d7a1233a4c436e36361`  
		Last Modified: Mon, 04 Dec 2017 16:23:38 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0435ce4d7b9458071514ba2c9496316e4d395f4a81f3eedc89e84cbacc033932`  
		Last Modified: Mon, 04 Dec 2017 16:23:38 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c1a5e0fa9fefe236f03cb7a4e880e84af1ac1d2f59449a9135d3bb1a38d339`  
		Last Modified: Mon, 04 Dec 2017 16:23:39 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481b2e72aa80c0ddc1e076b53978141210190cf104a466d8d697b214fd8cb7f6`  
		Last Modified: Mon, 04 Dec 2017 16:23:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
