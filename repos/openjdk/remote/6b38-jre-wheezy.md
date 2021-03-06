## `openjdk:6b38-jre-wheezy`

```console
$ docker pull openjdk@sha256:69d1634c2d261b0db529a7ee91ac0fc93d960e4cb53e83e2665be8c3431691d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7

### `openjdk:6b38-jre-wheezy` - linux; amd64

```console
$ docker pull openjdk@sha256:e69f6540ab037faf368f86f06d1ece7261666895746f911557fa8bbbd31398f8
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139776305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc9069b6805935fa05c1bc1170778fc155cd9450d8639a59da54e38e911593b6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 01:46:04 GMT
ADD file:281b987b09ac9b71793de5201331461636a08ec23af27a9e11a14484018993dd in / 
# Tue, 12 Dec 2017 01:46:04 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 07:56:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 07:56:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 15:01:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:01:46 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:01:47 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 15:01:47 GMT
RUN ln -svT "/usr/lib/jvm/java-6-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 15:01:48 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Tue, 12 Dec 2017 15:01:48 GMT
ENV JAVA_VERSION=6b38
# Tue, 12 Dec 2017 15:01:48 GMT
ENV JAVA_DEBIAN_VERSION=6b38-1.13.10-1~deb7u1
# Tue, 12 Dec 2017 15:02:36 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-6-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:762ae076e9a326e4eac3b3db9e3afe4b6dc930ec52dbb2aa27a300d1323a52b6`  
		Last Modified: Tue, 12 Dec 2017 01:59:44 GMT  
		Size: 38.1 MB (38109825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23de19d3f13a2be7ebc7920f3ba4c5b85177a11b50a1ade92d360c09aa349bf1`  
		Last Modified: Tue, 12 Dec 2017 08:06:02 GMT  
		Size: 7.0 MB (6950248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb6f7cbbff330da5be9ecbc972f6fc7cadec02022be4cca397fc000f60d469`  
		Last Modified: Tue, 12 Dec 2017 15:45:53 GMT  
		Size: 548.7 KB (548727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a068071674de62beaa2da19128e497fc2e22b754a4a343ac9e286bcb94c02e3`  
		Last Modified: Tue, 12 Dec 2017 15:45:53 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9eee10f8e2e50d042ab6a5290cf314d494dd98898f784f39847dd8505176873`  
		Last Modified: Tue, 12 Dec 2017 15:45:53 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53360b376d7ff6ee4f30dcca65c633060527a63de1dc033c4f3550a7fc388b7`  
		Last Modified: Tue, 12 Dec 2017 15:46:17 GMT  
		Size: 94.2 MB (94167128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:6b38-jre-wheezy` - linux; arm variant v7

```console
$ docker pull openjdk@sha256:8eba7df5fd24adfbd9aa53756968627ff630a4384b5daae1d115442a038ca29d
```

-	Docker Version: 17.06.0-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124388063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f81a7f63ab4f8c7755de0351100f15f7d4b8ff0c509aa13374e112e473c70a9d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Dec 2017 13:36:11 GMT
ADD file:9db26feeeebe82707411c8b6a09f22ba8e33fdd8bdf1e1cb3fd179cfc09b850e in / 
# Tue, 12 Dec 2017 13:36:12 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 14:25:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 14:25:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Dec 2017 15:04:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzip2 		unzip 		xz-utils 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2017 15:04:52 GMT
ENV LANG=C.UTF-8
# Tue, 12 Dec 2017 15:04:54 GMT
RUN { 		echo '#!/bin/sh'; 		echo 'set -e'; 		echo; 		echo 'dirname "$(dirname "$(readlink -f "$(which javac || which java)")")"'; 	} > /usr/local/bin/docker-java-home 	&& chmod +x /usr/local/bin/docker-java-home
# Tue, 12 Dec 2017 15:04:55 GMT
RUN ln -svT "/usr/lib/jvm/java-6-openjdk-$(dpkg --print-architecture)" /docker-java-home
# Tue, 12 Dec 2017 15:04:55 GMT
ENV JAVA_HOME=/docker-java-home/jre
# Tue, 12 Dec 2017 15:04:56 GMT
ENV JAVA_VERSION=6b38
# Tue, 12 Dec 2017 15:04:56 GMT
ENV JAVA_DEBIAN_VERSION=6b38-1.13.10-1~deb7u1
# Tue, 12 Dec 2017 15:05:28 GMT
RUN set -ex; 		if [ ! -d /usr/share/man/man1 ]; then 		mkdir -p /usr/share/man/man1; 	fi; 		apt-get update; 	apt-get install -y 		openjdk-6-jre="$JAVA_DEBIAN_VERSION" 	; 	rm -rf /var/lib/apt/lists/*; 		[ "$(readlink -f "$JAVA_HOME")" = "$(docker-java-home)" ]; 		update-alternatives --get-selections | awk -v home="$(readlink -f "$JAVA_HOME")" 'index($3, home) == 1 { $2 = "manual"; print | "update-alternatives --set-selections" }'; 	update-alternatives --query java | grep -q 'Status: manual'
```

-	Layers:
	-	`sha256:dd70000a68c40049fa024e9ebecc22bcd8a32b0fb098e9f3edafdbfc872054b4`  
		Last Modified: Tue, 12 Dec 2017 13:47:59 GMT  
		Size: 35.7 MB (35661805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ae93d1aa9ba1e13bd1449ae6d27b5849b9a9acbf7f273c7059aa1c7a7f700e`  
		Last Modified: Tue, 12 Dec 2017 14:37:06 GMT  
		Size: 6.4 MB (6369943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2684ab20a2a3c6524f48748b9c85aad895ffebf49c489cbd6bf5e15a8f1acb`  
		Last Modified: Tue, 12 Dec 2017 15:28:20 GMT  
		Size: 537.7 KB (537699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b57491d9e899b46ea0e09e5a12576af86d1fea52dc4c0edd5f6e5863690fdd3`  
		Last Modified: Tue, 12 Dec 2017 15:28:20 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c09dfd4f0b24ae955e75a9175a62feb5d42ef65c1c27322508c395563b5dfb4`  
		Last Modified: Tue, 12 Dec 2017 15:28:20 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0a04a19dec16de420ce3e37e8c96bfb658d2ba47931b36f69b431b634e0546`  
		Last Modified: Tue, 12 Dec 2017 15:28:37 GMT  
		Size: 81.8 MB (81818239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
