## http/https에서 browser가 caching 하지 않게 하는 http header

로그인용 사용자 이름, 비밀번호 및 기타 민감한 정보들을 보호하기 위해 SSL을 로그인 페이지나 회원 정보 페이지등은 SSL로 암호화 하는 경우가 많다.

SSL을 사용해서 민감한 정보들을 보호한다고 해도 브라우저에 이 정보가 캐싱되면 문제가 발생할 수 있다.(PC방이나 공공장소에서 사용 후 캐슁으로 인해 개인정보가 남는 등...)

다음 http header를 사용하면 브라우저 캐싱을 방지할 수 있다. 단 캐싱을 하지 않으면 성능 저하가 발생할 수 있으므로 로그인 페이지 등에 제한적으로 사용을 권장한다.


### HTTP 1.1
```java
Cache-Control: no-cache, no-store, must-revalidate
```

### HTTP 1.0
```java
Pragma: no-cache
```

### Proxy
```java
Expires: 0
```

## PHP
```php
header('Cache-Control: no-cache, no-store, must-revalidate'); // HTTP 1.1
header('Pragma: no-cache') // HTTP 1.0
header('Expires: 0') // Proxies
```

## Java Servelt
```java
response.setHeader("Cache-Control", "no-cache, no-store, must-revalidate"); // HTTP 1.1
response.setHeader("Pragma", "no-cache"); // HTTP 1.0
response.setHeader("Expires", 0); // Proxies
```