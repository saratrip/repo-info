<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo`

-	[`mongo:3`](#mongo3)
-	[`mongo:3.0`](#mongo30)
-	[`mongo:3.0.15`](#mongo3015)
-	[`mongo:3.0.15-wheezy`](#mongo3015-wheezy)
-	[`mongo:3.0.15-windowsservercore`](#mongo3015-windowsservercore)
-	[`mongo:3.0.15-windowsservercore-1709`](#mongo3015-windowsservercore-1709)
-	[`mongo:3.0.15-windowsservercore-ltsc2016`](#mongo3015-windowsservercore-ltsc2016)
-	[`mongo:3.0-wheezy`](#mongo30-wheezy)
-	[`mongo:3.0-windowsservercore`](#mongo30-windowsservercore)
-	[`mongo:3.0-windowsservercore-1709`](#mongo30-windowsservercore-1709)
-	[`mongo:3.0-windowsservercore-ltsc2016`](#mongo30-windowsservercore-ltsc2016)
-	[`mongo:3.2`](#mongo32)
-	[`mongo:3.2.18`](#mongo3218)
-	[`mongo:3.2.18-jessie`](#mongo3218-jessie)
-	[`mongo:3.2.18-windowsservercore`](#mongo3218-windowsservercore)
-	[`mongo:3.2.18-windowsservercore-1709`](#mongo3218-windowsservercore-1709)
-	[`mongo:3.2.18-windowsservercore-ltsc2016`](#mongo3218-windowsservercore-ltsc2016)
-	[`mongo:3.2-jessie`](#mongo32-jessie)
-	[`mongo:3.2-windowsservercore`](#mongo32-windowsservercore)
-	[`mongo:3.2-windowsservercore-1709`](#mongo32-windowsservercore-1709)
-	[`mongo:3.2-windowsservercore-ltsc2016`](#mongo32-windowsservercore-ltsc2016)
-	[`mongo:3.4`](#mongo34)
-	[`mongo:3.4.10`](#mongo3410)
-	[`mongo:3.4.10-jessie`](#mongo3410-jessie)
-	[`mongo:3.4.10-windowsservercore`](#mongo3410-windowsservercore)
-	[`mongo:3.4.10-windowsservercore-1709`](#mongo3410-windowsservercore-1709)
-	[`mongo:3.4.10-windowsservercore-ltsc2016`](#mongo3410-windowsservercore-ltsc2016)
-	[`mongo:3.4-jessie`](#mongo34-jessie)
-	[`mongo:3.4-windowsservercore`](#mongo34-windowsservercore)
-	[`mongo:3.4-windowsservercore-1709`](#mongo34-windowsservercore-1709)
-	[`mongo:3.4-windowsservercore-ltsc2016`](#mongo34-windowsservercore-ltsc2016)
-	[`mongo:3.6`](#mongo36)
-	[`mongo:3.6.1`](#mongo361)
-	[`mongo:3.6.1-jessie`](#mongo361-jessie)
-	[`mongo:3.6.1-windowsservercore`](#mongo361-windowsservercore)
-	[`mongo:3.6.1-windowsservercore-1709`](#mongo361-windowsservercore-1709)
-	[`mongo:3.6.1-windowsservercore-ltsc2016`](#mongo361-windowsservercore-ltsc2016)
-	[`mongo:3.6-jessie`](#mongo36-jessie)
-	[`mongo:3.6-windowsservercore`](#mongo36-windowsservercore)
-	[`mongo:3.6-windowsservercore-1709`](#mongo36-windowsservercore-1709)
-	[`mongo:3.6-windowsservercore-ltsc2016`](#mongo36-windowsservercore-ltsc2016)
-	[`mongo:3-jessie`](#mongo3-jessie)
-	[`mongo:3-windowsservercore`](#mongo3-windowsservercore)
-	[`mongo:3-windowsservercore-1709`](#mongo3-windowsservercore-1709)
-	[`mongo:3-windowsservercore-ltsc2016`](#mongo3-windowsservercore-ltsc2016)
-	[`mongo:jessie`](#mongojessie)
-	[`mongo:latest`](#mongolatest)
-	[`mongo:windowsservercore`](#mongowindowsservercore)
-	[`mongo:windowsservercore-1709`](#mongowindowsservercore-1709)
-	[`mongo:windowsservercore-ltsc2016`](#mongowindowsservercore-ltsc2016)

## `mongo:3`

```console
$ docker pull mongo@sha256:c78f6debfb5b10fe2ed390105a729123f3365a33e5aada6f5539922d1d7c75dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:56210d12db53301f71b6f3d38c200c54d9e4722d4884605f6bb24876613efb2f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130387820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1200574c8af96f9b81952bb1131c4a3853fc5c789d73bc50d623d0c6915d1172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Thu, 28 Dec 2017 00:15:43 GMT
ENV MONGO_VERSION=3.6.1
# Thu, 28 Dec 2017 00:15:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 28 Dec 2017 00:16:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 28 Dec 2017 00:16:04 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 28 Dec 2017 00:16:04 GMT
VOLUME [/data/db /data/configdb]
# Thu, 28 Dec 2017 00:16:04 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Thu, 28 Dec 2017 00:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Dec 2017 00:16:05 GMT
EXPOSE 27017/tcp
# Thu, 28 Dec 2017 00:16:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6b165aa31730e9c9ebfe57bc966413905188436bb0c41eecfdef96a09f8c99`  
		Last Modified: Thu, 28 Dec 2017 00:22:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772467f0b4cd666887cd2c67701ce0c258d248a476e05f7d17f29fa678aeae3e`  
		Last Modified: Thu, 28 Dec 2017 00:22:54 GMT  
		Size: 97.1 MB (97051101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d919fbb860064f1964560410ef4dc361653cd42e224e696821cedaba52859`  
		Last Modified: Thu, 28 Dec 2017 00:22:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cad17917cd13144fca5224b3e31f5f26ff3f1b1b6269a1c580653e9db9608b`  
		Last Modified: Thu, 28 Dec 2017 00:22:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0`

```console
$ docker pull mongo@sha256:9887b48e71c146fd3d177f4e08dde584e2a8c2d823d49747f4d2ce03753f3c63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.0` - linux; amd64

```console
$ docker pull mongo@sha256:77f22f913d8e62559b58437df321f02aabd6beeb863b5292c66c175716846f60
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84530333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28cba33aad0327cf5df59ca2cbea98487692775937b9b05d0a7d7780952ba11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:46:27 GMT
ADD file:664e20ea0b4805f811ed279f86823b281c39df127d0f73ae147468bc1a9e4020 in / 
# Tue, 12 Dec 2017 01:46:27 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:35:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:35:31 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 12 Dec 2017 02:35:43 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 		procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:15:47 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:15:47 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:16:02 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:16:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:16:05 GMT
ENV GPG_KEYS=492EAFE8CD016A07919F1D2B9ECBEC467F0CEB10
# Thu, 21 Dec 2017 01:16:06 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_MAJOR=3.0
# Thu, 21 Dec 2017 01:16:08 GMT
ENV MONGO_VERSION=3.0.15
# Thu, 21 Dec 2017 01:16:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian wheezy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:16:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:16:24 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:16:24 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:16:26 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:16:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b967c325a8b3055106908c059240f7ea99c3b22958080fa3a0c1688e1e6739d1`  
		Last Modified: Tue, 12 Dec 2017 02:00:41 GMT  
		Size: 19.2 MB (19164678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4b68f5594ff127e3c87e19190ca62d695d260de2c4e1dfbc1a110dab8e2de`  
		Last Modified: Tue, 12 Dec 2017 02:41:17 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24baba5a242ee93e67a0fcfe657c4944872fd9fd2a064328454997b46cdbd62`  
		Last Modified: Tue, 12 Dec 2017 02:41:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11f2476fef6def7b28fd2c24f84397a099411ed68ad67cf937d5f9b76a82d7`  
		Last Modified: Tue, 12 Dec 2017 02:41:15 GMT  
		Size: 2.7 MB (2660614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b2bf33f8e8bc113a559558c7e0fdc1f4e695b2bec89c09ccafc7f1dff9019`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 810.6 KB (810648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c0d1d2005390ed504d8dd433b7ce7c2f81d79abbc40e191d8e64e1d2b1729`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2fb164e25f84f88ebd54215876bc44293ae6dfd02646f473f87ea57cbbf853`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95455f9a86a6bacac05bdcca3ec35f202e59b2ace6dc2e5c14f3c1e1b154aab4`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460daad09d9d797d449205a3892eb7727250f88cb0fd838eb3da4477673c1bfd`  
		Last Modified: Thu, 21 Dec 2017 01:22:13 GMT  
		Size: 61.9 MB (61886207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab0d8c194a10785d610e3bc5a44fc56aebdc1b74d9475c1aed4690a23569518`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da624b820d4a1a38ffb4556bdd657dcea49c09fdfd356aa66b45a1d995b27`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9ad8e0e7784c98341e142dbd3bf28f8677fbbb98b85dbc7403a25779eb619`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.0` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:4b4cdf9d23dd03fb0de392555aca000ee07a04d2cd7524f23b1bc79600e2134b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5408818021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6731b906bb2bf8eb5d59f8f80e25cb6f1abb3457572f7730c9eae1945cd570e8`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:43:55 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:53:31 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:53:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fef99bf2799b9541f9c402c94b34d6956ad6af6bb8a3e27a8a01db14bb220`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31065debc73bc484363430f1d51f52e688c30017485223a31166a0a0303b8915`  
		Last Modified: Tue, 19 Dec 2017 04:07:10 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fd9f30823161ca0b37849fc3be9a0335985bb921f3c0cb803ca7b6032bdc5e`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb160f9367fa1c9e5e7f19405387c9a223f12e7b58e30933ef46c3d59358405a`  
		Last Modified: Tue, 19 Dec 2017 04:07:27 GMT  
		Size: 47.0 MB (46994564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add3786e86de14542bc7e6b0e40fd8437b9f9b6faab47fb1b3a498072f5cb79d`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12929d9801c71c998eb532a0cccfe18b3ec08feaa0f8b703442b72ab3c41185`  
		Last Modified: Tue, 19 Dec 2017 04:07:09 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a4787ad0ff4679d9818664e5258f86c202196a98c0a8c962163d03e78b685f`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.0` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:00389d2bd6ffd221dfd368ac17ecfc5e260eceb2047ee6863a71fbdc5bd75191
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2910420228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdbab21328ecf02ab2f68ac4290edca6369ec007e8168c943cb98ceebd36437`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:53:47 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:53:48 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:53:49 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:55:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:55:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:56:01 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:56:02 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a4f70e8a55dd9ea85316b97f10c7d87d64d891d4a3893db509966ddf56ca77`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3ea3f4e8d1ec0b6a063c611c64ffb2378d0ea00164896c00a217f03d1d5d8`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b39b3d13ed5c75186b92c5228062beafa6c75dc85824bf6ce76b7fdfefdeb0`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d712635eedd07152360df86c29be50fe9b990b6e6542bc774957a913a31c050`  
		Last Modified: Tue, 19 Dec 2017 04:07:52 GMT  
		Size: 46.6 MB (46586800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d2b16e18ce034f792da7086da5c088f939d755a4cdb266e8daae630494f63`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15104271b3f326fbb100b4c990b242c7c5e2da4f1dc143fb1d7a517df9edd65`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce9f53f93a4baac40828dea63b2616bab3b23f5d5c007506f00400fa4c2510`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0.15`

```console
$ docker pull mongo@sha256:9887b48e71c146fd3d177f4e08dde584e2a8c2d823d49747f4d2ce03753f3c63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.0.15` - linux; amd64

```console
$ docker pull mongo@sha256:77f22f913d8e62559b58437df321f02aabd6beeb863b5292c66c175716846f60
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84530333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28cba33aad0327cf5df59ca2cbea98487692775937b9b05d0a7d7780952ba11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:46:27 GMT
ADD file:664e20ea0b4805f811ed279f86823b281c39df127d0f73ae147468bc1a9e4020 in / 
# Tue, 12 Dec 2017 01:46:27 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:35:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:35:31 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 12 Dec 2017 02:35:43 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 		procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:15:47 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:15:47 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:16:02 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:16:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:16:05 GMT
ENV GPG_KEYS=492EAFE8CD016A07919F1D2B9ECBEC467F0CEB10
# Thu, 21 Dec 2017 01:16:06 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_MAJOR=3.0
# Thu, 21 Dec 2017 01:16:08 GMT
ENV MONGO_VERSION=3.0.15
# Thu, 21 Dec 2017 01:16:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian wheezy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:16:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:16:24 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:16:24 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:16:26 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:16:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b967c325a8b3055106908c059240f7ea99c3b22958080fa3a0c1688e1e6739d1`  
		Last Modified: Tue, 12 Dec 2017 02:00:41 GMT  
		Size: 19.2 MB (19164678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4b68f5594ff127e3c87e19190ca62d695d260de2c4e1dfbc1a110dab8e2de`  
		Last Modified: Tue, 12 Dec 2017 02:41:17 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24baba5a242ee93e67a0fcfe657c4944872fd9fd2a064328454997b46cdbd62`  
		Last Modified: Tue, 12 Dec 2017 02:41:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11f2476fef6def7b28fd2c24f84397a099411ed68ad67cf937d5f9b76a82d7`  
		Last Modified: Tue, 12 Dec 2017 02:41:15 GMT  
		Size: 2.7 MB (2660614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b2bf33f8e8bc113a559558c7e0fdc1f4e695b2bec89c09ccafc7f1dff9019`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 810.6 KB (810648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c0d1d2005390ed504d8dd433b7ce7c2f81d79abbc40e191d8e64e1d2b1729`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2fb164e25f84f88ebd54215876bc44293ae6dfd02646f473f87ea57cbbf853`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95455f9a86a6bacac05bdcca3ec35f202e59b2ace6dc2e5c14f3c1e1b154aab4`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460daad09d9d797d449205a3892eb7727250f88cb0fd838eb3da4477673c1bfd`  
		Last Modified: Thu, 21 Dec 2017 01:22:13 GMT  
		Size: 61.9 MB (61886207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab0d8c194a10785d610e3bc5a44fc56aebdc1b74d9475c1aed4690a23569518`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da624b820d4a1a38ffb4556bdd657dcea49c09fdfd356aa66b45a1d995b27`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9ad8e0e7784c98341e142dbd3bf28f8677fbbb98b85dbc7403a25779eb619`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.0.15` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:4b4cdf9d23dd03fb0de392555aca000ee07a04d2cd7524f23b1bc79600e2134b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5408818021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6731b906bb2bf8eb5d59f8f80e25cb6f1abb3457572f7730c9eae1945cd570e8`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:43:55 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:53:31 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:53:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fef99bf2799b9541f9c402c94b34d6956ad6af6bb8a3e27a8a01db14bb220`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31065debc73bc484363430f1d51f52e688c30017485223a31166a0a0303b8915`  
		Last Modified: Tue, 19 Dec 2017 04:07:10 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fd9f30823161ca0b37849fc3be9a0335985bb921f3c0cb803ca7b6032bdc5e`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb160f9367fa1c9e5e7f19405387c9a223f12e7b58e30933ef46c3d59358405a`  
		Last Modified: Tue, 19 Dec 2017 04:07:27 GMT  
		Size: 47.0 MB (46994564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add3786e86de14542bc7e6b0e40fd8437b9f9b6faab47fb1b3a498072f5cb79d`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12929d9801c71c998eb532a0cccfe18b3ec08feaa0f8b703442b72ab3c41185`  
		Last Modified: Tue, 19 Dec 2017 04:07:09 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a4787ad0ff4679d9818664e5258f86c202196a98c0a8c962163d03e78b685f`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.0.15` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:00389d2bd6ffd221dfd368ac17ecfc5e260eceb2047ee6863a71fbdc5bd75191
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2910420228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdbab21328ecf02ab2f68ac4290edca6369ec007e8168c943cb98ceebd36437`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:53:47 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:53:48 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:53:49 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:55:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:55:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:56:01 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:56:02 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a4f70e8a55dd9ea85316b97f10c7d87d64d891d4a3893db509966ddf56ca77`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3ea3f4e8d1ec0b6a063c611c64ffb2378d0ea00164896c00a217f03d1d5d8`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b39b3d13ed5c75186b92c5228062beafa6c75dc85824bf6ce76b7fdfefdeb0`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d712635eedd07152360df86c29be50fe9b990b6e6542bc774957a913a31c050`  
		Last Modified: Tue, 19 Dec 2017 04:07:52 GMT  
		Size: 46.6 MB (46586800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d2b16e18ce034f792da7086da5c088f939d755a4cdb266e8daae630494f63`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15104271b3f326fbb100b4c990b242c7c5e2da4f1dc143fb1d7a517df9edd65`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce9f53f93a4baac40828dea63b2616bab3b23f5d5c007506f00400fa4c2510`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0.15-wheezy`

```console
$ docker pull mongo@sha256:b2534b3119e159ee021c15600e67ad6945fa6eb5bf40e5f20defeae807734d69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.0.15-wheezy` - linux; amd64

```console
$ docker pull mongo@sha256:77f22f913d8e62559b58437df321f02aabd6beeb863b5292c66c175716846f60
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84530333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28cba33aad0327cf5df59ca2cbea98487692775937b9b05d0a7d7780952ba11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:46:27 GMT
ADD file:664e20ea0b4805f811ed279f86823b281c39df127d0f73ae147468bc1a9e4020 in / 
# Tue, 12 Dec 2017 01:46:27 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:35:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:35:31 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 12 Dec 2017 02:35:43 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 		procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:15:47 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:15:47 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:16:02 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:16:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:16:05 GMT
ENV GPG_KEYS=492EAFE8CD016A07919F1D2B9ECBEC467F0CEB10
# Thu, 21 Dec 2017 01:16:06 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_MAJOR=3.0
# Thu, 21 Dec 2017 01:16:08 GMT
ENV MONGO_VERSION=3.0.15
# Thu, 21 Dec 2017 01:16:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian wheezy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:16:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:16:24 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:16:24 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:16:26 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:16:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b967c325a8b3055106908c059240f7ea99c3b22958080fa3a0c1688e1e6739d1`  
		Last Modified: Tue, 12 Dec 2017 02:00:41 GMT  
		Size: 19.2 MB (19164678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4b68f5594ff127e3c87e19190ca62d695d260de2c4e1dfbc1a110dab8e2de`  
		Last Modified: Tue, 12 Dec 2017 02:41:17 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24baba5a242ee93e67a0fcfe657c4944872fd9fd2a064328454997b46cdbd62`  
		Last Modified: Tue, 12 Dec 2017 02:41:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11f2476fef6def7b28fd2c24f84397a099411ed68ad67cf937d5f9b76a82d7`  
		Last Modified: Tue, 12 Dec 2017 02:41:15 GMT  
		Size: 2.7 MB (2660614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b2bf33f8e8bc113a559558c7e0fdc1f4e695b2bec89c09ccafc7f1dff9019`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 810.6 KB (810648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c0d1d2005390ed504d8dd433b7ce7c2f81d79abbc40e191d8e64e1d2b1729`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2fb164e25f84f88ebd54215876bc44293ae6dfd02646f473f87ea57cbbf853`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95455f9a86a6bacac05bdcca3ec35f202e59b2ace6dc2e5c14f3c1e1b154aab4`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460daad09d9d797d449205a3892eb7727250f88cb0fd838eb3da4477673c1bfd`  
		Last Modified: Thu, 21 Dec 2017 01:22:13 GMT  
		Size: 61.9 MB (61886207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab0d8c194a10785d610e3bc5a44fc56aebdc1b74d9475c1aed4690a23569518`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da624b820d4a1a38ffb4556bdd657dcea49c09fdfd356aa66b45a1d995b27`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9ad8e0e7784c98341e142dbd3bf28f8677fbbb98b85dbc7403a25779eb619`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0.15-windowsservercore`

```console
$ docker pull mongo@sha256:e12029b7e8f626dea87234dd80b10d4a57f799cca53552c974236c975d622643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.0.15-windowsservercore` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:4b4cdf9d23dd03fb0de392555aca000ee07a04d2cd7524f23b1bc79600e2134b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5408818021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6731b906bb2bf8eb5d59f8f80e25cb6f1abb3457572f7730c9eae1945cd570e8`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:43:55 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:53:31 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:53:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fef99bf2799b9541f9c402c94b34d6956ad6af6bb8a3e27a8a01db14bb220`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31065debc73bc484363430f1d51f52e688c30017485223a31166a0a0303b8915`  
		Last Modified: Tue, 19 Dec 2017 04:07:10 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fd9f30823161ca0b37849fc3be9a0335985bb921f3c0cb803ca7b6032bdc5e`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb160f9367fa1c9e5e7f19405387c9a223f12e7b58e30933ef46c3d59358405a`  
		Last Modified: Tue, 19 Dec 2017 04:07:27 GMT  
		Size: 47.0 MB (46994564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add3786e86de14542bc7e6b0e40fd8437b9f9b6faab47fb1b3a498072f5cb79d`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12929d9801c71c998eb532a0cccfe18b3ec08feaa0f8b703442b72ab3c41185`  
		Last Modified: Tue, 19 Dec 2017 04:07:09 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a4787ad0ff4679d9818664e5258f86c202196a98c0a8c962163d03e78b685f`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.0.15-windowsservercore` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:00389d2bd6ffd221dfd368ac17ecfc5e260eceb2047ee6863a71fbdc5bd75191
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2910420228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdbab21328ecf02ab2f68ac4290edca6369ec007e8168c943cb98ceebd36437`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:53:47 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:53:48 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:53:49 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:55:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:55:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:56:01 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:56:02 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a4f70e8a55dd9ea85316b97f10c7d87d64d891d4a3893db509966ddf56ca77`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3ea3f4e8d1ec0b6a063c611c64ffb2378d0ea00164896c00a217f03d1d5d8`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b39b3d13ed5c75186b92c5228062beafa6c75dc85824bf6ce76b7fdfefdeb0`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d712635eedd07152360df86c29be50fe9b990b6e6542bc774957a913a31c050`  
		Last Modified: Tue, 19 Dec 2017 04:07:52 GMT  
		Size: 46.6 MB (46586800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d2b16e18ce034f792da7086da5c088f939d755a4cdb266e8daae630494f63`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15104271b3f326fbb100b4c990b242c7c5e2da4f1dc143fb1d7a517df9edd65`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce9f53f93a4baac40828dea63b2616bab3b23f5d5c007506f00400fa4c2510`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0.15-windowsservercore-1709`

```console
$ docker pull mongo@sha256:e642279115a9cf54418580ea40439f0798498301e4f0f36efc7236a25dde7587
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.125; amd64

### `mongo:3.0.15-windowsservercore-1709` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:00389d2bd6ffd221dfd368ac17ecfc5e260eceb2047ee6863a71fbdc5bd75191
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2910420228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdbab21328ecf02ab2f68ac4290edca6369ec007e8168c943cb98ceebd36437`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:53:47 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:53:48 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:53:49 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:55:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:55:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:56:01 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:56:02 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a4f70e8a55dd9ea85316b97f10c7d87d64d891d4a3893db509966ddf56ca77`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3ea3f4e8d1ec0b6a063c611c64ffb2378d0ea00164896c00a217f03d1d5d8`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b39b3d13ed5c75186b92c5228062beafa6c75dc85824bf6ce76b7fdfefdeb0`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d712635eedd07152360df86c29be50fe9b990b6e6542bc774957a913a31c050`  
		Last Modified: Tue, 19 Dec 2017 04:07:52 GMT  
		Size: 46.6 MB (46586800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d2b16e18ce034f792da7086da5c088f939d755a4cdb266e8daae630494f63`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15104271b3f326fbb100b4c990b242c7c5e2da4f1dc143fb1d7a517df9edd65`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce9f53f93a4baac40828dea63b2616bab3b23f5d5c007506f00400fa4c2510`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0.15-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:8cd3f28d7652fabf62d3dd176e4c191e44420d75538ad097fe3c937251b17bd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `mongo:3.0.15-windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:4b4cdf9d23dd03fb0de392555aca000ee07a04d2cd7524f23b1bc79600e2134b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5408818021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6731b906bb2bf8eb5d59f8f80e25cb6f1abb3457572f7730c9eae1945cd570e8`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:43:55 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:53:31 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:53:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fef99bf2799b9541f9c402c94b34d6956ad6af6bb8a3e27a8a01db14bb220`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31065debc73bc484363430f1d51f52e688c30017485223a31166a0a0303b8915`  
		Last Modified: Tue, 19 Dec 2017 04:07:10 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fd9f30823161ca0b37849fc3be9a0335985bb921f3c0cb803ca7b6032bdc5e`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb160f9367fa1c9e5e7f19405387c9a223f12e7b58e30933ef46c3d59358405a`  
		Last Modified: Tue, 19 Dec 2017 04:07:27 GMT  
		Size: 47.0 MB (46994564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add3786e86de14542bc7e6b0e40fd8437b9f9b6faab47fb1b3a498072f5cb79d`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12929d9801c71c998eb532a0cccfe18b3ec08feaa0f8b703442b72ab3c41185`  
		Last Modified: Tue, 19 Dec 2017 04:07:09 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a4787ad0ff4679d9818664e5258f86c202196a98c0a8c962163d03e78b685f`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0-wheezy`

```console
$ docker pull mongo@sha256:b2534b3119e159ee021c15600e67ad6945fa6eb5bf40e5f20defeae807734d69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.0-wheezy` - linux; amd64

```console
$ docker pull mongo@sha256:77f22f913d8e62559b58437df321f02aabd6beeb863b5292c66c175716846f60
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84530333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28cba33aad0327cf5df59ca2cbea98487692775937b9b05d0a7d7780952ba11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:46:27 GMT
ADD file:664e20ea0b4805f811ed279f86823b281c39df127d0f73ae147468bc1a9e4020 in / 
# Tue, 12 Dec 2017 01:46:27 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:35:30 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:35:31 GMT
RUN echo 'deb http://deb.debian.org/debian wheezy-backports main' > /etc/apt/sources.list.d/backports.list
# Tue, 12 Dec 2017 02:35:43 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 		procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:15:47 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:15:47 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:16:02 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:16:05 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:16:05 GMT
ENV GPG_KEYS=492EAFE8CD016A07919F1D2B9ECBEC467F0CEB10
# Thu, 21 Dec 2017 01:16:06 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:16:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:16:07 GMT
ENV MONGO_MAJOR=3.0
# Thu, 21 Dec 2017 01:16:08 GMT
ENV MONGO_VERSION=3.0.15
# Thu, 21 Dec 2017 01:16:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian wheezy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:16:21 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:16:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:16:24 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:16:24 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:16:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:16:26 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:16:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:b967c325a8b3055106908c059240f7ea99c3b22958080fa3a0c1688e1e6739d1`  
		Last Modified: Tue, 12 Dec 2017 02:00:41 GMT  
		Size: 19.2 MB (19164678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f4b68f5594ff127e3c87e19190ca62d695d260de2c4e1dfbc1a110dab8e2de`  
		Last Modified: Tue, 12 Dec 2017 02:41:17 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24baba5a242ee93e67a0fcfe657c4944872fd9fd2a064328454997b46cdbd62`  
		Last Modified: Tue, 12 Dec 2017 02:41:16 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af11f2476fef6def7b28fd2c24f84397a099411ed68ad67cf937d5f9b76a82d7`  
		Last Modified: Tue, 12 Dec 2017 02:41:15 GMT  
		Size: 2.7 MB (2660614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b2bf33f8e8bc113a559558c7e0fdc1f4e695b2bec89c09ccafc7f1dff9019`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 810.6 KB (810648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2c0d1d2005390ed504d8dd433b7ce7c2f81d79abbc40e191d8e64e1d2b1729`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2fb164e25f84f88ebd54215876bc44293ae6dfd02646f473f87ea57cbbf853`  
		Last Modified: Thu, 21 Dec 2017 01:22:01 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95455f9a86a6bacac05bdcca3ec35f202e59b2ace6dc2e5c14f3c1e1b154aab4`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460daad09d9d797d449205a3892eb7727250f88cb0fd838eb3da4477673c1bfd`  
		Last Modified: Thu, 21 Dec 2017 01:22:13 GMT  
		Size: 61.9 MB (61886207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab0d8c194a10785d610e3bc5a44fc56aebdc1b74d9475c1aed4690a23569518`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424da624b820d4a1a38ffb4556bdd657dcea49c09fdfd356aa66b45a1d995b27`  
		Last Modified: Thu, 21 Dec 2017 01:21:59 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c9ad8e0e7784c98341e142dbd3bf28f8677fbbb98b85dbc7403a25779eb619`  
		Last Modified: Thu, 21 Dec 2017 01:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0-windowsservercore`

```console
$ docker pull mongo@sha256:e12029b7e8f626dea87234dd80b10d4a57f799cca53552c974236c975d622643
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.0-windowsservercore` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:4b4cdf9d23dd03fb0de392555aca000ee07a04d2cd7524f23b1bc79600e2134b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5408818021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6731b906bb2bf8eb5d59f8f80e25cb6f1abb3457572f7730c9eae1945cd570e8`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:43:55 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:53:31 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:53:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fef99bf2799b9541f9c402c94b34d6956ad6af6bb8a3e27a8a01db14bb220`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31065debc73bc484363430f1d51f52e688c30017485223a31166a0a0303b8915`  
		Last Modified: Tue, 19 Dec 2017 04:07:10 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fd9f30823161ca0b37849fc3be9a0335985bb921f3c0cb803ca7b6032bdc5e`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb160f9367fa1c9e5e7f19405387c9a223f12e7b58e30933ef46c3d59358405a`  
		Last Modified: Tue, 19 Dec 2017 04:07:27 GMT  
		Size: 47.0 MB (46994564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add3786e86de14542bc7e6b0e40fd8437b9f9b6faab47fb1b3a498072f5cb79d`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12929d9801c71c998eb532a0cccfe18b3ec08feaa0f8b703442b72ab3c41185`  
		Last Modified: Tue, 19 Dec 2017 04:07:09 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a4787ad0ff4679d9818664e5258f86c202196a98c0a8c962163d03e78b685f`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.0-windowsservercore` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:00389d2bd6ffd221dfd368ac17ecfc5e260eceb2047ee6863a71fbdc5bd75191
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2910420228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdbab21328ecf02ab2f68ac4290edca6369ec007e8168c943cb98ceebd36437`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:53:47 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:53:48 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:53:49 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:55:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:55:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:56:01 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:56:02 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a4f70e8a55dd9ea85316b97f10c7d87d64d891d4a3893db509966ddf56ca77`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3ea3f4e8d1ec0b6a063c611c64ffb2378d0ea00164896c00a217f03d1d5d8`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b39b3d13ed5c75186b92c5228062beafa6c75dc85824bf6ce76b7fdfefdeb0`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d712635eedd07152360df86c29be50fe9b990b6e6542bc774957a913a31c050`  
		Last Modified: Tue, 19 Dec 2017 04:07:52 GMT  
		Size: 46.6 MB (46586800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d2b16e18ce034f792da7086da5c088f939d755a4cdb266e8daae630494f63`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15104271b3f326fbb100b4c990b242c7c5e2da4f1dc143fb1d7a517df9edd65`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce9f53f93a4baac40828dea63b2616bab3b23f5d5c007506f00400fa4c2510`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0-windowsservercore-1709`

```console
$ docker pull mongo@sha256:e642279115a9cf54418580ea40439f0798498301e4f0f36efc7236a25dde7587
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.125; amd64

### `mongo:3.0-windowsservercore-1709` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:00389d2bd6ffd221dfd368ac17ecfc5e260eceb2047ee6863a71fbdc5bd75191
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2910420228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cdbab21328ecf02ab2f68ac4290edca6369ec007e8168c943cb98ceebd36437`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:53:47 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:53:48 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:53:49 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:55:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:55:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:56:01 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:56:02 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a4f70e8a55dd9ea85316b97f10c7d87d64d891d4a3893db509966ddf56ca77`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3ea3f4e8d1ec0b6a063c611c64ffb2378d0ea00164896c00a217f03d1d5d8`  
		Last Modified: Tue, 19 Dec 2017 04:07:41 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b39b3d13ed5c75186b92c5228062beafa6c75dc85824bf6ce76b7fdfefdeb0`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d712635eedd07152360df86c29be50fe9b990b6e6542bc774957a913a31c050`  
		Last Modified: Tue, 19 Dec 2017 04:07:52 GMT  
		Size: 46.6 MB (46586800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603d2b16e18ce034f792da7086da5c088f939d755a4cdb266e8daae630494f63`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15104271b3f326fbb100b4c990b242c7c5e2da4f1dc143fb1d7a517df9edd65`  
		Last Modified: Tue, 19 Dec 2017 04:07:38 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdce9f53f93a4baac40828dea63b2616bab3b23f5d5c007506f00400fa4c2510`  
		Last Modified: Tue, 19 Dec 2017 04:07:39 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:8cd3f28d7652fabf62d3dd176e4c191e44420d75538ad097fe3c937251b17bd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `mongo:3.0-windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:4b4cdf9d23dd03fb0de392555aca000ee07a04d2cd7524f23b1bc79600e2134b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5408818021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6731b906bb2bf8eb5d59f8f80e25cb6f1abb3457572f7730c9eae1945cd570e8`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_VERSION=3.0.15
# Wed, 13 Dec 2017 02:43:54 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.0.15-signed.msi
# Wed, 13 Dec 2017 02:43:55 GMT
ENV MONGO_DOWNLOAD_SHA256=0a10cb87da164df7a1d31180d2ea1f3b096dda6e3d7b9f95c184ef953a1677bb
# Wed, 13 Dec 2017 02:53:29 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:53:30 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:53:31 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:53:32 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fef99bf2799b9541f9c402c94b34d6956ad6af6bb8a3e27a8a01db14bb220`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31065debc73bc484363430f1d51f52e688c30017485223a31166a0a0303b8915`  
		Last Modified: Tue, 19 Dec 2017 04:07:10 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fd9f30823161ca0b37849fc3be9a0335985bb921f3c0cb803ca7b6032bdc5e`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb160f9367fa1c9e5e7f19405387c9a223f12e7b58e30933ef46c3d59358405a`  
		Last Modified: Tue, 19 Dec 2017 04:07:27 GMT  
		Size: 47.0 MB (46994564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add3786e86de14542bc7e6b0e40fd8437b9f9b6faab47fb1b3a498072f5cb79d`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12929d9801c71c998eb532a0cccfe18b3ec08feaa0f8b703442b72ab3c41185`  
		Last Modified: Tue, 19 Dec 2017 04:07:09 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a4787ad0ff4679d9818664e5258f86c202196a98c0a8c962163d03e78b685f`  
		Last Modified: Tue, 19 Dec 2017 04:07:08 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2`

```console
$ docker pull mongo@sha256:53470e94fbdc602a29dd6ecab712fba1d85509fb6f6c2e2ca3ae2de3aa899c15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.2` - linux; amd64

```console
$ docker pull mongo@sha256:99956969bc26f22650eae3c8ded898f1a0d2b172f8c3b12264459291e50b4d2c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104184765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a418e907f3f37c73be41c969e322962956b2a54e544084846ae4c85f503be7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:17:02 GMT
ENV GPG_KEYS=DFFA3DCF326E302C4787673A01C4E7FAAAB2461C 	42F3E95A2C4F08279C4960ADD68FA50FEA312927
# Thu, 21 Dec 2017 01:17:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:17:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:17:06 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_MAJOR=3.2
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_VERSION=3.2.18
# Thu, 21 Dec 2017 01:17:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:17:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:17:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:17:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:17:26 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:17:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:17:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:17:27 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:17:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc977f80d9b54fb489113d6bca4c2d46cb7ca05350b2aebb5600cfdbbab0fbf2`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 3.6 KB (3597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66827fc3b9db49a38fead890e65ee4cf13bd901f37d035a7fcbc50998ebc6966`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912770bc2c7515034fbfa85483723b7cd8218f77ace4a96b1b89f0626170252`  
		Last Modified: Thu, 21 Dec 2017 01:23:32 GMT  
		Size: 70.8 MB (70845919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708e66e1928c3fe6ce818cfb0b88572aba860e34e06eef5f1230dd89ec64cf99`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b508231daf5410e2319031abd5fd613c48381b6a38e837c14b5b5157f844dfe`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7323cb076d46824e7836df95dcd71ae59aa719bb207d189d0bcf78f26222bc90`  
		Last Modified: Thu, 21 Dec 2017 01:23:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.2` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:dbde78a735d50a29bb6d859fff596f91b014daefd8a1793312f02c4b42919a6a
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5419342240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5efd99f479fcc84f7597a41100a841e4e432d15597925b7193ac22584e1f93ad`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:56:13 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:56:14 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:56:15 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 02:58:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:58:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:58:29 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:58:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697dfa7cde4d0e474d11846a2d0df84865c8e551c8eb659f8a203eb48049e9a5`  
		Last Modified: Tue, 19 Dec 2017 04:08:11 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d076bca83fcb3d2ef0424de829e9b65f3c40e36f76b82e671c53d2a5db32b1bc`  
		Last Modified: Tue, 19 Dec 2017 04:08:14 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d9e889e4438f14bdb0eeae3d2cc95843e5668cee2fde6e88e93ddc2c056333`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1d6edaefa23958f3b70b79a0e0647d6c04e90fda82864a14d7f71e995c7c59`  
		Last Modified: Tue, 19 Dec 2017 04:08:25 GMT  
		Size: 57.5 MB (57518791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f134b93bb28baa9146c35fd7450857a75c5d660287edc050ddebccbd2995a7f`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcb2e49dd76ac7497e78243c85a3c6ba418532e6dd41c917aa21c6721032ea`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ef1bf01c653e6f7236f652ad644f3040f5ac1b5fbb5d21778d657a16e67045`  
		Last Modified: Tue, 19 Dec 2017 04:08:10 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.2` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:221495d2b9b7a642fa59fb6640c5bbc1efdfc0ec8fddd8b84e2b93b35bc9ab6b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2916434524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a0f0b7b41be06d7d22d922fbdb8183c10277249b84615c7adbdfabfd70345a`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:58:40 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:58:41 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:58:42 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 03:00:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:00:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:00:22 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:00:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b144e842ac867249c947aa0cf6cf59e6fcfbcc49e6efb2e7f0742dbc20ad51`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a66e6991fc46847e0d0c8add3693bab61b5b83da78d5c40608e55a28c2c58d`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8fb4692c41b99c2be66bd7f2a704c2e6d0ec417f74897ec824a4bcc63e6062`  
		Last Modified: Tue, 19 Dec 2017 04:08:38 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3901e8f2cbaccbbf2ed1272e07ccc92366ffd5ff3f102f07c431b332b52bbd`  
		Last Modified: Tue, 19 Dec 2017 04:08:52 GMT  
		Size: 52.6 MB (52601081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257eb31b051e51e455018425175f8873db12de2b0d695cf1801362366a6f19d6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3a97356c88a1060f27de644028c806b2ae706532c438abf9ab257d1eb0e6b`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cc34ffd5375d43282d15f2441bea0f89e1bba25a1d6315cc2f20b84cac17b6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2.18`

```console
$ docker pull mongo@sha256:53470e94fbdc602a29dd6ecab712fba1d85509fb6f6c2e2ca3ae2de3aa899c15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.2.18` - linux; amd64

```console
$ docker pull mongo@sha256:99956969bc26f22650eae3c8ded898f1a0d2b172f8c3b12264459291e50b4d2c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104184765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a418e907f3f37c73be41c969e322962956b2a54e544084846ae4c85f503be7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:17:02 GMT
ENV GPG_KEYS=DFFA3DCF326E302C4787673A01C4E7FAAAB2461C 	42F3E95A2C4F08279C4960ADD68FA50FEA312927
# Thu, 21 Dec 2017 01:17:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:17:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:17:06 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_MAJOR=3.2
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_VERSION=3.2.18
# Thu, 21 Dec 2017 01:17:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:17:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:17:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:17:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:17:26 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:17:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:17:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:17:27 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:17:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc977f80d9b54fb489113d6bca4c2d46cb7ca05350b2aebb5600cfdbbab0fbf2`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 3.6 KB (3597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66827fc3b9db49a38fead890e65ee4cf13bd901f37d035a7fcbc50998ebc6966`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912770bc2c7515034fbfa85483723b7cd8218f77ace4a96b1b89f0626170252`  
		Last Modified: Thu, 21 Dec 2017 01:23:32 GMT  
		Size: 70.8 MB (70845919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708e66e1928c3fe6ce818cfb0b88572aba860e34e06eef5f1230dd89ec64cf99`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b508231daf5410e2319031abd5fd613c48381b6a38e837c14b5b5157f844dfe`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7323cb076d46824e7836df95dcd71ae59aa719bb207d189d0bcf78f26222bc90`  
		Last Modified: Thu, 21 Dec 2017 01:23:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.2.18` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:dbde78a735d50a29bb6d859fff596f91b014daefd8a1793312f02c4b42919a6a
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5419342240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5efd99f479fcc84f7597a41100a841e4e432d15597925b7193ac22584e1f93ad`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:56:13 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:56:14 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:56:15 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 02:58:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:58:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:58:29 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:58:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697dfa7cde4d0e474d11846a2d0df84865c8e551c8eb659f8a203eb48049e9a5`  
		Last Modified: Tue, 19 Dec 2017 04:08:11 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d076bca83fcb3d2ef0424de829e9b65f3c40e36f76b82e671c53d2a5db32b1bc`  
		Last Modified: Tue, 19 Dec 2017 04:08:14 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d9e889e4438f14bdb0eeae3d2cc95843e5668cee2fde6e88e93ddc2c056333`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1d6edaefa23958f3b70b79a0e0647d6c04e90fda82864a14d7f71e995c7c59`  
		Last Modified: Tue, 19 Dec 2017 04:08:25 GMT  
		Size: 57.5 MB (57518791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f134b93bb28baa9146c35fd7450857a75c5d660287edc050ddebccbd2995a7f`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcb2e49dd76ac7497e78243c85a3c6ba418532e6dd41c917aa21c6721032ea`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ef1bf01c653e6f7236f652ad644f3040f5ac1b5fbb5d21778d657a16e67045`  
		Last Modified: Tue, 19 Dec 2017 04:08:10 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.2.18` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:221495d2b9b7a642fa59fb6640c5bbc1efdfc0ec8fddd8b84e2b93b35bc9ab6b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2916434524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a0f0b7b41be06d7d22d922fbdb8183c10277249b84615c7adbdfabfd70345a`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:58:40 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:58:41 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:58:42 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 03:00:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:00:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:00:22 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:00:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b144e842ac867249c947aa0cf6cf59e6fcfbcc49e6efb2e7f0742dbc20ad51`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a66e6991fc46847e0d0c8add3693bab61b5b83da78d5c40608e55a28c2c58d`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8fb4692c41b99c2be66bd7f2a704c2e6d0ec417f74897ec824a4bcc63e6062`  
		Last Modified: Tue, 19 Dec 2017 04:08:38 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3901e8f2cbaccbbf2ed1272e07ccc92366ffd5ff3f102f07c431b332b52bbd`  
		Last Modified: Tue, 19 Dec 2017 04:08:52 GMT  
		Size: 52.6 MB (52601081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257eb31b051e51e455018425175f8873db12de2b0d695cf1801362366a6f19d6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3a97356c88a1060f27de644028c806b2ae706532c438abf9ab257d1eb0e6b`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cc34ffd5375d43282d15f2441bea0f89e1bba25a1d6315cc2f20b84cac17b6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2.18-jessie`

```console
$ docker pull mongo@sha256:ac7624fb058e0258419803a4197ce4cd764095a860bfb428e9e8498d80fe4025
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.2.18-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:99956969bc26f22650eae3c8ded898f1a0d2b172f8c3b12264459291e50b4d2c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104184765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a418e907f3f37c73be41c969e322962956b2a54e544084846ae4c85f503be7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:17:02 GMT
ENV GPG_KEYS=DFFA3DCF326E302C4787673A01C4E7FAAAB2461C 	42F3E95A2C4F08279C4960ADD68FA50FEA312927
# Thu, 21 Dec 2017 01:17:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:17:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:17:06 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_MAJOR=3.2
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_VERSION=3.2.18
# Thu, 21 Dec 2017 01:17:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:17:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:17:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:17:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:17:26 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:17:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:17:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:17:27 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:17:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc977f80d9b54fb489113d6bca4c2d46cb7ca05350b2aebb5600cfdbbab0fbf2`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 3.6 KB (3597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66827fc3b9db49a38fead890e65ee4cf13bd901f37d035a7fcbc50998ebc6966`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912770bc2c7515034fbfa85483723b7cd8218f77ace4a96b1b89f0626170252`  
		Last Modified: Thu, 21 Dec 2017 01:23:32 GMT  
		Size: 70.8 MB (70845919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708e66e1928c3fe6ce818cfb0b88572aba860e34e06eef5f1230dd89ec64cf99`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b508231daf5410e2319031abd5fd613c48381b6a38e837c14b5b5157f844dfe`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7323cb076d46824e7836df95dcd71ae59aa719bb207d189d0bcf78f26222bc90`  
		Last Modified: Thu, 21 Dec 2017 01:23:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2.18-windowsservercore`

```console
$ docker pull mongo@sha256:fd93932dca86ffb105fcd27431b56c2b53673faf377244076f00407289260e11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.2.18-windowsservercore` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:dbde78a735d50a29bb6d859fff596f91b014daefd8a1793312f02c4b42919a6a
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5419342240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5efd99f479fcc84f7597a41100a841e4e432d15597925b7193ac22584e1f93ad`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:56:13 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:56:14 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:56:15 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 02:58:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:58:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:58:29 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:58:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697dfa7cde4d0e474d11846a2d0df84865c8e551c8eb659f8a203eb48049e9a5`  
		Last Modified: Tue, 19 Dec 2017 04:08:11 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d076bca83fcb3d2ef0424de829e9b65f3c40e36f76b82e671c53d2a5db32b1bc`  
		Last Modified: Tue, 19 Dec 2017 04:08:14 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d9e889e4438f14bdb0eeae3d2cc95843e5668cee2fde6e88e93ddc2c056333`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1d6edaefa23958f3b70b79a0e0647d6c04e90fda82864a14d7f71e995c7c59`  
		Last Modified: Tue, 19 Dec 2017 04:08:25 GMT  
		Size: 57.5 MB (57518791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f134b93bb28baa9146c35fd7450857a75c5d660287edc050ddebccbd2995a7f`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcb2e49dd76ac7497e78243c85a3c6ba418532e6dd41c917aa21c6721032ea`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ef1bf01c653e6f7236f652ad644f3040f5ac1b5fbb5d21778d657a16e67045`  
		Last Modified: Tue, 19 Dec 2017 04:08:10 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.2.18-windowsservercore` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:221495d2b9b7a642fa59fb6640c5bbc1efdfc0ec8fddd8b84e2b93b35bc9ab6b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2916434524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a0f0b7b41be06d7d22d922fbdb8183c10277249b84615c7adbdfabfd70345a`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:58:40 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:58:41 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:58:42 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 03:00:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:00:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:00:22 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:00:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b144e842ac867249c947aa0cf6cf59e6fcfbcc49e6efb2e7f0742dbc20ad51`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a66e6991fc46847e0d0c8add3693bab61b5b83da78d5c40608e55a28c2c58d`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8fb4692c41b99c2be66bd7f2a704c2e6d0ec417f74897ec824a4bcc63e6062`  
		Last Modified: Tue, 19 Dec 2017 04:08:38 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3901e8f2cbaccbbf2ed1272e07ccc92366ffd5ff3f102f07c431b332b52bbd`  
		Last Modified: Tue, 19 Dec 2017 04:08:52 GMT  
		Size: 52.6 MB (52601081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257eb31b051e51e455018425175f8873db12de2b0d695cf1801362366a6f19d6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3a97356c88a1060f27de644028c806b2ae706532c438abf9ab257d1eb0e6b`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cc34ffd5375d43282d15f2441bea0f89e1bba25a1d6315cc2f20b84cac17b6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2.18-windowsservercore-1709`

```console
$ docker pull mongo@sha256:65c8e9ed61dadd86792ef01107942c9af9e051466e82e1ea67bc32ac24719b20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.125; amd64

### `mongo:3.2.18-windowsservercore-1709` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:221495d2b9b7a642fa59fb6640c5bbc1efdfc0ec8fddd8b84e2b93b35bc9ab6b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2916434524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a0f0b7b41be06d7d22d922fbdb8183c10277249b84615c7adbdfabfd70345a`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:58:40 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:58:41 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:58:42 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 03:00:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:00:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:00:22 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:00:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b144e842ac867249c947aa0cf6cf59e6fcfbcc49e6efb2e7f0742dbc20ad51`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a66e6991fc46847e0d0c8add3693bab61b5b83da78d5c40608e55a28c2c58d`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8fb4692c41b99c2be66bd7f2a704c2e6d0ec417f74897ec824a4bcc63e6062`  
		Last Modified: Tue, 19 Dec 2017 04:08:38 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3901e8f2cbaccbbf2ed1272e07ccc92366ffd5ff3f102f07c431b332b52bbd`  
		Last Modified: Tue, 19 Dec 2017 04:08:52 GMT  
		Size: 52.6 MB (52601081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257eb31b051e51e455018425175f8873db12de2b0d695cf1801362366a6f19d6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3a97356c88a1060f27de644028c806b2ae706532c438abf9ab257d1eb0e6b`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cc34ffd5375d43282d15f2441bea0f89e1bba25a1d6315cc2f20b84cac17b6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2.18-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:4ca988afc2c9acfa3be94244d24bc011688d20749ac8db617e42acf0f943d38e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `mongo:3.2.18-windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:dbde78a735d50a29bb6d859fff596f91b014daefd8a1793312f02c4b42919a6a
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5419342240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5efd99f479fcc84f7597a41100a841e4e432d15597925b7193ac22584e1f93ad`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:56:13 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:56:14 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:56:15 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 02:58:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:58:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:58:29 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:58:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697dfa7cde4d0e474d11846a2d0df84865c8e551c8eb659f8a203eb48049e9a5`  
		Last Modified: Tue, 19 Dec 2017 04:08:11 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d076bca83fcb3d2ef0424de829e9b65f3c40e36f76b82e671c53d2a5db32b1bc`  
		Last Modified: Tue, 19 Dec 2017 04:08:14 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d9e889e4438f14bdb0eeae3d2cc95843e5668cee2fde6e88e93ddc2c056333`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1d6edaefa23958f3b70b79a0e0647d6c04e90fda82864a14d7f71e995c7c59`  
		Last Modified: Tue, 19 Dec 2017 04:08:25 GMT  
		Size: 57.5 MB (57518791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f134b93bb28baa9146c35fd7450857a75c5d660287edc050ddebccbd2995a7f`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcb2e49dd76ac7497e78243c85a3c6ba418532e6dd41c917aa21c6721032ea`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ef1bf01c653e6f7236f652ad644f3040f5ac1b5fbb5d21778d657a16e67045`  
		Last Modified: Tue, 19 Dec 2017 04:08:10 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2-jessie`

```console
$ docker pull mongo@sha256:ac7624fb058e0258419803a4197ce4cd764095a860bfb428e9e8498d80fe4025
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.2-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:99956969bc26f22650eae3c8ded898f1a0d2b172f8c3b12264459291e50b4d2c
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104184765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a418e907f3f37c73be41c969e322962956b2a54e544084846ae4c85f503be7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:17:02 GMT
ENV GPG_KEYS=DFFA3DCF326E302C4787673A01C4E7FAAAB2461C 	42F3E95A2C4F08279C4960ADD68FA50FEA312927
# Thu, 21 Dec 2017 01:17:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:17:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:17:06 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_MAJOR=3.2
# Thu, 21 Dec 2017 01:17:06 GMT
ENV MONGO_VERSION=3.2.18
# Thu, 21 Dec 2017 01:17:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:17:24 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:17:25 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:17:25 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:17:26 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:17:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:17:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:17:27 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:17:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc977f80d9b54fb489113d6bca4c2d46cb7ca05350b2aebb5600cfdbbab0fbf2`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 3.6 KB (3597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66827fc3b9db49a38fead890e65ee4cf13bd901f37d035a7fcbc50998ebc6966`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e912770bc2c7515034fbfa85483723b7cd8218f77ace4a96b1b89f0626170252`  
		Last Modified: Thu, 21 Dec 2017 01:23:32 GMT  
		Size: 70.8 MB (70845919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708e66e1928c3fe6ce818cfb0b88572aba860e34e06eef5f1230dd89ec64cf99`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b508231daf5410e2319031abd5fd613c48381b6a38e837c14b5b5157f844dfe`  
		Last Modified: Thu, 21 Dec 2017 01:23:18 GMT  
		Size: 3.6 KB (3569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7323cb076d46824e7836df95dcd71ae59aa719bb207d189d0bcf78f26222bc90`  
		Last Modified: Thu, 21 Dec 2017 01:23:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2-windowsservercore`

```console
$ docker pull mongo@sha256:fd93932dca86ffb105fcd27431b56c2b53673faf377244076f00407289260e11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.2-windowsservercore` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:dbde78a735d50a29bb6d859fff596f91b014daefd8a1793312f02c4b42919a6a
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5419342240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5efd99f479fcc84f7597a41100a841e4e432d15597925b7193ac22584e1f93ad`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:56:13 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:56:14 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:56:15 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 02:58:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:58:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:58:29 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:58:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697dfa7cde4d0e474d11846a2d0df84865c8e551c8eb659f8a203eb48049e9a5`  
		Last Modified: Tue, 19 Dec 2017 04:08:11 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d076bca83fcb3d2ef0424de829e9b65f3c40e36f76b82e671c53d2a5db32b1bc`  
		Last Modified: Tue, 19 Dec 2017 04:08:14 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d9e889e4438f14bdb0eeae3d2cc95843e5668cee2fde6e88e93ddc2c056333`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1d6edaefa23958f3b70b79a0e0647d6c04e90fda82864a14d7f71e995c7c59`  
		Last Modified: Tue, 19 Dec 2017 04:08:25 GMT  
		Size: 57.5 MB (57518791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f134b93bb28baa9146c35fd7450857a75c5d660287edc050ddebccbd2995a7f`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcb2e49dd76ac7497e78243c85a3c6ba418532e6dd41c917aa21c6721032ea`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ef1bf01c653e6f7236f652ad644f3040f5ac1b5fbb5d21778d657a16e67045`  
		Last Modified: Tue, 19 Dec 2017 04:08:10 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.2-windowsservercore` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:221495d2b9b7a642fa59fb6640c5bbc1efdfc0ec8fddd8b84e2b93b35bc9ab6b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2916434524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a0f0b7b41be06d7d22d922fbdb8183c10277249b84615c7adbdfabfd70345a`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:58:40 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:58:41 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:58:42 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 03:00:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:00:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:00:22 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:00:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b144e842ac867249c947aa0cf6cf59e6fcfbcc49e6efb2e7f0742dbc20ad51`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a66e6991fc46847e0d0c8add3693bab61b5b83da78d5c40608e55a28c2c58d`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8fb4692c41b99c2be66bd7f2a704c2e6d0ec417f74897ec824a4bcc63e6062`  
		Last Modified: Tue, 19 Dec 2017 04:08:38 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3901e8f2cbaccbbf2ed1272e07ccc92366ffd5ff3f102f07c431b332b52bbd`  
		Last Modified: Tue, 19 Dec 2017 04:08:52 GMT  
		Size: 52.6 MB (52601081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257eb31b051e51e455018425175f8873db12de2b0d695cf1801362366a6f19d6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3a97356c88a1060f27de644028c806b2ae706532c438abf9ab257d1eb0e6b`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cc34ffd5375d43282d15f2441bea0f89e1bba25a1d6315cc2f20b84cac17b6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2-windowsservercore-1709`

```console
$ docker pull mongo@sha256:65c8e9ed61dadd86792ef01107942c9af9e051466e82e1ea67bc32ac24719b20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.125; amd64

### `mongo:3.2-windowsservercore-1709` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:221495d2b9b7a642fa59fb6640c5bbc1efdfc0ec8fddd8b84e2b93b35bc9ab6b
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2916434524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a0f0b7b41be06d7d22d922fbdb8183c10277249b84615c7adbdfabfd70345a`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:58:40 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:58:41 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:58:42 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 03:00:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:00:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:00:22 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:00:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b144e842ac867249c947aa0cf6cf59e6fcfbcc49e6efb2e7f0742dbc20ad51`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a66e6991fc46847e0d0c8add3693bab61b5b83da78d5c40608e55a28c2c58d`  
		Last Modified: Tue, 19 Dec 2017 04:08:40 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8fb4692c41b99c2be66bd7f2a704c2e6d0ec417f74897ec824a4bcc63e6062`  
		Last Modified: Tue, 19 Dec 2017 04:08:38 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3901e8f2cbaccbbf2ed1272e07ccc92366ffd5ff3f102f07c431b332b52bbd`  
		Last Modified: Tue, 19 Dec 2017 04:08:52 GMT  
		Size: 52.6 MB (52601081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257eb31b051e51e455018425175f8873db12de2b0d695cf1801362366a6f19d6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad3a97356c88a1060f27de644028c806b2ae706532c438abf9ab257d1eb0e6b`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cc34ffd5375d43282d15f2441bea0f89e1bba25a1d6315cc2f20b84cac17b6`  
		Last Modified: Tue, 19 Dec 2017 04:08:37 GMT  
		Size: 1.2 KB (1198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:4ca988afc2c9acfa3be94244d24bc011688d20749ac8db617e42acf0f943d38e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `mongo:3.2-windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:dbde78a735d50a29bb6d859fff596f91b014daefd8a1793312f02c4b42919a6a
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5419342240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5efd99f479fcc84f7597a41100a841e4e432d15597925b7193ac22584e1f93ad`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 02:56:13 GMT
ENV MONGO_VERSION=3.2.18
# Wed, 13 Dec 2017 02:56:14 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.2.18-signed.msi
# Wed, 13 Dec 2017 02:56:15 GMT
ENV MONGO_DOWNLOAD_SHA256=f86aba3b01fc3b50ffecfe1ae11cd9d3e0456b3e84cc25e9cc2eb40bcfa40452
# Wed, 13 Dec 2017 02:58:26 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 02:58:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 02:58:29 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 02:58:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697dfa7cde4d0e474d11846a2d0df84865c8e551c8eb659f8a203eb48049e9a5`  
		Last Modified: Tue, 19 Dec 2017 04:08:11 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d076bca83fcb3d2ef0424de829e9b65f3c40e36f76b82e671c53d2a5db32b1bc`  
		Last Modified: Tue, 19 Dec 2017 04:08:14 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d9e889e4438f14bdb0eeae3d2cc95843e5668cee2fde6e88e93ddc2c056333`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1d6edaefa23958f3b70b79a0e0647d6c04e90fda82864a14d7f71e995c7c59`  
		Last Modified: Tue, 19 Dec 2017 04:08:25 GMT  
		Size: 57.5 MB (57518791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f134b93bb28baa9146c35fd7450857a75c5d660287edc050ddebccbd2995a7f`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcb2e49dd76ac7497e78243c85a3c6ba418532e6dd41c917aa21c6721032ea`  
		Last Modified: Tue, 19 Dec 2017 04:08:09 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ef1bf01c653e6f7236f652ad644f3040f5ac1b5fbb5d21778d657a16e67045`  
		Last Modified: Tue, 19 Dec 2017 04:08:10 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4`

```console
$ docker pull mongo@sha256:0b60ff501b450f30010eae11a279bb9364a7e8f7459bc7601434957f4c019c10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.4` - linux; amd64

```console
$ docker pull mongo@sha256:77dd9838010b4de7f7274d4b3a0cf57fe51890de2f284dc80e81f752ff883550
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131854682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905a87e116de6dcfc7860d2c24afaf4b87ee0c8db295494a144a1a3d24ac1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:19:41 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 21 Dec 2017 01:19:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_MAJOR=3.4
# Thu, 21 Dec 2017 01:19:45 GMT
ENV MONGO_VERSION=3.4.10
# Thu, 21 Dec 2017 01:19:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:20:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:20:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:20:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:20:54 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:20:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:20:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:20:56 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:20:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b17a05532222a454ee2adb0f8fb5e1e189f20b5a732082107712a92f0d5c784`  
		Last Modified: Thu, 21 Dec 2017 01:24:00 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723351cb8b477e49637a166a9f6e1392c8ecdcef5df971d33348e2aeaecd3e7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd8437755a7eca2d118b41346592b0e55d4529d05aedc5180563d26b2c832e`  
		Last Modified: Thu, 21 Dec 2017 01:24:16 GMT  
		Size: 98.5 MB (98517998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61012c0435729d9c1eb7125e91a3db7ffa9492e1224ee9fe356415df24d11ad7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aeb242d479c37f92572a4077aba093f3433e0401c9a56d3391dff44861e370`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 3.6 KB (3571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc8171e92f4532da660f8d79d2d40ea612c785860ae359be8f463e525f0230c`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:e66a905109292a8d27c89f50c4d08c31a5bb8074cf66d5413eaebd67b15e5162
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5429497767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ec78caa0215927ffe98d1d2a4cd2a40de7d244b69b7408cd88093180bf8fda`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:00:37 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:00:38 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:00:39 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:02:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:02:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:02:46 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:02:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baabcbaac6b1ea90ee37f64c65b56fbd5820d2830440bd97f25b389de1ac7ffa`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b2879821df58c2a8ee8a0c67d6dcc088e61115241cbcb844587a4b7ab39add`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b6754af4adde273c46d7cf0fe3567e8abc00d305b4234221f04a2c0c391192`  
		Last Modified: Tue, 19 Dec 2017 04:09:05 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b967eaee48d3ada8b70cd927f3d58f3aa388bcdc3c3e867a734133a4edf73d6e`  
		Last Modified: Tue, 19 Dec 2017 04:09:22 GMT  
		Size: 67.7 MB (67674311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dabd9cd2b6f531b7deb401ce402d18398f65a00bd85ab748d639b3a93e5936`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbea43d3b1a6a636e0d617e4bdf7a2006004a69f1a86dc2d858eda24c9ec165`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cd6814fa168c62d43235366fa45ad34f22ea265954c30075a6845d7c4540f5`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:29302f0f0eee02cb1df6ecedb46c0ba3f2e51c2a47379f4ad7de5795e0e8c332
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2926599685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba42d72049e85b3e5b42280dfd62ed78e80bb8e7101d91b64e16840ad5fa6959`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:03:04 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:04:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:04:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:04:55 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:04:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3897e104207f2d5fcfbeb59db966ec737475f376aaf98b3b77e20bd0d28a99`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f909469ec493bd10b7bad5b5fb130796da35ceffdd10017495d139676f7cd`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2306bda02ae76915dce1b47898ce5b4599e9cd01ef0dbe5abfa25fdeb461a1`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8495b3df676b97f4c3e13a85c40754d9e20c470e12801f3333501163338ed`  
		Last Modified: Tue, 19 Dec 2017 04:09:52 GMT  
		Size: 62.8 MB (62766246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9a53e77635aaccd959073dcf5e3923c5240a7e5bfb8899bc5a63a91e91b7e`  
		Last Modified: Tue, 19 Dec 2017 04:09:35 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebecba35c2e569980a8b7b04578cf30e0d719bbb9a7dbbf5f6e103cae3d7fd2a`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286875f590bc8985af9b15c002756168e9695752fa557785aea4a360c886318`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.10`

```console
$ docker pull mongo@sha256:0b60ff501b450f30010eae11a279bb9364a7e8f7459bc7601434957f4c019c10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.4.10` - linux; amd64

```console
$ docker pull mongo@sha256:77dd9838010b4de7f7274d4b3a0cf57fe51890de2f284dc80e81f752ff883550
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131854682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905a87e116de6dcfc7860d2c24afaf4b87ee0c8db295494a144a1a3d24ac1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:19:41 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 21 Dec 2017 01:19:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_MAJOR=3.4
# Thu, 21 Dec 2017 01:19:45 GMT
ENV MONGO_VERSION=3.4.10
# Thu, 21 Dec 2017 01:19:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:20:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:20:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:20:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:20:54 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:20:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:20:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:20:56 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:20:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b17a05532222a454ee2adb0f8fb5e1e189f20b5a732082107712a92f0d5c784`  
		Last Modified: Thu, 21 Dec 2017 01:24:00 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723351cb8b477e49637a166a9f6e1392c8ecdcef5df971d33348e2aeaecd3e7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd8437755a7eca2d118b41346592b0e55d4529d05aedc5180563d26b2c832e`  
		Last Modified: Thu, 21 Dec 2017 01:24:16 GMT  
		Size: 98.5 MB (98517998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61012c0435729d9c1eb7125e91a3db7ffa9492e1224ee9fe356415df24d11ad7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aeb242d479c37f92572a4077aba093f3433e0401c9a56d3391dff44861e370`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 3.6 KB (3571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc8171e92f4532da660f8d79d2d40ea612c785860ae359be8f463e525f0230c`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4.10` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:e66a905109292a8d27c89f50c4d08c31a5bb8074cf66d5413eaebd67b15e5162
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5429497767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ec78caa0215927ffe98d1d2a4cd2a40de7d244b69b7408cd88093180bf8fda`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:00:37 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:00:38 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:00:39 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:02:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:02:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:02:46 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:02:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baabcbaac6b1ea90ee37f64c65b56fbd5820d2830440bd97f25b389de1ac7ffa`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b2879821df58c2a8ee8a0c67d6dcc088e61115241cbcb844587a4b7ab39add`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b6754af4adde273c46d7cf0fe3567e8abc00d305b4234221f04a2c0c391192`  
		Last Modified: Tue, 19 Dec 2017 04:09:05 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b967eaee48d3ada8b70cd927f3d58f3aa388bcdc3c3e867a734133a4edf73d6e`  
		Last Modified: Tue, 19 Dec 2017 04:09:22 GMT  
		Size: 67.7 MB (67674311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dabd9cd2b6f531b7deb401ce402d18398f65a00bd85ab748d639b3a93e5936`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbea43d3b1a6a636e0d617e4bdf7a2006004a69f1a86dc2d858eda24c9ec165`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cd6814fa168c62d43235366fa45ad34f22ea265954c30075a6845d7c4540f5`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4.10` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:29302f0f0eee02cb1df6ecedb46c0ba3f2e51c2a47379f4ad7de5795e0e8c332
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2926599685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba42d72049e85b3e5b42280dfd62ed78e80bb8e7101d91b64e16840ad5fa6959`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:03:04 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:04:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:04:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:04:55 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:04:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3897e104207f2d5fcfbeb59db966ec737475f376aaf98b3b77e20bd0d28a99`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f909469ec493bd10b7bad5b5fb130796da35ceffdd10017495d139676f7cd`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2306bda02ae76915dce1b47898ce5b4599e9cd01ef0dbe5abfa25fdeb461a1`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8495b3df676b97f4c3e13a85c40754d9e20c470e12801f3333501163338ed`  
		Last Modified: Tue, 19 Dec 2017 04:09:52 GMT  
		Size: 62.8 MB (62766246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9a53e77635aaccd959073dcf5e3923c5240a7e5bfb8899bc5a63a91e91b7e`  
		Last Modified: Tue, 19 Dec 2017 04:09:35 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebecba35c2e569980a8b7b04578cf30e0d719bbb9a7dbbf5f6e103cae3d7fd2a`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286875f590bc8985af9b15c002756168e9695752fa557785aea4a360c886318`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.10-jessie`

```console
$ docker pull mongo@sha256:38829565a5781afeecb287a6a2da6535396712718a63a4e2dcc7f006a0611cd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.4.10-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:77dd9838010b4de7f7274d4b3a0cf57fe51890de2f284dc80e81f752ff883550
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131854682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905a87e116de6dcfc7860d2c24afaf4b87ee0c8db295494a144a1a3d24ac1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:19:41 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 21 Dec 2017 01:19:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_MAJOR=3.4
# Thu, 21 Dec 2017 01:19:45 GMT
ENV MONGO_VERSION=3.4.10
# Thu, 21 Dec 2017 01:19:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:20:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:20:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:20:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:20:54 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:20:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:20:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:20:56 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:20:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b17a05532222a454ee2adb0f8fb5e1e189f20b5a732082107712a92f0d5c784`  
		Last Modified: Thu, 21 Dec 2017 01:24:00 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723351cb8b477e49637a166a9f6e1392c8ecdcef5df971d33348e2aeaecd3e7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd8437755a7eca2d118b41346592b0e55d4529d05aedc5180563d26b2c832e`  
		Last Modified: Thu, 21 Dec 2017 01:24:16 GMT  
		Size: 98.5 MB (98517998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61012c0435729d9c1eb7125e91a3db7ffa9492e1224ee9fe356415df24d11ad7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aeb242d479c37f92572a4077aba093f3433e0401c9a56d3391dff44861e370`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 3.6 KB (3571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc8171e92f4532da660f8d79d2d40ea612c785860ae359be8f463e525f0230c`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.10-windowsservercore`

```console
$ docker pull mongo@sha256:7aa2a83b38bbb41dbeeb86387fc536d43977b15d43ed9b8d1dcef0d62007b0d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.4.10-windowsservercore` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:e66a905109292a8d27c89f50c4d08c31a5bb8074cf66d5413eaebd67b15e5162
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5429497767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ec78caa0215927ffe98d1d2a4cd2a40de7d244b69b7408cd88093180bf8fda`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:00:37 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:00:38 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:00:39 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:02:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:02:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:02:46 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:02:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baabcbaac6b1ea90ee37f64c65b56fbd5820d2830440bd97f25b389de1ac7ffa`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b2879821df58c2a8ee8a0c67d6dcc088e61115241cbcb844587a4b7ab39add`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b6754af4adde273c46d7cf0fe3567e8abc00d305b4234221f04a2c0c391192`  
		Last Modified: Tue, 19 Dec 2017 04:09:05 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b967eaee48d3ada8b70cd927f3d58f3aa388bcdc3c3e867a734133a4edf73d6e`  
		Last Modified: Tue, 19 Dec 2017 04:09:22 GMT  
		Size: 67.7 MB (67674311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dabd9cd2b6f531b7deb401ce402d18398f65a00bd85ab748d639b3a93e5936`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbea43d3b1a6a636e0d617e4bdf7a2006004a69f1a86dc2d858eda24c9ec165`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cd6814fa168c62d43235366fa45ad34f22ea265954c30075a6845d7c4540f5`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4.10-windowsservercore` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:29302f0f0eee02cb1df6ecedb46c0ba3f2e51c2a47379f4ad7de5795e0e8c332
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2926599685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba42d72049e85b3e5b42280dfd62ed78e80bb8e7101d91b64e16840ad5fa6959`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:03:04 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:04:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:04:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:04:55 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:04:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3897e104207f2d5fcfbeb59db966ec737475f376aaf98b3b77e20bd0d28a99`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f909469ec493bd10b7bad5b5fb130796da35ceffdd10017495d139676f7cd`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2306bda02ae76915dce1b47898ce5b4599e9cd01ef0dbe5abfa25fdeb461a1`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8495b3df676b97f4c3e13a85c40754d9e20c470e12801f3333501163338ed`  
		Last Modified: Tue, 19 Dec 2017 04:09:52 GMT  
		Size: 62.8 MB (62766246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9a53e77635aaccd959073dcf5e3923c5240a7e5bfb8899bc5a63a91e91b7e`  
		Last Modified: Tue, 19 Dec 2017 04:09:35 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebecba35c2e569980a8b7b04578cf30e0d719bbb9a7dbbf5f6e103cae3d7fd2a`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286875f590bc8985af9b15c002756168e9695752fa557785aea4a360c886318`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.10-windowsservercore-1709`

```console
$ docker pull mongo@sha256:b54357b02c9de5b60a13d54d6db47a46d4f6b7f47a80c0b963a9e031629866bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.125; amd64

### `mongo:3.4.10-windowsservercore-1709` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:29302f0f0eee02cb1df6ecedb46c0ba3f2e51c2a47379f4ad7de5795e0e8c332
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2926599685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba42d72049e85b3e5b42280dfd62ed78e80bb8e7101d91b64e16840ad5fa6959`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:03:04 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:04:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:04:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:04:55 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:04:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3897e104207f2d5fcfbeb59db966ec737475f376aaf98b3b77e20bd0d28a99`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f909469ec493bd10b7bad5b5fb130796da35ceffdd10017495d139676f7cd`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2306bda02ae76915dce1b47898ce5b4599e9cd01ef0dbe5abfa25fdeb461a1`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8495b3df676b97f4c3e13a85c40754d9e20c470e12801f3333501163338ed`  
		Last Modified: Tue, 19 Dec 2017 04:09:52 GMT  
		Size: 62.8 MB (62766246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9a53e77635aaccd959073dcf5e3923c5240a7e5bfb8899bc5a63a91e91b7e`  
		Last Modified: Tue, 19 Dec 2017 04:09:35 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebecba35c2e569980a8b7b04578cf30e0d719bbb9a7dbbf5f6e103cae3d7fd2a`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286875f590bc8985af9b15c002756168e9695752fa557785aea4a360c886318`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.10-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:1e30ccadf1ae1a8781f2782c8160a1ec9c326b295bdafda4cd94e1c1bffc6e78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `mongo:3.4.10-windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:e66a905109292a8d27c89f50c4d08c31a5bb8074cf66d5413eaebd67b15e5162
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5429497767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ec78caa0215927ffe98d1d2a4cd2a40de7d244b69b7408cd88093180bf8fda`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:00:37 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:00:38 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:00:39 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:02:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:02:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:02:46 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:02:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baabcbaac6b1ea90ee37f64c65b56fbd5820d2830440bd97f25b389de1ac7ffa`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b2879821df58c2a8ee8a0c67d6dcc088e61115241cbcb844587a4b7ab39add`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b6754af4adde273c46d7cf0fe3567e8abc00d305b4234221f04a2c0c391192`  
		Last Modified: Tue, 19 Dec 2017 04:09:05 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b967eaee48d3ada8b70cd927f3d58f3aa388bcdc3c3e867a734133a4edf73d6e`  
		Last Modified: Tue, 19 Dec 2017 04:09:22 GMT  
		Size: 67.7 MB (67674311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dabd9cd2b6f531b7deb401ce402d18398f65a00bd85ab748d639b3a93e5936`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbea43d3b1a6a636e0d617e4bdf7a2006004a69f1a86dc2d858eda24c9ec165`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cd6814fa168c62d43235366fa45ad34f22ea265954c30075a6845d7c4540f5`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4-jessie`

```console
$ docker pull mongo@sha256:38829565a5781afeecb287a6a2da6535396712718a63a4e2dcc7f006a0611cd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.4-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:77dd9838010b4de7f7274d4b3a0cf57fe51890de2f284dc80e81f752ff883550
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131854682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e905a87e116de6dcfc7860d2c24afaf4b87ee0c8db295494a144a1a3d24ac1ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:19:41 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 21 Dec 2017 01:19:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:19:44 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:19:44 GMT
ENV MONGO_MAJOR=3.4
# Thu, 21 Dec 2017 01:19:45 GMT
ENV MONGO_VERSION=3.4.10
# Thu, 21 Dec 2017 01:19:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 21 Dec 2017 01:20:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 21 Dec 2017 01:20:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 21 Dec 2017 01:20:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 21 Dec 2017 01:20:54 GMT
COPY file:536cddf4d6e1f87efc5d647e6253f8eefcd6e23caf8860574fbd37e620e4683f in /usr/local/bin/ 
# Thu, 21 Dec 2017 01:20:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 21 Dec 2017 01:20:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Dec 2017 01:20:56 GMT
EXPOSE 27017/tcp
# Thu, 21 Dec 2017 01:20:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b17a05532222a454ee2adb0f8fb5e1e189f20b5a732082107712a92f0d5c784`  
		Last Modified: Thu, 21 Dec 2017 01:24:00 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1723351cb8b477e49637a166a9f6e1392c8ecdcef5df971d33348e2aeaecd3e7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dd8437755a7eca2d118b41346592b0e55d4529d05aedc5180563d26b2c832e`  
		Last Modified: Thu, 21 Dec 2017 01:24:16 GMT  
		Size: 98.5 MB (98517998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61012c0435729d9c1eb7125e91a3db7ffa9492e1224ee9fe356415df24d11ad7`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76aeb242d479c37f92572a4077aba093f3433e0401c9a56d3391dff44861e370`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 3.6 KB (3571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc8171e92f4532da660f8d79d2d40ea612c785860ae359be8f463e525f0230c`  
		Last Modified: Thu, 21 Dec 2017 01:23:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4-windowsservercore`

```console
$ docker pull mongo@sha256:7aa2a83b38bbb41dbeeb86387fc536d43977b15d43ed9b8d1dcef0d62007b0d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.4-windowsservercore` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:e66a905109292a8d27c89f50c4d08c31a5bb8074cf66d5413eaebd67b15e5162
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5429497767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ec78caa0215927ffe98d1d2a4cd2a40de7d244b69b7408cd88093180bf8fda`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:00:37 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:00:38 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:00:39 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:02:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:02:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:02:46 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:02:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baabcbaac6b1ea90ee37f64c65b56fbd5820d2830440bd97f25b389de1ac7ffa`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b2879821df58c2a8ee8a0c67d6dcc088e61115241cbcb844587a4b7ab39add`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b6754af4adde273c46d7cf0fe3567e8abc00d305b4234221f04a2c0c391192`  
		Last Modified: Tue, 19 Dec 2017 04:09:05 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b967eaee48d3ada8b70cd927f3d58f3aa388bcdc3c3e867a734133a4edf73d6e`  
		Last Modified: Tue, 19 Dec 2017 04:09:22 GMT  
		Size: 67.7 MB (67674311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dabd9cd2b6f531b7deb401ce402d18398f65a00bd85ab748d639b3a93e5936`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbea43d3b1a6a636e0d617e4bdf7a2006004a69f1a86dc2d858eda24c9ec165`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cd6814fa168c62d43235366fa45ad34f22ea265954c30075a6845d7c4540f5`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4-windowsservercore` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:29302f0f0eee02cb1df6ecedb46c0ba3f2e51c2a47379f4ad7de5795e0e8c332
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2926599685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba42d72049e85b3e5b42280dfd62ed78e80bb8e7101d91b64e16840ad5fa6959`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:03:04 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:04:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:04:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:04:55 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:04:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3897e104207f2d5fcfbeb59db966ec737475f376aaf98b3b77e20bd0d28a99`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f909469ec493bd10b7bad5b5fb130796da35ceffdd10017495d139676f7cd`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2306bda02ae76915dce1b47898ce5b4599e9cd01ef0dbe5abfa25fdeb461a1`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8495b3df676b97f4c3e13a85c40754d9e20c470e12801f3333501163338ed`  
		Last Modified: Tue, 19 Dec 2017 04:09:52 GMT  
		Size: 62.8 MB (62766246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9a53e77635aaccd959073dcf5e3923c5240a7e5bfb8899bc5a63a91e91b7e`  
		Last Modified: Tue, 19 Dec 2017 04:09:35 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebecba35c2e569980a8b7b04578cf30e0d719bbb9a7dbbf5f6e103cae3d7fd2a`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286875f590bc8985af9b15c002756168e9695752fa557785aea4a360c886318`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4-windowsservercore-1709`

```console
$ docker pull mongo@sha256:b54357b02c9de5b60a13d54d6db47a46d4f6b7f47a80c0b963a9e031629866bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.125; amd64

### `mongo:3.4-windowsservercore-1709` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:29302f0f0eee02cb1df6ecedb46c0ba3f2e51c2a47379f4ad7de5795e0e8c332
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2926599685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba42d72049e85b3e5b42280dfd62ed78e80bb8e7101d91b64e16840ad5fa6959`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:03:04 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:03:05 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:04:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:04:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:04:55 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:04:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3897e104207f2d5fcfbeb59db966ec737475f376aaf98b3b77e20bd0d28a99`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3f909469ec493bd10b7bad5b5fb130796da35ceffdd10017495d139676f7cd`  
		Last Modified: Tue, 19 Dec 2017 04:09:38 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2306bda02ae76915dce1b47898ce5b4599e9cd01ef0dbe5abfa25fdeb461a1`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8495b3df676b97f4c3e13a85c40754d9e20c470e12801f3333501163338ed`  
		Last Modified: Tue, 19 Dec 2017 04:09:52 GMT  
		Size: 62.8 MB (62766246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad9a53e77635aaccd959073dcf5e3923c5240a7e5bfb8899bc5a63a91e91b7e`  
		Last Modified: Tue, 19 Dec 2017 04:09:35 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebecba35c2e569980a8b7b04578cf30e0d719bbb9a7dbbf5f6e103cae3d7fd2a`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286875f590bc8985af9b15c002756168e9695752fa557785aea4a360c886318`  
		Last Modified: Tue, 19 Dec 2017 04:09:36 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:1e30ccadf1ae1a8781f2782c8160a1ec9c326b295bdafda4cd94e1c1bffc6e78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `mongo:3.4-windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:e66a905109292a8d27c89f50c4d08c31a5bb8074cf66d5413eaebd67b15e5162
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 GB (5429497767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ec78caa0215927ffe98d1d2a4cd2a40de7d244b69b7408cd88093180bf8fda`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Dec 2017 03:00:37 GMT
ENV MONGO_VERSION=3.4.10
# Wed, 13 Dec 2017 03:00:38 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.10-signed.msi
# Wed, 13 Dec 2017 03:00:39 GMT
ENV MONGO_DOWNLOAD_SHA256=6b650bdf62792fb44445edfee2100b9a8d861710348c8bbd3b93f56d11d5e7ea
# Wed, 13 Dec 2017 03:02:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 13 Dec 2017 03:02:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2017 03:02:46 GMT
EXPOSE 27017/tcp
# Wed, 13 Dec 2017 03:02:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baabcbaac6b1ea90ee37f64c65b56fbd5820d2830440bd97f25b389de1ac7ffa`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b2879821df58c2a8ee8a0c67d6dcc088e61115241cbcb844587a4b7ab39add`  
		Last Modified: Tue, 19 Dec 2017 04:09:07 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b6754af4adde273c46d7cf0fe3567e8abc00d305b4234221f04a2c0c391192`  
		Last Modified: Tue, 19 Dec 2017 04:09:05 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b967eaee48d3ada8b70cd927f3d58f3aa388bcdc3c3e867a734133a4edf73d6e`  
		Last Modified: Tue, 19 Dec 2017 04:09:22 GMT  
		Size: 67.7 MB (67674311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45dabd9cd2b6f531b7deb401ce402d18398f65a00bd85ab748d639b3a93e5936`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbea43d3b1a6a636e0d617e4bdf7a2006004a69f1a86dc2d858eda24c9ec165`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6cd6814fa168c62d43235366fa45ad34f22ea265954c30075a6845d7c4540f5`  
		Last Modified: Tue, 19 Dec 2017 04:09:04 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:c78f6debfb5b10fe2ed390105a729123f3365a33e5aada6f5539922d1d7c75dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:56210d12db53301f71b6f3d38c200c54d9e4722d4884605f6bb24876613efb2f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130387820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1200574c8af96f9b81952bb1131c4a3853fc5c789d73bc50d623d0c6915d1172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Thu, 28 Dec 2017 00:15:43 GMT
ENV MONGO_VERSION=3.6.1
# Thu, 28 Dec 2017 00:15:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 28 Dec 2017 00:16:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 28 Dec 2017 00:16:04 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 28 Dec 2017 00:16:04 GMT
VOLUME [/data/db /data/configdb]
# Thu, 28 Dec 2017 00:16:04 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Thu, 28 Dec 2017 00:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Dec 2017 00:16:05 GMT
EXPOSE 27017/tcp
# Thu, 28 Dec 2017 00:16:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6b165aa31730e9c9ebfe57bc966413905188436bb0c41eecfdef96a09f8c99`  
		Last Modified: Thu, 28 Dec 2017 00:22:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772467f0b4cd666887cd2c67701ce0c258d248a476e05f7d17f29fa678aeae3e`  
		Last Modified: Thu, 28 Dec 2017 00:22:54 GMT  
		Size: 97.1 MB (97051101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d919fbb860064f1964560410ef4dc361653cd42e224e696821cedaba52859`  
		Last Modified: Thu, 28 Dec 2017 00:22:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cad17917cd13144fca5224b3e31f5f26ff3f1b1b6269a1c580653e9db9608b`  
		Last Modified: Thu, 28 Dec 2017 00:22:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.1`

```console
$ docker pull mongo@sha256:c78f6debfb5b10fe2ed390105a729123f3365a33e5aada6f5539922d1d7c75dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.6.1` - linux; amd64

```console
$ docker pull mongo@sha256:56210d12db53301f71b6f3d38c200c54d9e4722d4884605f6bb24876613efb2f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130387820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1200574c8af96f9b81952bb1131c4a3853fc5c789d73bc50d623d0c6915d1172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Thu, 28 Dec 2017 00:15:43 GMT
ENV MONGO_VERSION=3.6.1
# Thu, 28 Dec 2017 00:15:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 28 Dec 2017 00:16:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 28 Dec 2017 00:16:04 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 28 Dec 2017 00:16:04 GMT
VOLUME [/data/db /data/configdb]
# Thu, 28 Dec 2017 00:16:04 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Thu, 28 Dec 2017 00:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Dec 2017 00:16:05 GMT
EXPOSE 27017/tcp
# Thu, 28 Dec 2017 00:16:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6b165aa31730e9c9ebfe57bc966413905188436bb0c41eecfdef96a09f8c99`  
		Last Modified: Thu, 28 Dec 2017 00:22:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772467f0b4cd666887cd2c67701ce0c258d248a476e05f7d17f29fa678aeae3e`  
		Last Modified: Thu, 28 Dec 2017 00:22:54 GMT  
		Size: 97.1 MB (97051101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d919fbb860064f1964560410ef4dc361653cd42e224e696821cedaba52859`  
		Last Modified: Thu, 28 Dec 2017 00:22:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cad17917cd13144fca5224b3e31f5f26ff3f1b1b6269a1c580653e9db9608b`  
		Last Modified: Thu, 28 Dec 2017 00:22:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.1` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.1` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.1-jessie`

```console
$ docker pull mongo@sha256:f734d0fbaecefa95e269f8902525a69151cd3626da88cafa5a277d623e4d7c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.6.1-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:56210d12db53301f71b6f3d38c200c54d9e4722d4884605f6bb24876613efb2f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130387820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1200574c8af96f9b81952bb1131c4a3853fc5c789d73bc50d623d0c6915d1172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Thu, 28 Dec 2017 00:15:43 GMT
ENV MONGO_VERSION=3.6.1
# Thu, 28 Dec 2017 00:15:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 28 Dec 2017 00:16:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 28 Dec 2017 00:16:04 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 28 Dec 2017 00:16:04 GMT
VOLUME [/data/db /data/configdb]
# Thu, 28 Dec 2017 00:16:04 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Thu, 28 Dec 2017 00:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Dec 2017 00:16:05 GMT
EXPOSE 27017/tcp
# Thu, 28 Dec 2017 00:16:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6b165aa31730e9c9ebfe57bc966413905188436bb0c41eecfdef96a09f8c99`  
		Last Modified: Thu, 28 Dec 2017 00:22:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772467f0b4cd666887cd2c67701ce0c258d248a476e05f7d17f29fa678aeae3e`  
		Last Modified: Thu, 28 Dec 2017 00:22:54 GMT  
		Size: 97.1 MB (97051101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d919fbb860064f1964560410ef4dc361653cd42e224e696821cedaba52859`  
		Last Modified: Thu, 28 Dec 2017 00:22:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cad17917cd13144fca5224b3e31f5f26ff3f1b1b6269a1c580653e9db9608b`  
		Last Modified: Thu, 28 Dec 2017 00:22:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.1-windowsservercore`

```console
$ docker pull mongo@sha256:7a433605bf77d114d6c5a2947398565baf45b545176c407fa00b63b8c8cb3dd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.6.1-windowsservercore` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.1-windowsservercore` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.1-windowsservercore-1709`

```console
$ docker pull mongo@sha256:511c3e95ac728c2b41b5886b99110c19fc20fa6a5d965033b0e2ea748fde8a8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.125; amd64

### `mongo:3.6.1-windowsservercore-1709` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.1-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:df1f2f6d3ea85e4830748919a0ea70268d79194f52296bd7245200abf7a4d3cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `mongo:3.6.1-windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-jessie`

```console
$ docker pull mongo@sha256:f734d0fbaecefa95e269f8902525a69151cd3626da88cafa5a277d623e4d7c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3.6-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:56210d12db53301f71b6f3d38c200c54d9e4722d4884605f6bb24876613efb2f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130387820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1200574c8af96f9b81952bb1131c4a3853fc5c789d73bc50d623d0c6915d1172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Thu, 28 Dec 2017 00:15:43 GMT
ENV MONGO_VERSION=3.6.1
# Thu, 28 Dec 2017 00:15:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 28 Dec 2017 00:16:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 28 Dec 2017 00:16:04 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 28 Dec 2017 00:16:04 GMT
VOLUME [/data/db /data/configdb]
# Thu, 28 Dec 2017 00:16:04 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Thu, 28 Dec 2017 00:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Dec 2017 00:16:05 GMT
EXPOSE 27017/tcp
# Thu, 28 Dec 2017 00:16:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6b165aa31730e9c9ebfe57bc966413905188436bb0c41eecfdef96a09f8c99`  
		Last Modified: Thu, 28 Dec 2017 00:22:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772467f0b4cd666887cd2c67701ce0c258d248a476e05f7d17f29fa678aeae3e`  
		Last Modified: Thu, 28 Dec 2017 00:22:54 GMT  
		Size: 97.1 MB (97051101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d919fbb860064f1964560410ef4dc361653cd42e224e696821cedaba52859`  
		Last Modified: Thu, 28 Dec 2017 00:22:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cad17917cd13144fca5224b3e31f5f26ff3f1b1b6269a1c580653e9db9608b`  
		Last Modified: Thu, 28 Dec 2017 00:22:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:7a433605bf77d114d6c5a2947398565baf45b545176c407fa00b63b8c8cb3dd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1709`

```console
$ docker pull mongo@sha256:511c3e95ac728c2b41b5886b99110c19fc20fa6a5d965033b0e2ea748fde8a8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.125; amd64

### `mongo:3.6-windowsservercore-1709` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:df1f2f6d3ea85e4830748919a0ea70268d79194f52296bd7245200abf7a4d3cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-jessie`

```console
$ docker pull mongo@sha256:f734d0fbaecefa95e269f8902525a69151cd3626da88cafa5a277d623e4d7c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:3-jessie` - linux; amd64

```console
$ docker pull mongo@sha256:56210d12db53301f71b6f3d38c200c54d9e4722d4884605f6bb24876613efb2f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130387820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1200574c8af96f9b81952bb1131c4a3853fc5c789d73bc50d623d0c6915d1172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Thu, 28 Dec 2017 00:15:43 GMT
ENV MONGO_VERSION=3.6.1
# Thu, 28 Dec 2017 00:15:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 28 Dec 2017 00:16:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 28 Dec 2017 00:16:04 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 28 Dec 2017 00:16:04 GMT
VOLUME [/data/db /data/configdb]
# Thu, 28 Dec 2017 00:16:04 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Thu, 28 Dec 2017 00:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Dec 2017 00:16:05 GMT
EXPOSE 27017/tcp
# Thu, 28 Dec 2017 00:16:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6b165aa31730e9c9ebfe57bc966413905188436bb0c41eecfdef96a09f8c99`  
		Last Modified: Thu, 28 Dec 2017 00:22:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772467f0b4cd666887cd2c67701ce0c258d248a476e05f7d17f29fa678aeae3e`  
		Last Modified: Thu, 28 Dec 2017 00:22:54 GMT  
		Size: 97.1 MB (97051101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d919fbb860064f1964560410ef4dc361653cd42e224e696821cedaba52859`  
		Last Modified: Thu, 28 Dec 2017 00:22:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cad17917cd13144fca5224b3e31f5f26ff3f1b1b6269a1c580653e9db9608b`  
		Last Modified: Thu, 28 Dec 2017 00:22:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:7a433605bf77d114d6c5a2947398565baf45b545176c407fa00b63b8c8cb3dd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:3-windowsservercore` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1709`

```console
$ docker pull mongo@sha256:511c3e95ac728c2b41b5886b99110c19fc20fa6a5d965033b0e2ea748fde8a8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.125; amd64

### `mongo:3-windowsservercore-1709` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:df1f2f6d3ea85e4830748919a0ea70268d79194f52296bd7245200abf7a4d3cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:jessie`

```console
$ docker pull mongo@sha256:f734d0fbaecefa95e269f8902525a69151cd3626da88cafa5a277d623e4d7c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `mongo:jessie` - linux; amd64

```console
$ docker pull mongo@sha256:56210d12db53301f71b6f3d38c200c54d9e4722d4884605f6bb24876613efb2f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130387820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1200574c8af96f9b81952bb1131c4a3853fc5c789d73bc50d623d0c6915d1172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Thu, 28 Dec 2017 00:15:43 GMT
ENV MONGO_VERSION=3.6.1
# Thu, 28 Dec 2017 00:15:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 28 Dec 2017 00:16:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 28 Dec 2017 00:16:04 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 28 Dec 2017 00:16:04 GMT
VOLUME [/data/db /data/configdb]
# Thu, 28 Dec 2017 00:16:04 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Thu, 28 Dec 2017 00:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Dec 2017 00:16:05 GMT
EXPOSE 27017/tcp
# Thu, 28 Dec 2017 00:16:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6b165aa31730e9c9ebfe57bc966413905188436bb0c41eecfdef96a09f8c99`  
		Last Modified: Thu, 28 Dec 2017 00:22:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772467f0b4cd666887cd2c67701ce0c258d248a476e05f7d17f29fa678aeae3e`  
		Last Modified: Thu, 28 Dec 2017 00:22:54 GMT  
		Size: 97.1 MB (97051101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d919fbb860064f1964560410ef4dc361653cd42e224e696821cedaba52859`  
		Last Modified: Thu, 28 Dec 2017 00:22:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cad17917cd13144fca5224b3e31f5f26ff3f1b1b6269a1c580653e9db9608b`  
		Last Modified: Thu, 28 Dec 2017 00:22:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:c78f6debfb5b10fe2ed390105a729123f3365a33e5aada6f5539922d1d7c75dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:56210d12db53301f71b6f3d38c200c54d9e4722d4884605f6bb24876613efb2f
```

-	Docker Version: 17.06.2-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130387820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1200574c8af96f9b81952bb1131c4a3853fc5c789d73bc50d623d0c6915d1172`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 12 Dec 2017 01:41:34 GMT
ADD file:e7ac45803c3ab9b7023933b75f5a88eda1f3edca97c7e462401860777cf312f7 in / 
# Tue, 12 Dec 2017 01:41:35 GMT
CMD ["bash"]
# Tue, 12 Dec 2017 02:36:34 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Tue, 12 Dec 2017 02:38:45 GMT
RUN apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	&& rm -rf /var/lib/apt/lists/*
# Thu, 21 Dec 2017 01:16:42 GMT
ENV GOSU_VERSION=1.10
# Thu, 21 Dec 2017 01:16:42 GMT
ENV JSYAML_VERSION=3.10.0
# Thu, 21 Dec 2017 01:17:01 GMT
RUN set -ex; 		apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --keyserver ha.pool.sks-keyservers.net --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-get purge -y --auto-remove wget
# Thu, 21 Dec 2017 01:17:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 21 Dec 2017 01:21:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 21 Dec 2017 01:21:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 21 Dec 2017 01:21:17 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 21 Dec 2017 01:21:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 21 Dec 2017 01:21:18 GMT
ENV MONGO_MAJOR=3.6
# Thu, 28 Dec 2017 00:15:43 GMT
ENV MONGO_VERSION=3.6.1
# Thu, 28 Dec 2017 00:15:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/debian jessie/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR main" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 28 Dec 2017 00:16:03 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 28 Dec 2017 00:16:04 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 28 Dec 2017 00:16:04 GMT
VOLUME [/data/db /data/configdb]
# Thu, 28 Dec 2017 00:16:04 GMT
COPY file:18c5d9b642a89adf49e037d95a9e7de6b60557c77e049c9652605cf9cba57df9 in /usr/local/bin/ 
# Thu, 28 Dec 2017 00:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Dec 2017 00:16:05 GMT
EXPOSE 27017/tcp
# Thu, 28 Dec 2017 00:16:05 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:c4bb02b17bb4b034c95a948c99c762cf0486a45f45441a052208d7750f1b413b`  
		Last Modified: Tue, 12 Dec 2017 01:48:52 GMT  
		Size: 30.1 MB (30114519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f58e3bb3be4bfc57e890138990e250f521d69af3a0c39c7d0394727c66dc676`  
		Last Modified: Tue, 12 Dec 2017 02:41:52 GMT  
		Size: 2.1 KB (2087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a229fb575a6e558f699a74bc9037d818b6d74c607e68ef6cf1c548daf10ebc52`  
		Last Modified: Tue, 12 Dec 2017 02:42:30 GMT  
		Size: 2.4 MB (2397783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5ddc533743964c2e280d7a7e70667e892c29b518c04ee34aa56aa9449b59da`  
		Last Modified: Thu, 21 Dec 2017 01:23:21 GMT  
		Size: 816.7 KB (816688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9d2af6e2069f3050614a5f983f7147427a7f4e907c67bbb070e346ab333ed5`  
		Last Modified: Thu, 21 Dec 2017 01:23:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6c28c0235b619029c8b8c9d512f97756a986bfa458e64b5aa45784af894ac3`  
		Last Modified: Thu, 21 Dec 2017 01:24:43 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6b165aa31730e9c9ebfe57bc966413905188436bb0c41eecfdef96a09f8c99`  
		Last Modified: Thu, 28 Dec 2017 00:22:36 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772467f0b4cd666887cd2c67701ce0c258d248a476e05f7d17f29fa678aeae3e`  
		Last Modified: Thu, 28 Dec 2017 00:22:54 GMT  
		Size: 97.1 MB (97051101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d919fbb860064f1964560410ef4dc361653cd42e224e696821cedaba52859`  
		Last Modified: Thu, 28 Dec 2017 00:22:38 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cad17917cd13144fca5224b3e31f5f26ff3f1b1b6269a1c580653e9db9608b`  
		Last Modified: Thu, 28 Dec 2017 00:22:37 GMT  
		Size: 3.7 KB (3718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:7a433605bf77d114d6c5a2947398565baf45b545176c407fa00b63b8c8cb3dd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64
	-	windows version 10.0.16299.125; amd64

### `mongo:windowsservercore` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1709`

```console
$ docker pull mongo@sha256:511c3e95ac728c2b41b5886b99110c19fc20fa6a5d965033b0e2ea748fde8a8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.16299.125; amd64

### `mongo:windowsservercore-1709` - windows version 10.0.16299.125; amd64

```console
$ docker pull mongo@sha256:d89e786e6fd181804336ab6c0b6e1f87e6c96858d9a46c8493a18b921498b94e
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 GB (3338494894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a52b013210e6623ff35456dc66d228c8a3a17c23fbabb5b507192f82ff784c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 29 Sep 2017 14:43:28 GMT
RUN Apply image 10.0.16299.15
# Sat, 09 Dec 2017 18:00:03 GMT
RUN Install update 10.0.16299.125
# Wed, 13 Dec 2017 02:53:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 01:26:57 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 01:26:58 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 01:26:59 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:40:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:40:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:40:36 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:40:37 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:5847a47b8593f7c39aa5e3db09e50b76d42aa8898c0440c70cc9c69747d4c479`  
		Last Modified: Tue, 17 Oct 2017 15:51:05 GMT  
		Size: 2.3 GB (2274300585 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e50cc21fbc56936f06a5d9dfe4559b7108a89064fcb39dfbe14150d5cfeb912b`  
		Last Modified: Mon, 11 Dec 2017 22:06:21 GMT  
		Size: 589.5 MB (589524514 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a768329167a641833bde82301c06d629170e446fe0d207a2fe4a55c0a7aeb6ac`  
		Last Modified: Tue, 19 Dec 2017 04:07:42 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e3bb4b9749c84007c7810c65240f8106ba9608f199a7e485e3ba2d21a7a864`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0697d468897e9e6d6bfbe41501d2de9b645a46eab2a4dec083748d5730f6eb3`  
		Last Modified: Fri, 29 Dec 2017 01:42:24 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2490784db3cb2b59d48ca3176511804c2a85b36d7c9bc793a94eb23c9027dec`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b365c0cf397768a4bf7aac72bb76a6dfc29449089a4fe4b0fca2cef80a70689a`  
		Last Modified: Fri, 29 Dec 2017 01:43:12 GMT  
		Size: 474.7 MB (474661422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79f395b54d7591d7b11fc73904a05bc00129fcaa0ab30d6d9fc5efe95fbf38b`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013616d6f38ceab757949e1069006e4895ee0bf317e30970529ab93eb2e1cfe6`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d39a64fef9b2dca3963911767ef3b25812e5b42ff9f66a1cb15b1b540d43ea`  
		Last Modified: Fri, 29 Dec 2017 01:42:22 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:df1f2f6d3ea85e4830748919a0ea70268d79194f52296bd7245200abf7a4d3cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull mongo@sha256:3a9345a8268c7fb01a145e0e2477d8723c24f26383ffa728bba17fc836ae9914
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5836956052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a77765337380bb8b7086a133a9df23c5ea32c972b31ae3bbb44e1df1e18eec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Wed, 13 Dec 2017 02:43:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 29 Dec 2017 00:56:09 GMT
ENV MONGO_VERSION=3.6.1
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_URL=http://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.1-signed.msi
# Fri, 29 Dec 2017 00:56:10 GMT
ENV MONGO_DOWNLOAD_SHA256=ff04f71216c93de9d96735cece828be5c48478d9b92519f647152ba7f17494de
# Fri, 29 Dec 2017 01:26:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 29 Dec 2017 01:26:43 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 29 Dec 2017 01:26:46 GMT
EXPOSE 27017/tcp
# Fri, 29 Dec 2017 01:26:48 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 13 Dec 2016 10:53:31 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3725c17d990aca553df2f531b536a72c07f2781fcbb60b01a557e3666808dda2`  
		Last Modified: Mon, 11 Dec 2017 21:43:15 GMT  
		Size: 1.3 GB (1291829199 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c29de164cfa4c6f227e7f0a8df3325f748ead8e6293c8f40db2bdc289e3a94d9`  
		Last Modified: Tue, 19 Dec 2017 04:07:11 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7089526b167439127c14e9c504c0fff40f08905bd84680ed04054ab9004fe729`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46871ac23fa560cdb922d43d1352e8e2e3ac0d6bb62fed8b0447ba441b506c70`  
		Last Modified: Fri, 29 Dec 2017 01:41:07 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f15b49c2c0bb9bc31247ac927a2aa1475d647444e1ab2a88fa01d5ee804a67`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe26687608cd705811ce9b5874024082a4ec76314c48f389ac372695ef09af6a`  
		Last Modified: Fri, 29 Dec 2017 01:41:58 GMT  
		Size: 475.1 MB (475132603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6741cc54d376ea2838cc5853c0eb0739d9d1e05c1346aad29bc9cc666ef67f`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528989e591fd649b081bd74aec092a9a894314b41b0d1b81f85926694f53460e`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20273f474dc39cb1fd684fa537e37f86129f99f94e0e756be474abc54058c757`  
		Last Modified: Fri, 29 Dec 2017 01:41:05 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
