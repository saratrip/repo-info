## `gradle:jdk7-alpine`

```console
$ docker pull gradle@sha256:0a8388963573857e2e845d5b8264dbe048d99d9257d86b9d829b4f5817b55e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `gradle:jdk7-alpine` - linux; amd64

```console
$ docker pull gradle@sha256:93f8d21185ebb4a8d6c904be931c0113d86025acb9b09397921d9c376d5e2904
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155304881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d979198d32f9dbf3f92681c16d0d0db10f05b5a6d6a401819c0f1b0d9d87f6d4`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 01 Dec 2017 18:48:48 GMT
ADD file:2b00f26f6004576e2f8faeb3fb0517a14f79ea89a059fe096b54cbecf5da512e in / 
# Fri, 01 Dec 2017 18:48:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Dec 2017 03:42:44 GMT
ENV LANG=C.UTF-8
# Tue, 05 Dec 2017 03:42:45 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 05 Dec 2017 03:42:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.7-openjdk
# Tue, 05 Dec 2017 03:42:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/java-1.7-openjdk/jre/bin:/usr/lib/jvm/java-1.7-openjdk/bin
# Tue, 05 Dec 2017 03:42:46 GMT
ENV JAVA_VERSION=7u151
# Tue, 05 Dec 2017 03:42:46 GMT
ENV JAVA_ALPINE_VERSION=7.151.2.6.11-r0
# Tue, 05 Dec 2017 03:43:03 GMT
RUN set -x 	&& apk add --no-cache 		openjdk7="$JAVA_ALPINE_VERSION" 	&& [ "$JAVA_HOME" = "$(docker-java-home)" ]
# Tue, 05 Dec 2017 04:38:11 GMT
CMD ["gradle"]
# Tue, 05 Dec 2017 04:38:11 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 21 Dec 2017 01:16:23 GMT
ENV GRADLE_VERSION=4.4.1
# Thu, 21 Dec 2017 01:16:24 GMT
ARG GRADLE_DOWNLOAD_SHA256=e7cf7d1853dfc30c1c44f571d3919eeeedef002823b66b6a988d27e919686389
# Thu, 21 Dec 2017 01:16:30 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=e7cf7d1853dfc30c1c44f571d3919eeeedef002823b66b6a988d27e919686389
RUN set -o errexit -o nounset 	&& echo "Installing build dependencies" 	&& apk add --no-cache --virtual .build-deps 		ca-certificates 		openssl 		unzip 		&& echo "Downloading Gradle" 	&& wget -O gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip" 		&& echo "Checking download hash" 	&& echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum -c - 		&& echo "Installing Gradle" 	&& unzip gradle.zip 	&& rm gradle.zip 	&& mkdir /opt 	&& mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/" 	&& ln -s "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle 		&& apk del .build-deps 		&& echo "Adding gradle user and group" 	&& addgroup -S -g 1000 gradle 	&& adduser -D -S -G gradle -u 1000 -s /bin/ash gradle 	&& mkdir /home/gradle/.gradle 	&& chown -R gradle:gradle /home/gradle 		&& echo "Symlinking root Gradle cache to gradle Gradle cache" 	&& ln -s /home/gradle/.gradle /root/.gradle
# Thu, 21 Dec 2017 01:16:30 GMT
USER [gradle]
# Thu, 21 Dec 2017 01:16:30 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 21 Dec 2017 01:16:31 GMT
WORKDIR /home/gradle
# Thu, 21 Dec 2017 01:16:34 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=e7cf7d1853dfc30c1c44f571d3919eeeedef002823b66b6a988d27e919686389
RUN set -o errexit -o nounset 	&& echo "Testing Gradle installation" 	&& gradle --version
```

-	Layers:
	-	`sha256:2fdfe1cd78c20d05774f0919be19bc1a3e4729bce219968e4188e7e0f1af679d`  
		Last Modified: Fri, 01 Dec 2017 18:50:32 GMT  
		Size: 2.1 MB (2064911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82630fd6e5ba7225587bd7986c7b6245801f8c7b001c9db318aecbb7fcb188a4`  
		Last Modified: Tue, 05 Dec 2017 03:44:19 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5176a718d97095c6e24a35aff7276746d1ef705923fe2c0e2775e0b312029e7`  
		Last Modified: Tue, 05 Dec 2017 03:44:30 GMT  
		Size: 77.4 MB (77404229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e3d8c6343b0b1e0a175435b3dcea0193eb9b4702314a9adfa0ba183a3f77cf`  
		Last Modified: Thu, 21 Dec 2017 01:26:35 GMT  
		Size: 75.8 MB (75835363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15100e068277e1a82fcc6b73166180b5b7cbde9689c3c9fb78ca555cc43f5ca2`  
		Last Modified: Thu, 21 Dec 2017 01:26:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
