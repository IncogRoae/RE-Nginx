## Init Nginx Web Server

[공식 문서](https://nginx.org/en/linux_packages.html#Ubuntu)를 참고하여 Nginx Web Server를 구성합니다.

### Package 구성

설치된 패키지는 아래와 같습니다.
- curl: HTTP를 통해 데이터를 전송하거나 다운로드하는 도구입니다.
- gnupg2: GPG 서명 검증에 사용되는 암호화 도구입니다.
- ca-certificates: SSL/TLS 연결을 위한 신뢰할 수 있는 인증 기관(CA)의 인증서를 관리합니다.
- lsb-release: 배포판 정보를 제공하는 도구입니다.
- ubuntu-keyring: Ubuntu의 공식 GPG 키를 관리하여 소프트웨어의 신뢰성을 검증하는 데 사용됩니다.
- libpcre3: 정규 표현식 처리 기능을 제공하는 PCRE 라이브러리입니다.

### Inventory 구성
- webserver1: 서버가 배포되는 인스턴스 입니다.
- webserver2: Blue/Green 배포시 사용되는 서버입니다.
- loadbalancer
