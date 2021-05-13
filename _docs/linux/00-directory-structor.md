---
title: "리눅스 디렉토리 구조"
permalink: /docs/linux/directory-structor/
excerpt: "https://www.thegeekstuff.com/2010/09/linux-file-system-structure/"
last_modified_at: 2021-05-13
redirect_from:
  - /theme-setup/
toc: true
---

위치 | 설명
:---|:---
`/` | 최상위 디렉토리 <br> 모든 파일과 디렉토리는 이곳에서 시작된다.
/bin | 이진파일(실행파일) <br> 시스템의 모든 사용자가 사용하는 명령이 있다. <br> 기본적인 명령어가 저장된 디렉토리 <br> mv, cp, rm 등이 존재함
/sbin | 시스템 이진파일(실행파일) <br> 시스템 유지 관리 목적의 명령이 있다. <br> iptables, reboot, ifconfig, fdish
/etc | 설정파일이 존재
/dev | 시스템에 연결된 모든 장치가 포함됨 <br> 물리적 장치가 파일화되어 저장
/proc | 시스템 프로세스에 대한 정보가 저장되어 있다. <br> 시스템 리소스에 대한 텍스트 정보가 있는 가상 파일 시스템
/var | 변수 파일을 나타낸다 <br> 증가 할 것으로 예상되는 파일의 내용은 이곳에서 찾을 수 있다. (log, db, tmp, lock 등)
/tmp | 임시파일 <br> 시스템이 재부팅 될 때 삭제된다
/usr | 일반 사용자들이 사용하는 디렉토리 <br> bin, sbin, lib, local 등이 하위에 존재
/home | 사용자들의 홈디렉토리가 있는 곳 <br> 사용자를 추가하면 동일한 사용자 id로 디렉토리가 생성
/boot | 리눅스의 부트로더(Boot loader)가 있는 디렉토리
/lib | /bin 및 /sbin 아래에 있는 바이너리를 지원하는 라이브러리 파일을 저장
/opt | 응용프로그램 패키지 설치 장소 <br> 패키지 매니저가 자체적으로 설치/삭제를 수행함
/mnt | 시스템 관리자가 파일 시스템을 마운트 할 수있는 임시 마운트 디렉토리
/media | DVD, CD-ROME, USB 등의 탈부착 가능한 장치들의 임시 마운트 디렉토리
/srv | 서버 특정 서비스 관련 데이터를 포함
/root | 관리자계정 root 사용자의 홈 디렉토리
