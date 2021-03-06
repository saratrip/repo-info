## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:238db25b1f2e91dcc0976bc4d330b0760e706e2961c68d6add5010dc852b416e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.1944; amd64

### `golang:1-nanoserver` - windows version 10.0.14393.1944; amd64

```console
$ docker pull golang@sha256:508f474e3e7bd48ec079fcb3dda5c872493c480ef7d7524fd22ef3c18f410f06
```

-	Docker Version: 17.06.1-ee-2
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **505.8 MB (505801828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea2cbf503109ced366497e40af0c41d5d7f57969872540b1d36f502c295a8105`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Tue, 13 Dec 2016 10:47:17 GMT
RUN Apply image 10.0.14393.0
# Mon, 11 Dec 2017 21:42:41 GMT
RUN Install update 10.0.14393.1944
# Thu, 14 Dec 2017 01:18:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Dec 2017 01:18:45 GMT
ENV GOPATH=C:\gopath
# Thu, 14 Dec 2017 01:19:51 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath;
# Thu, 14 Dec 2017 01:39:30 GMT
ENV GOLANG_VERSION=1.9.2
# Thu, 14 Dec 2017 01:43:49 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '682ec3626a9c45b657c2456e35cadad119057408d37f334c6c24d88389c2164c'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Complete.';
# Thu, 14 Dec 2017 01:43:51 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:bce2fbc256ea437a87dadac2f69aabd25bed4f56255549090056c1131fad0277`  
		Last Modified: Tue, 13 Dec 2016 10:47:17 GMT  
		Size: 252.7 MB (252691002 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4806a44e00a0febaf206c2414777a070782c559757658199cf5e0d8f0ead2bba`  
		Last Modified: Mon, 11 Dec 2017 21:42:41 GMT  
		Size: 146.0 MB (146023673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a60e8bffbe40bfe08d89397474add53072023b6b9ed318db036dd0b8d0c5ff16`  
		Last Modified: Thu, 14 Dec 2017 02:06:00 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790dd7636ad5f40635dc2d101ad76a613a9d87e453bd33e130610afc3dc4ad74`  
		Last Modified: Thu, 14 Dec 2017 02:05:56 GMT  
		Size: 934.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46622a39a737717895806efee92e02f8dab84f6724681f8d91f8500906684fe`  
		Last Modified: Thu, 14 Dec 2017 02:05:57 GMT  
		Size: 837.9 KB (837859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfa4594787403cd0d314421d441c12ac5469acda210b701e027a243b462e602`  
		Last Modified: Thu, 14 Dec 2017 02:11:08 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9819920a60a156a7f681257a1a8cfbd974e9b57e81c232ee7ec6bf0d917a29ce`  
		Last Modified: Thu, 14 Dec 2017 02:11:31 GMT  
		Size: 106.2 MB (106245364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041ab7e30d16387dfd85a4dd9e8a8831edafa11421cc924a8c8a0955061c5c58`  
		Last Modified: Thu, 14 Dec 2017 02:11:10 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
