## `ghost:1-alpine`

```console
$ docker pull ghost@sha256:9c9741ce3545c4c443fec4cde1b76153dace571466eb436aaa7ee68685ad7ae0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ghost:1-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:935c376835ebbba7dfbf8d59fd201a4d73b16cccb839c80904316e0d2f0ad692
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141111474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43b540ff6be2c65868ce9d0cd2dddf9582fa37d549995036ffa07758b5d88650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 01 Dec 2017 18:49:44 GMT
ADD file:c05a199f603e2a97ea93d9f6cc210a1c8ab27eda35f3613722bfcf697da36483 in / 
# Fri, 01 Dec 2017 18:49:45 GMT
CMD ["/bin/sh"]
# Wed, 03 Jan 2018 19:36:58 GMT
ENV NODE_VERSION=6.12.3
# Wed, 03 Jan 2018 19:48:47 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         binutils-gold         curl         g++         gcc         gnupg         libgcc         linux-headers         make         python   && for key in     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     B9AE9905FFD7803F25714661B63B535A4C206CA9     56730D5401028683275BD23C23EFEFE93C4CFFFE     77984A986EBC2AA786BC0F66B01FBB92821C587A   ; do     gpg --keyserver pgp.mit.edu --recv-keys "$key" ||     gpg --keyserver keyserver.pgp.com --recv-keys "$key" ||     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ;   done     && curl -SLO "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -SLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN)     && make install     && apk del .build-deps     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt
# Wed, 03 Jan 2018 19:48:47 GMT
ENV YARN_VERSION=1.3.2
# Wed, 03 Jan 2018 19:48:56 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --keyserver pgp.mit.edu --recv-keys "$key" ||     gpg --keyserver keyserver.pgp.com --recv-keys "$key" ||     gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ;   done   && curl -fSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt/yarn   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/yarn --strip-components=1   && ln -s /opt/yarn/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn/bin/yarn /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 03 Jan 2018 19:48:56 GMT
CMD ["node"]
# Wed, 03 Jan 2018 20:36:52 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 03 Jan 2018 20:36:55 GMT
RUN apk add --no-cache 		bash
# Wed, 03 Jan 2018 20:36:56 GMT
ENV NODE_ENV=production
# Wed, 03 Jan 2018 20:36:56 GMT
ENV GHOST_CLI_VERSION=1.4.1
# Wed, 03 Jan 2018 20:37:18 GMT
RUN npm install -g "ghost-cli@$GHOST_CLI_VERSION"
# Wed, 03 Jan 2018 20:37:19 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 03 Jan 2018 20:37:19 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 03 Jan 2018 23:46:41 GMT
ENV GHOST_VERSION=1.19.1
# Wed, 03 Jan 2018 23:47:31 GMT
RUN set -ex; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		"$GHOST_INSTALL/current/node_modules/knex-migrator/bin/knex-migrator" --version
# Wed, 03 Jan 2018 23:54:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/var/lib/ghost/current/node_modules/knex-migrator/bin
# Wed, 03 Jan 2018 23:54:54 GMT
WORKDIR /var/lib/ghost
# Wed, 03 Jan 2018 23:54:54 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 03 Jan 2018 23:54:55 GMT
COPY file:fe4f8ce065580d78daf2ea3ae3ab9174f3edd7740df8b95889926dc1cdfe77b0 in /usr/local/bin 
# Wed, 03 Jan 2018 23:54:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Jan 2018 23:54:55 GMT
EXPOSE 2368/tcp
# Wed, 03 Jan 2018 23:54:55 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:ab7e51e37a183df284512426b1cb56d0404532b6011c823f35127c796fb97b13`  
		Last Modified: Fri, 01 Dec 2017 18:58:11 GMT  
		Size: 2.4 MB (2387532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c27b0dcc9bf200d7d01f5d74069b46a6d0b7140cb9efaa2790fb0596d2ea27`  
		Last Modified: Wed, 03 Jan 2018 20:06:01 GMT  
		Size: 15.5 MB (15457842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587c169b3f90fea8e468a46b07f614e31971903339625f68eb740c24eefa7058`  
		Last Modified: Wed, 03 Jan 2018 20:05:56 GMT  
		Size: 1.0 MB (1017575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87133e6fc11b0ea089ef9677f3de32bd4661deb115763523dfc12770f23ad704`  
		Last Modified: Wed, 03 Jan 2018 20:52:02 GMT  
		Size: 8.4 KB (8363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f5abc017d23e317904675eb8773b14bc82897f1b08e61ac235dc2c8e8af014`  
		Last Modified: Wed, 03 Jan 2018 20:52:06 GMT  
		Size: 1.1 MB (1112416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1361013706d003433939eaf8bb83a479283d1aa3d99af180143f7a193c247c95`  
		Last Modified: Wed, 03 Jan 2018 20:52:21 GMT  
		Size: 19.1 MB (19123562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebaa545376312a80a32c90d72576267acd4e95579af343ef48dd8b74469b9c`  
		Last Modified: Wed, 03 Jan 2018 23:57:36 GMT  
		Size: 102.0 MB (102003624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e51320b88b6e89d716296795409fa19798ddfe5377c2cc6a94678ce820cfe6e`  
		Last Modified: Wed, 03 Jan 2018 23:57:00 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
