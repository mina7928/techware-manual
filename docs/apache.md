# Apache 2.4

## 아파치 시작하기

CentOS 기준으로 작성함

### 선행 설치

* PCRE
  ```sh
  yum install -y pcre-devel
  ```
* expat
  ```sh
  yum install -y expat-devel & export LD_LIBRARY_PATH
  ```
* zlib
  ```sh
  yum install -y zlib-devel
  ```

### Apache 설치

설치파일 다운로드
* HTTPD: [https://dlcdn.apache.org/httpd/httpd-2.4.54.tar.gz](https://dlcdn.apache.org/httpd/httpd-2.4.54.tar.gz)
* APR: https://dlcdn.apache.org/apr/apr-1.7.0.tar.gz
* APR-Util: https://dlcdn.apache.org/apr/apr-util-1.6.1.tar.gz

컴파일 & 설치
```sh
 ./configure
 make
 make install
```

## 설정

#### HTTP

$PREFIX/config/httpd.conf
- Listen
- Port
- DocumentRoot

```shell
curl localhost
```

#### HTTPS (SSL 인증서)
PassPhrase

#### 가상호스트 (VirtualHost)

#### 로깅
에러 로그
액세스 로그

#### 리다이렉트
rewrite
redirect
proxy

#### Tomcat 연동

##### mod_jk
mod_jk download
mod_jk make install
mod_jk.so
workers.properties
urimap.properties
mod_jk.log
mod_jk.conf

##### mod_proxy

#### Django 연동
##### mod_wsgi
##### mod_??
##### mod_??


#### 프록시
##### mod_proxy
##### mod_ws??


## 아파치 운영 관리

#### 아파치 버전 업그레이드 방법

#### 모니터링

#### 보안 취약점 조치

#### SSL 오프로딩 (SSL Offloading)

<ul class="footer_nav">
    {%- if prev %}
      <li class="prev">
        Previous topic: <a href="{{ prev.link|e }}">{{ prev.title }}</a>
      </li>
    {%- endif %}

    {%- if next %}
      <li class="next">
        Next topic: <a href="{{ next.link|e }}">{{ next.title }}</a>
      </li>
    {%- endif %}
</ul>
