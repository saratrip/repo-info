## `maven:3-jdk-9`

```console
$ docker pull maven@sha256:591f12e676ded930b5305620e9464e6661fa48dc0c03883e45e5eb74ed2369c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `maven:3-jdk-9` - linux; amd64

```console
$ docker pull maven@sha256:2c40777e4daa65667abfe0a8c191f1798867dc78749084757d2980cb3b580707
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.5 MB (409501301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:809114416854705e17024554bf0f6765676cd6d6f45263766f2fe5a2b0b83e37`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Dec 2017 01:43:09 GMT
ADD file:f4f0ede88e0b0edf8235b2a5ff46ab7d8de71d56720cb7dc3032bca0e1872695 in / 
# Tue, 12 Dec 2017 01:43:10 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:51:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:51:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 07:51:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:25:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:25:35 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:25:36 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 15:25:37 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 15:25:37 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Dec 2017 15:25:38 GMT
ENV JAVA_VERSION=9.0.1+11
# Tue, 12 Dec 2017 15:25:38 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Tue, 12 Dec 2017 15:27:37 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Tue, 12 Dec 2017 15:27:38 GMT
CMD ["jshell"]
# Tue, 12 Dec 2017 19:19:11 GMT
ARG MAVEN_VERSION=3.5.2
# Tue, 12 Dec 2017 19:19:11 GMT
ARG USER_HOME_DIR=/root
# Tue, 12 Dec 2017 19:19:11 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Tue, 12 Dec 2017 19:19:12 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Tue, 12 Dec 2017 19:19:13 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN ln -s /etc/java-9-openjdk /usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)/conf
# Tue, 12 Dec 2017 19:19:15 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 12 Dec 2017 19:19:21 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 12 Dec 2017 19:19:22 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 12 Dec 2017 19:20:03 GMT
COPY file:fb726a12bbbf8ff54c8d9fceef4fa3018c11a435bfa04ee5f73156c544907861 in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 12 Dec 2017 19:20:03 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 12 Dec 2017 19:20:03 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 12 Dec 2017 19:20:04 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a8797cd0c76e8b1532d95708a0a38554c89e6fa0cdd856dbede8555225cdea00`  
		Last Modified: Tue, 12 Dec 2017 01:51:30 GMT  
		Size: 48.4 MB (48429060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdce62b256df9c745afac618b5a44d73531cede1a187586e73ed27bd7e1c508`  
		Last Modified: Tue, 12 Dec 2017 08:01:58 GMT  
		Size: 8.6 MB (8636787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c93763e33f35c3974631198e261ac389cb564d90b37f0443650ce34fee2dba2`  
		Last Modified: Tue, 12 Dec 2017 08:01:57 GMT  
		Size: 9.0 MB (8973876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbb22c778e9128dce650ba952241183b7375138fa397187b7967efef8221039`  
		Last Modified: Tue, 12 Dec 2017 08:02:29 GMT  
		Size: 48.6 MB (48567783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7d6f2e29096cc93e652b48e0f9cbe3c28587efeb67afb05a4a3c95bfd53cbd`  
		Last Modified: Tue, 12 Dec 2017 16:21:06 GMT  
		Size: 894.4 KB (894420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834793cb302ca7c856b57ded5f91611a4c74209cd8dd50fad662bf5479f954e0`  
		Last Modified: Tue, 12 Dec 2017 16:21:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35762e32445880df44cfe0452638ad5d1af2ca1b35e54ff612bc8de21a204f4`  
		Last Modified: Tue, 12 Dec 2017 16:21:05 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767ae54d85a98ebc04ac36a2f00fb89d040bb316d7e72258cb5ba95184a42bd8`  
		Last Modified: Tue, 12 Dec 2017 16:22:08 GMT  
		Size: 285.1 MB (285113816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e238308c6de4d74e116e96e048ec6bb6ba8ef6d2e24f3bdd887d8789dd6b79b1`  
		Last Modified: Tue, 12 Dec 2017 19:21:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c386b67bfd0dd2a295fa362d27812d1a68f81bcc2a944f1bd99b57b2ae7fabb0`  
		Last Modified: Tue, 12 Dec 2017 19:21:13 GMT  
		Size: 8.9 MB (8883843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e687b0095a8d1cc310ed37e30881261e25f9c6f928b41709254cb12f5c86181b`  
		Last Modified: Tue, 12 Dec 2017 19:22:57 GMT  
		Size: 750.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4719e791393a309dcb9ca547817ef91844fc8c063711b89124505e916dfd7bca`  
		Last Modified: Tue, 12 Dec 2017 19:22:57 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-9` - linux; arm variant v5

```console
$ docker pull maven@sha256:be840e736e2645eb21ea96a1c1aea3906953ab08b7cde79b6625900caba3c659
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **375.5 MB (375539005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2d888cd8b6036f033e40f8bbbe6921f7a30b78cdd0df8de83479aebcc8ac6f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Dec 2017 20:59:59 GMT
ADD file:af4cd7d5c7a1769f049a442dfd7a1b0fa6359ce5306569a5130c55609ec5175e in / 
# Tue, 12 Dec 2017 20:59:59 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 22:56:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 22:56:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 22:57:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 23:39:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 23:39:09 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 23:39:10 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 23:39:11 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 23:39:11 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Dec 2017 23:39:11 GMT
ENV JAVA_VERSION=9.0.1+11
# Tue, 12 Dec 2017 23:39:12 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Tue, 12 Dec 2017 23:41:42 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Tue, 12 Dec 2017 23:41:51 GMT
CMD ["jshell"]
# Wed, 13 Dec 2017 02:13:33 GMT
ARG MAVEN_VERSION=3.5.2
# Wed, 13 Dec 2017 02:13:34 GMT
ARG USER_HOME_DIR=/root
# Wed, 13 Dec 2017 02:13:34 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Wed, 13 Dec 2017 02:13:35 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Wed, 13 Dec 2017 02:13:37 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN ln -s /etc/java-9-openjdk /usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)/conf
# Wed, 13 Dec 2017 02:13:40 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 13 Dec 2017 02:13:41 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 13 Dec 2017 02:13:41 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 13 Dec 2017 02:14:57 GMT
COPY file:fb726a12bbbf8ff54c8d9fceef4fa3018c11a435bfa04ee5f73156c544907861 in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 13 Dec 2017 02:14:58 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 13 Dec 2017 02:14:58 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 13 Dec 2017 02:14:59 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:acff8687551d235a654afe80e0891cce1bd27c306fff4e41bb6b44b226a473e4`  
		Last Modified: Tue, 12 Dec 2017 21:10:06 GMT  
		Size: 46.9 MB (46876188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12a8cc19c8faf784e145d3a3c486d1b5a0892e4af7a81189d15f0eb18053a58`  
		Last Modified: Tue, 12 Dec 2017 23:08:24 GMT  
		Size: 7.8 MB (7808219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93c884700496b57c386401815cba851f8f8f992a0295e68194990608ff2dea2`  
		Last Modified: Tue, 12 Dec 2017 23:08:23 GMT  
		Size: 8.7 MB (8718966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ee1043aa0902f88a632c6b234c1bb077d60f488629571507684973eb93faa6`  
		Last Modified: Tue, 12 Dec 2017 23:08:50 GMT  
		Size: 46.4 MB (46397899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2099c7b7dd2213f466f51f6b0bfa54387da43193cf9ce36ee3cbdd2109e550`  
		Last Modified: Tue, 12 Dec 2017 23:57:33 GMT  
		Size: 887.6 KB (887635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f617a7acf88155aa54c4680de33c2c8bebf3d8f0c74d454fb551a387fce856d`  
		Last Modified: Tue, 12 Dec 2017 23:57:33 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5b69c29b35770fd4cf754353c079ca508f0985cacb91608e06978340869b4c`  
		Last Modified: Tue, 12 Dec 2017 23:57:33 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab4b92fa27c1e851d400e002fa6f39816f1f964ef6f91cc5dc4f91faad66612`  
		Last Modified: Tue, 12 Dec 2017 23:58:27 GMT  
		Size: 256.0 MB (255964511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215745c08c4d19133d0b31f4638d7c8f59ce1e470fb9ed60f58c027822cdc9a5`  
		Last Modified: Wed, 13 Dec 2017 02:16:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64cac283a53765bc4ce07cc333be4077c126ca507fb61a5c219345d56096fc7`  
		Last Modified: Wed, 13 Dec 2017 02:16:37 GMT  
		Size: 8.9 MB (8883875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6df5d2c7b6890806f4521b0035304bd35b348fe0c278b053f8f6a7a6b49c117`  
		Last Modified: Wed, 13 Dec 2017 02:19:21 GMT  
		Size: 747.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28e90511c509043220fa66255b189a846fff9654ba38c96adb379f5b0fa2193`  
		Last Modified: Wed, 13 Dec 2017 02:19:21 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-9` - linux; arm variant v7

```console
$ docker pull maven@sha256:0b5eac4df0afbcd3697ac0e76060af89835456996e8dddd6be9ff47e9349a973
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.6 MB (372555814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2635a8044c950cddb6a4d68a97f1b43de509dc813fcab7e2b324171bde433317`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Dec 2017 13:30:47 GMT
ADD file:b788e24f4cada715c58008741a4bc6b55912bf54f897e9febf55038c7259474a in / 
# Tue, 12 Dec 2017 13:30:48 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:18:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:18:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 14:18:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:20:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:20:45 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:20:47 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 15:20:48 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 15:20:48 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Dec 2017 15:20:49 GMT
ENV JAVA_VERSION=9.0.1+11
# Tue, 12 Dec 2017 15:20:49 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Tue, 12 Dec 2017 15:22:27 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Tue, 12 Dec 2017 15:22:29 GMT
CMD ["jshell"]
# Tue, 12 Dec 2017 18:33:32 GMT
ARG MAVEN_VERSION=3.5.2
# Tue, 12 Dec 2017 18:33:32 GMT
ARG USER_HOME_DIR=/root
# Tue, 12 Dec 2017 18:33:32 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Tue, 12 Dec 2017 18:33:33 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Tue, 12 Dec 2017 18:33:34 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN ln -s /etc/java-9-openjdk /usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)/conf
# Tue, 12 Dec 2017 18:33:37 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Tue, 12 Dec 2017 18:33:37 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 12 Dec 2017 18:33:38 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 12 Dec 2017 18:35:04 GMT
COPY file:fb726a12bbbf8ff54c8d9fceef4fa3018c11a435bfa04ee5f73156c544907861 in /usr/local/bin/mvn-entrypoint.sh 
# Tue, 12 Dec 2017 18:35:05 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Tue, 12 Dec 2017 18:35:05 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 12 Dec 2017 18:35:06 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:ee9da7ca0ecfb9e496d4e6a11a2de17d38b2676f64081ca6643b85f1026bd24a`  
		Last Modified: Tue, 12 Dec 2017 13:42:33 GMT  
		Size: 44.8 MB (44836300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9035433aec00afaaa737a1213c4367cab1ef3d7a572aa2cb952e73854b963d0`  
		Last Modified: Tue, 12 Dec 2017 14:32:26 GMT  
		Size: 7.5 MB (7534247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d036c584b8f46f4616710df516ffdb5657ef66387fcf24bd3752cdeaf9091427`  
		Last Modified: Tue, 12 Dec 2017 14:32:26 GMT  
		Size: 8.4 MB (8438419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b479b9228413b4b2b667f467e0854f29fee2f1d886dafe3d80c8ff1f88f6cb`  
		Last Modified: Tue, 12 Dec 2017 14:33:01 GMT  
		Size: 44.5 MB (44458911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dadcdc8043e8fffd22e2d161e44baa8c3d5ed465d22bc1f5cb8d3931247c41`  
		Last Modified: Tue, 12 Dec 2017 15:36:36 GMT  
		Size: 870.1 KB (870124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4734d69edf519efe4fbedf536d25fa88468f9b50ffdfac218ac60ada6894f4a9`  
		Last Modified: Tue, 12 Dec 2017 15:36:36 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f645962f883a82f79eec1768f3b5ffff9ae768be34e53cf4bcde87794f169db3`  
		Last Modified: Tue, 12 Dec 2017 15:36:36 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e50d73e0e0281ee08c8a052af07664a4efb14940603581ee862bcd1af7fcd4`  
		Last Modified: Tue, 12 Dec 2017 15:37:27 GMT  
		Size: 257.5 MB (257532250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d396909f1cf0b2ca38623ecb5a385ea53369e8bac474454b31bc5079996ad851`  
		Last Modified: Tue, 12 Dec 2017 18:36:41 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cc2701350ca5fcfe7b1651795da8eeea5914203e01f9a1068b8ea2cab1e11e`  
		Last Modified: Tue, 12 Dec 2017 18:36:43 GMT  
		Size: 8.9 MB (8883861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcee69fbabde82e04cad191c7e7fb8f02ad3db0ca5f1ecb632cd7f15671545cc`  
		Last Modified: Tue, 12 Dec 2017 18:39:23 GMT  
		Size: 746.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b332ae5606c1aa30b39161adcc5ae45ce1ec84d91b4c2ce5d683570be3a4807`  
		Last Modified: Tue, 12 Dec 2017 18:39:24 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-9` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:ce8abc74eed68bff5e9d26f9e869e8be1861701604abeb31e03653ab62d0a81e
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.4 MB (381391963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e9dd1ab5d51cbec7e2015c5b9562b6c61a1bc43b81d1348276de21be5718bed`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Dec 2017 18:28:41 GMT
ADD file:7487b447e9ae95ddff2e8f1bbdc2b089a3a6fb70edf7f218bf3c662727c19ade in / 
# Tue, 12 Dec 2017 18:28:42 GMT
CMD ["bash"]
# Fri, 15 Dec 2017 16:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 Dec 2017 16:03:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 Dec 2017 16:04:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 Dec 2017 21:05:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 Dec 2017 21:05:47 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2017 21:05:50 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 15 Dec 2017 21:05:53 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 15 Dec 2017 21:05:54 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 15 Dec 2017 21:05:55 GMT
ENV JAVA_VERSION=9.0.1+11
# Fri, 15 Dec 2017 21:05:56 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Fri, 15 Dec 2017 21:13:11 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Fri, 15 Dec 2017 21:13:14 GMT
CMD ["jshell"]
# Sat, 16 Dec 2017 08:53:40 GMT
ARG MAVEN_VERSION=3.5.2
# Sat, 16 Dec 2017 08:53:41 GMT
ARG USER_HOME_DIR=/root
# Sat, 16 Dec 2017 08:53:42 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Sat, 16 Dec 2017 08:53:42 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Sat, 16 Dec 2017 08:53:45 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN ln -s /etc/java-9-openjdk /usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)/conf
# Sat, 16 Dec 2017 08:53:50 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 16 Dec 2017 08:53:50 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 16 Dec 2017 08:53:51 GMT
ENV MAVEN_CONFIG=/root/.m2
# Sat, 16 Dec 2017 08:54:49 GMT
COPY file:fb726a12bbbf8ff54c8d9fceef4fa3018c11a435bfa04ee5f73156c544907861 in /usr/local/bin/mvn-entrypoint.sh 
# Sat, 16 Dec 2017 08:54:50 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Sat, 16 Dec 2017 08:54:51 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Sat, 16 Dec 2017 08:54:52 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:aa10cf671b46f67e3e12579e72f085c7b8402ff25ccafb8616eb9e1cbe71bf85`  
		Last Modified: Tue, 12 Dec 2017 18:44:03 GMT  
		Size: 46.2 MB (46188985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cce7e08176846c9ad6c15ff845d12c630e1d4ab1a0f8ef1e7a0786ec45ad2b`  
		Last Modified: Fri, 15 Dec 2017 17:17:29 GMT  
		Size: 7.9 MB (7856875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a14a037f71e9308ee97c32436f3203d1f06a675930a80dba9a16c2f5c78166`  
		Last Modified: Fri, 15 Dec 2017 17:17:29 GMT  
		Size: 8.7 MB (8712398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc237cede08f1aa41bf239b023687354ee22244dafaac2d899ca82852f5a4e6`  
		Last Modified: Fri, 15 Dec 2017 17:17:54 GMT  
		Size: 46.8 MB (46825072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf59a433671cc9e6cb0740414a980b5866f853840f657a6fe8e0023410f3da07`  
		Last Modified: Fri, 15 Dec 2017 21:23:51 GMT  
		Size: 879.7 KB (879675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2929b11fd08b394168f3e2c92a004b93a1b5e2c671f773aa3a65f007de0e92c7`  
		Last Modified: Fri, 15 Dec 2017 21:23:50 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b743b029cc4db8cfe412e877421656a601ce9ef0a9cee63ccb20ddfed7481839`  
		Last Modified: Fri, 15 Dec 2017 21:23:50 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f314e6c5c8fcb9f7a2ff781341b1b4304cfa7ecbddc19320ea75825ad37a6e95`  
		Last Modified: Fri, 15 Dec 2017 21:24:57 GMT  
		Size: 262.0 MB (262043388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d4cf2ee530af6c62e0942bb9ee4bec1931cee90c75590eb7720f32327244df`  
		Last Modified: Sat, 16 Dec 2017 08:55:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42264b512e8376f502bd8de1164034297d52f61d7ab8a8a750491c21d3b82691`  
		Last Modified: Sat, 16 Dec 2017 08:55:30 GMT  
		Size: 8.9 MB (8883856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04400f4a1fca0815a6e9170d4e5f364a47dfe291bdb7179e8690f8e1f15072e`  
		Last Modified: Sat, 16 Dec 2017 08:56:10 GMT  
		Size: 747.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c81a998aead1280f09d331a51549c05958a1c4d0ddc1078fb3291bb7dd3c12`  
		Last Modified: Sat, 16 Dec 2017 08:56:10 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-9` - linux; 386

```console
$ docker pull maven@sha256:73726357560e37a2990b61f320823d7c0f77a3293690ffe5244cbf88bb03591a
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **419.0 MB (419031105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74e7a07ef1879cb4bc0e3bd852ad7e3e301c6506b2ed8b7b0bcc79da5a1cea20`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Dec 2017 14:24:56 GMT
ADD file:7e72f60be83facf3a36831facc1a26f572f3ae83fc49b2bc4c8de0b6e3321e84 in / 
# Tue, 12 Dec 2017 14:24:56 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 17:02:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 17:02:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 17:03:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 18:53:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 18:53:54 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 18:53:54 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 18:53:55 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 18:53:55 GMT
ENV JAVA_HOME=/docker-java-home
# Tue, 12 Dec 2017 18:53:56 GMT
ENV JAVA_VERSION=9.0.1+11
# Tue, 12 Dec 2017 18:53:56 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Tue, 12 Dec 2017 18:56:23 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Tue, 12 Dec 2017 19:01:52 GMT
CMD ["jshell"]
# Wed, 13 Dec 2017 20:59:52 GMT
ARG MAVEN_VERSION=3.5.2
# Wed, 13 Dec 2017 20:59:52 GMT
ARG USER_HOME_DIR=/root
# Wed, 13 Dec 2017 20:59:53 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Wed, 13 Dec 2017 20:59:53 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Wed, 13 Dec 2017 20:59:54 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN ln -s /etc/java-9-openjdk /usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)/conf
# Wed, 13 Dec 2017 20:59:58 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Wed, 13 Dec 2017 21:00:07 GMT
ENV MAVEN_HOME=/usr/share/maven
# Wed, 13 Dec 2017 21:00:07 GMT
ENV MAVEN_CONFIG=/root/.m2
# Wed, 13 Dec 2017 21:08:30 GMT
COPY file:fb726a12bbbf8ff54c8d9fceef4fa3018c11a435bfa04ee5f73156c544907861 in /usr/local/bin/mvn-entrypoint.sh 
# Wed, 13 Dec 2017 21:08:30 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Wed, 13 Dec 2017 21:08:31 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Wed, 13 Dec 2017 21:08:31 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:c3cf1d3d69aef55e4aef2c1f0a9455d1dfbbb7ae17d15a0d963e8c55e6e61af4`  
		Last Modified: Tue, 12 Dec 2017 14:58:13 GMT  
		Size: 49.3 MB (49250980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e767ba54897a1df6013ec3b06fd1546d3123979a02ac1f8f8eb0f079fd928126`  
		Last Modified: Tue, 12 Dec 2017 17:33:48 GMT  
		Size: 8.6 MB (8608693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936341216c1a183dced55abc7be29ddca5b53a3fe1a3d85f00538784bd1a090d`  
		Last Modified: Tue, 12 Dec 2017 17:33:48 GMT  
		Size: 9.3 MB (9251281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf1165f2ef33ed9e795182bb0912cf7dd9ac26b5bd6e12fb53b9c469c2f832b`  
		Last Modified: Tue, 12 Dec 2017 17:34:24 GMT  
		Size: 50.2 MB (50228972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3238289ff178b02f347c62e82e28c2045f3d60083b8cf34c8319df235149cb49`  
		Last Modified: Tue, 12 Dec 2017 19:41:48 GMT  
		Size: 902.4 KB (902445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5da487583a16f34d9a3443d5a4774b3095efcbc454349d539b2d419d104ba15`  
		Last Modified: Tue, 12 Dec 2017 19:41:47 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a66969633f8bf1dd82a5e7401fbf03204700471a82be4aef72d8d99cff738b9`  
		Last Modified: Tue, 12 Dec 2017 19:41:47 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbe34cfad356be1815a0d386b40dd8a143521521f0fb97793e461176511a1b1`  
		Last Modified: Tue, 12 Dec 2017 19:43:27 GMT  
		Size: 291.9 MB (291903171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4baaf5fe7e6f346d7a17b0a8173a89bd0a30492f6465bc744f07a11b8f7ac1bb`  
		Last Modified: Wed, 13 Dec 2017 21:19:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4eb183fccf98783581cdcfa98fde265278091b3995405186d35a26de66572b4`  
		Last Modified: Wed, 13 Dec 2017 21:19:47 GMT  
		Size: 8.9 MB (8883844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b79a5820ddf11896e160ab34ffb43559de1983dff5413c7cd2d54bf8f621de8`  
		Last Modified: Wed, 13 Dec 2017 21:47:50 GMT  
		Size: 751.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7c0d944bf1e9886526b4aad7b9ad3ce0e53b985f303faeebf989383a7d8585`  
		Last Modified: Wed, 13 Dec 2017 21:47:50 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-9` - linux; ppc64le

```console
$ docker pull maven@sha256:27da86cfce59300c4aa79ee62cca41a4df436149493bde4d5e9a08130907622c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.8 MB (396836239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:610da4c2226dcb000b8cee328067de5cac05019b520e31e6701d4765981eb57a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 12 Dec 2017 01:34:15 GMT
ADD file:7904a0f79cc86767c6e3ac367f0df06aa262c6639e79e39652eac766c3faf4b6 in / 
# Tue, 12 Dec 2017 01:34:16 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 03:12:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 03:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 03:16:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 Dec 2017 06:28:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 Dec 2017 06:28:08 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2017 06:28:12 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Fri, 15 Dec 2017 06:28:15 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Fri, 15 Dec 2017 06:28:17 GMT
ENV JAVA_HOME=/docker-java-home
# Fri, 15 Dec 2017 06:28:18 GMT
ENV JAVA_VERSION=9.0.1+11
# Fri, 15 Dec 2017 06:28:20 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Fri, 15 Dec 2017 06:35:19 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Fri, 15 Dec 2017 06:35:25 GMT
CMD ["jshell"]
# Fri, 15 Dec 2017 07:13:29 GMT
ARG MAVEN_VERSION=3.5.2
# Fri, 15 Dec 2017 07:13:31 GMT
ARG USER_HOME_DIR=/root
# Fri, 15 Dec 2017 07:13:33 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Fri, 15 Dec 2017 07:13:34 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Fri, 15 Dec 2017 07:13:39 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN ln -s /etc/java-9-openjdk /usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)/conf
# Fri, 15 Dec 2017 07:13:45 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 15 Dec 2017 07:13:46 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 15 Dec 2017 07:13:47 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 15 Dec 2017 07:14:19 GMT
COPY file:fb726a12bbbf8ff54c8d9fceef4fa3018c11a435bfa04ee5f73156c544907861 in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 15 Dec 2017 07:14:20 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Fri, 15 Dec 2017 07:14:22 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 15 Dec 2017 07:14:23 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:21b73404fd38d2445a6ecbcf148b2dd5047623273b33ea9546ddf6796601ec9b`  
		Last Modified: Tue, 12 Dec 2017 01:40:28 GMT  
		Size: 49.7 MB (49652013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3d5e1672290a07cf756dbcee37e26f4e406df9a113e8e2dc11abbc2b31d867`  
		Last Modified: Tue, 12 Dec 2017 03:54:16 GMT  
		Size: 8.2 MB (8207114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7d8032257e5508a59f355bd1eb60e35584078939f47f0f54ca3e647ed03f71`  
		Last Modified: Tue, 12 Dec 2017 03:54:18 GMT  
		Size: 9.2 MB (9192961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf62220ef17b233f919a5cd42f1c6eb64f590665103726af12d898db12754fc2`  
		Last Modified: Tue, 12 Dec 2017 03:54:33 GMT  
		Size: 51.2 MB (51189959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00eec43fc367b4384fdfaa02ad922fa1023ef70d53771f7a360bcf4d37902375`  
		Last Modified: Fri, 15 Dec 2017 06:47:51 GMT  
		Size: 889.6 KB (889573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a580d903a55481d49889e7f96442ee8d7b88ba8fed5a1ce82940423f7e50b146`  
		Last Modified: Fri, 15 Dec 2017 06:47:50 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db62cabaa771ae496b4cbf394db65e14ea45a8eb02851b6050c01620c311a408`  
		Last Modified: Fri, 15 Dec 2017 06:47:50 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421e4940dad323173677b9cd282e4589750e7fa0e1fe1cb1aad95b0418e790b5`  
		Last Modified: Fri, 15 Dec 2017 06:48:53 GMT  
		Size: 268.8 MB (268819028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d6a52dae4073d32e54406b78c98585ce2e001403f1b75b32383a6f81325acc`  
		Last Modified: Fri, 15 Dec 2017 07:15:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbefa9defd52052e0e9503bb4eca50fa66d466603d878a31ef07f887e520ffe`  
		Last Modified: Fri, 15 Dec 2017 07:15:14 GMT  
		Size: 8.9 MB (8883877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd15931733c3cd075aec3eed963614c5acb1ea7cc211bcc86bad88455b7abdf7`  
		Last Modified: Fri, 15 Dec 2017 07:15:45 GMT  
		Size: 747.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c620e11254a8f94e778f2426897b5fca50b16cfc40dfb63d11d4a743e3ddd3`  
		Last Modified: Fri, 15 Dec 2017 07:15:45 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-jdk-9` - linux; s390x

```console
$ docker pull maven@sha256:a321b691921ce7a453f0d4316ecd596bfad9af6db6670d13384ec78e37317f20
```

-	Docker Version: 17.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.1 MB (371108986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce19719576594795247f6753b10a1b8ad9f9b04e7dd58c06c1b78a3f122027e1`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 09 Oct 2017 21:43:27 GMT
ADD file:51898e1a12f3bbc77c696e9156d7bb51579dc530148ca78c00142c511a349de6 in / 
# Mon, 09 Oct 2017 21:43:27 GMT
CMD ["bash"]
# Mon, 09 Oct 2017 22:13:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 16:42:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Nov 2017 16:43:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 22:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Nov 2017 22:47:56 GMT
ENV LANG=C.UTF-8
# Thu, 02 Nov 2017 22:47:56 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Thu, 02 Nov 2017 22:47:57 GMT
RUN ln -svT "/usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Thu, 02 Nov 2017 22:47:57 GMT
ENV JAVA_HOME=/docker-java-home
# Sat, 04 Nov 2017 16:58:27 GMT
ENV JAVA_VERSION=9.0.1+11
# Sat, 04 Nov 2017 16:58:27 GMT
ENV JAVA_DEBIAN_VERSION=9.0.1+11-1
# Sat, 04 Nov 2017 16:59:46 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-9-jdk="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
# Sat, 04 Nov 2017 16:59:47 GMT
CMD ["jshell"]
# Sat, 04 Nov 2017 17:30:03 GMT
ARG MAVEN_VERSION=3.5.2
# Sat, 04 Nov 2017 17:30:03 GMT
ARG USER_HOME_DIR=/root
# Sat, 04 Nov 2017 17:30:03 GMT
ARG SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff
# Sat, 04 Nov 2017 17:30:03 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries
# Sat, 04 Nov 2017 17:30:04 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN ln -s /etc/java-9-openjdk /usr/lib/jvm/java-9-openjdk-$(dpkg --print-architecture)/conf
# Sat, 04 Nov 2017 17:30:07 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.5.2/binaries MAVEN_VERSION=3.5.2 SHA=707b1f6e390a65bde4af4cdaf2a24d45fc19a6ded00fff02e91626e3e42ceaff USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha256sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Sat, 04 Nov 2017 17:30:07 GMT
ENV MAVEN_HOME=/usr/share/maven
# Sat, 04 Nov 2017 17:30:08 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 07 Dec 2017 04:09:10 GMT
COPY file:fb726a12bbbf8ff54c8d9fceef4fa3018c11a435bfa04ee5f73156c544907861 in /usr/local/bin/mvn-entrypoint.sh 
# Thu, 07 Dec 2017 04:09:10 GMT
COPY file:b3fc14e8337e0079a4e97eace880b4b7cddc0dc0ea733de80749f78fe1eb089a in /usr/share/maven/ref/ 
# Thu, 07 Dec 2017 04:09:11 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 07 Dec 2017 04:09:11 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:387500139c6151d781fe62dbc679af96a9ac79dc2049d4b57d00beb6515f3617`  
		Last Modified: Mon, 09 Oct 2017 21:47:41 GMT  
		Size: 47.3 MB (47292875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2bf7517ce1b767b32d484c45cdbde2774795f97aa23cbd2ca4f9aa57e0907e`  
		Last Modified: Mon, 09 Oct 2017 22:20:45 GMT  
		Size: 8.1 MB (8093416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf6e9bec5e8ebc238611abf06601adf9ff50529f0f19c63cbfaa10a33c32121`  
		Last Modified: Thu, 02 Nov 2017 16:55:12 GMT  
		Size: 9.5 MB (9478048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc27c91df378d34d3fe35fa5f2a0c2b27d326e071ec06354215b99bd258e2e4`  
		Last Modified: Thu, 02 Nov 2017 16:55:31 GMT  
		Size: 50.3 MB (50321473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad1d85bd50f537c631a09410463102dbf36792961b6ec7e3e59ad565eeba3c2`  
		Last Modified: Sat, 04 Nov 2017 17:05:07 GMT  
		Size: 904.6 KB (904634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe1ce9d339a420ab9d9ede1d8f2b127672ff8bfdc8a6ad88cdd7742619b4338`  
		Last Modified: Sat, 04 Nov 2017 17:05:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c98cb25aeb88a941e25c4ceb73fd096e142236cb799773aef05ade533e09ec9`  
		Last Modified: Sat, 04 Nov 2017 17:05:07 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2071655c756fa4fec702e922a6b93ede29a33ce3a2067f54ee2c635639b319`  
		Last Modified: Sat, 04 Nov 2017 17:05:35 GMT  
		Size: 246.1 MB (246132996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb21701084750e2c7bb4a500aaae11f450556f70946f2c9e5e6be26d15476cb`  
		Last Modified: Sat, 04 Nov 2017 17:31:56 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a34a6e5536895a426fcb667760b9214bca4df6d05a96e958d127080d820dee`  
		Last Modified: Sat, 04 Nov 2017 17:31:58 GMT  
		Size: 8.9 MB (8883832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af13cf83b83081e3a80e3540de6f5d091712bf476a8214ceefdff429c33aee`  
		Last Modified: Thu, 07 Dec 2017 04:11:43 GMT  
		Size: 747.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c671f8fd26c1047e48049af54566d1e284b99d85ceac4aaad25c0a2dd18559`  
		Last Modified: Thu, 07 Dec 2017 04:11:43 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
