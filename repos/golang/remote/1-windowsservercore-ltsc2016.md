## `golang:1-windowsservercore-ltsc2016`

```console
$ docker pull golang@sha256:4baaf3a81f3cdd902ad1f0e9d8fa98a129bb02a28fc297080540500115d54f34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `golang:1-windowsservercore-ltsc2016` - windows version 10.0.14393.1944; amd64

```console
$ docker pull golang@sha256:7ed39a103598c313c35a28891c0b5477e4a3dbe7d1c90c9a22866d04271c0551
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 GB (5510734408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fdcf0b6413be0035d27e587039e76736b5b882ca07f32fd15aee4a24460ddb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Tue, 13 Dec 2016 10:53:31 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:43:15 GMT
RUN Install update 10.0.14393.1944
# Thu, 14 Dec 2017 00:34:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Dec 2017 00:34:00 GMT
ENV GIT_VERSION=2.11.1
# Thu, 14 Dec 2017 00:34:01 GMT
ENV GIT_TAG=v2.11.1.windows.1
# Thu, 14 Dec 2017 00:34:02 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.11.1.windows.1/MinGit-2.11.1-64-bit.zip
# Thu, 14 Dec 2017 00:34:03 GMT
ENV GIT_DOWNLOAD_SHA256=668d16a799dd721ed126cc91bed49eb2c072ba1b25b50048280a4e2c5ed56e59
# Thu, 14 Dec 2017 00:36:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  git --version'; git --version; 		Write-Host 'Complete.';
# Thu, 14 Dec 2017 00:36:16 GMT
ENV GOPATH=C:\gopath
# Thu, 14 Dec 2017 00:37:27 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 14 Dec 2017 01:27:30 GMT
ENV GOLANG_VERSION=1.9.2
# Thu, 14 Dec 2017 01:34:12 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '682ec3626a9c45b657c2456e35cadad119057408d37f334c6c24d88389c2164c'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Thu, 14 Dec 2017 01:34:14 GMT
WORKDIR C:\gopath
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
	-	`sha256:a3d5f61b176f33e17d386e2d798dc5fcf5b313841fcbf7e3b51cd9c892c4fa9d`  
		Last Modified: Thu, 14 Dec 2017 01:59:07 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabfd4a1d78aa04f5b8f793e2337babee92a3e2fbf9698a7bde819386a87443d`  
		Last Modified: Thu, 14 Dec 2017 01:59:06 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac7459dae3268ef6030a9ce1de519aeff528930bb5a1d727572cac7c0f0a9ce`  
		Last Modified: Thu, 14 Dec 2017 01:59:05 GMT  
		Size: 1.1 KB (1077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba15213d04646108885deb8321df61e7f8170554027a7f25da95444ca425808`  
		Last Modified: Thu, 14 Dec 2017 01:59:02 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071931363cb2c646896130aebb51cb4c973df128900d018405b32b7ce18ded00`  
		Last Modified: Thu, 14 Dec 2017 01:59:02 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d89fe67196eed515930805e54391a024df10eaaba54ca7c55f223eea555244f`  
		Last Modified: Thu, 14 Dec 2017 01:59:19 GMT  
		Size: 29.3 MB (29276801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581204f6ebd7ede573fac6c6e814b6fa48ae1c6d6e1f05fd864e91b01524c418`  
		Last Modified: Thu, 14 Dec 2017 01:59:00 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d483800fff05a932e1af0d6526758b79e00f1bd7bc30324edef7feb26143ecfd`  
		Last Modified: Thu, 14 Dec 2017 01:59:01 GMT  
		Size: 4.8 MB (4805320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74003b47a238d6496ffd4ba866a255c1bcff60329e429bb8518b526016c95896`  
		Last Modified: Thu, 14 Dec 2017 02:09:06 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6219bbce92c221c4e691968dfda8d848357eaaaae16ee6832cb791e9348f8f`  
		Last Modified: Thu, 14 Dec 2017 02:10:04 GMT  
		Size: 114.8 MB (114827617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84595ef06cf64711dae26fa9346d3a33623181163edabdd70c5ff4fe36774224`  
		Last Modified: Thu, 14 Dec 2017 02:09:06 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
