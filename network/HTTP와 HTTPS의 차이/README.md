## 📝 HTTP와 HTTPS의 차이

<br>

**🔍 HTTP(HyperText Transfer Protocol)**

* 서버/클라이언트 모델을 따라 데이터를 주고 받기 위한 애플리케이션 계층 프로토콜
* 80번 포트를 기본적으로 사용
* 상태를 가지지 않는 Stateless 프로토콜
* Method, Path, Version, Headers, Body 등으로 구성

<br>

> 🤔 **프로토콜?**
>
> 컴퓨터 내부 또는 컴퓨터 사이에 데이터 교환 방식을 정의하는 규칙 체계

<br>

**❌ HTTP의 단점**

* 암호화가 되지 않은 평문 데이터를 전송하는 프로토콜

<br>

‼️ **비밀번호처럼 중요한 정보를 주고 받으면 제 3자가 정보를 조회할 수 있어 보안에 취약하다!**

<br>

---

<br>

**🔍 HTTPS(HyperText Transfer Protocol Secure)**

* HTTP에 데이터 암호화가 추가된 프로토콜
* 443번 포트를 기본적으로 사용

<br>

**⚙️ HTTPS의 동작 과정**

1. 클라이언트가 서버로 최초 연결 시도
   
2. 서버는 공개키(인증서)를 브라우저에게 전달
   
3. 브라우저는 인증서의 유효성을 검사하고 세션키 발급
   
4. 브라우저는 세션키를 보관하며 추가로 서버의 공개로 세션키를 암호화하여 서버로 전송
   
5. 서버는 개인키로 암호화된 세션키를 복호화하여 세션키 획득
   
6. 클라이언트와 서버는 동일한 세션키를 공유하므로 데이터를 전달할 때 세션키로 암/복호화를 진행

<br><br>

![HTTPS의 동작 과정](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcCodLU%2FbtrqRZnoOFq%2Fe6kFHjADoVby70466Jkq51%2Fimg.png)
<p align="center">(출처: https://mangkyu.tistory.com/98)</p>
