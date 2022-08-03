######
Apache
######

****
설치
****

^^^^^^^^
선행 설치
^^^^^^^^

* PCRE: ``yum install -y pcre-devel``
* expat ``yum install -y expat-devel & export LD_LIBRARY_PATH``
* zlib: ``yum install -y zlib-devel``

^^^^^^^^^^^
Apache 설치
^^^^^^^^^^^

설치파일 다운로드
* HTTPD: https://dlcdn.apache.org/httpd/httpd-2.4.54.tar.gz
* APR: https://dlcdn.apache.org/apr/apr-1.7.0.tar.gz
* APR-Util: https://dlcdn.apache.org/apr/apr-util-1.6.1.tar.gz

컴파일 & 설치::

 ./configure
 make
 make install




+----+----+
|아아|ㅁㅁ|
+----+----+

^^^^
설정
^^^^

