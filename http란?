![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/757d4617-8577-428d-95b6-cb4d841d3efc/Untitled.png)

A하고 B가 있다고 가정해보자.

A는 B에게 Stream으로 연결한 후, 데이터를 요청하게 될 것이고, 그 후 B는 A에게 그에 맞는 응답을 할 것이다. 이것이 Http 통신의 기본적인 구조이다.

예를 들면 A(=Client)는 배고픈 자, B(=Server)는 음식을 가지고 있는 자

---

### **Http 란?**

> http는 HTML 문서와 같은 리소스들을 가져올 수 있도록 해주는 [프로토콜](https://www.notion.so/c5cd61f5e0524e51a2f7dc45ef077e32)
> 
- 웹에서 이루는 모든 데이터 교환의 기초
- 클라이언트-서버 간의 프로토콜
- 클라이언트와 서버들은 스트림을 이용해 개별적인 메시지 교환에 의해 통신한다.
- 클라이언트 → 서버 : 전송되는 메시지 ⇒ 요청(Request)
- 서버 → 클라이언트 : 응답으로 전송되는 메시지 ⇒ 응답(Response)

---

http 통신에는 약속이 필요한데, http 1.1 기준에서는 수많은 약속이 존재한다.

이 중에서 대표적인 통신방법 4가지가 있는데,

### **Get**

- 데이터를 줘! (**Select**, 데이터를 달라고 할 때 요청)

### Post

- 데이터를 추가해줘! (**Insert**, 한건 또는 N건)
- 예를 들어, 회원가입을 할 때, 웹브라우저에 나의 정보를 적게 될 것이다. 그러므로 Naver 나 Daum 같은 웹브라우저가 통신을 통해서 나의 개인정보를 갖게 된다. 요청의 방법을 통해서(아이디, 패스워드, 성별, 주소 등) 던져주고 난 뒤, 서버는 해당 정보들을 추가한 뒤, 데이터에 Mapping 하게 되는데, Insert를 요청하는 것과 동일하다.

### Put

- 데이터를 수정해줘! (**Update**)
- 예를 들어, post 방식을 통해 회원가입을 하게 되었는데, 만약 내 주소가 잘못되었다고 가정하자. 이 때 put 방식을 통해 update 문을 이용한다.

### Delete

- 데이터를 삭제해줘! (**Delete**)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c418bbe4-2ddc-44b3-8b10-781f15d449f7/Untitled.png)

✨✨여기서 중요✨✨

클라이언트에서 서버로 어떤 정보를 요청 할 때 ***무슨 정보를 요청하는 것인지 어떻게 아는 것인가?***

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/001c6343-22ff-4a0d-affe-3d245a520f9a/Untitled.png)

이 때, 클라이언트가 요청하는 동시에 그에 해당하는 ***추가적인 정보***도 던질 수 있다!

그러기 위해서는 [MINE](https://www.notion.so/MINE-500726a722424272a827b2dfb80465df) 타입이라는 존재도 알아야 한다.

---

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b9d5b75f-7fb8-45aa-849a-5076efdd18fa/Untitled.png)

### 포트란 무엇인가?

> 네트워크 상에서 통신하기 위해서 호스트 내부적으로 프로세스가 할당받아야 하는 고유한 숫자
> 

- 포트는 통신을 할 때 특정 서비스를 이용하기 위한 연결고리
- 예를 들어, A와 B가 각자 80번 포트로 지정 했을 경우, 서비스 이용가능
- 만약 A가 80번, B가 81번 포트 설정할 경우, 통신 불가능

### 소켓은 무엇인가?

> 프로세스가 드넓은 네트워크 세계로 데이터를 내보내거나 혹은 그 세계로부터 데이터를 받기 위한 실제적인 창구 역할을 한다.
> 

- 소켓은 포트와 매우 연관성이 있는데, 네이버로 예를 들어보자.
- 네이버는 대표적인 사이트인 만큼 이용자 수도 엄청나게 많다. 그만큼 통신도 많이 이뤄지고 있다. 다수의 이용자들이 뉴스를 보려고 클릭을 하게 될 때, 한 사람씩 볼 수 있게 제한을 두게 된다면 어떻게 될까?
- 그러면 네이버는 서비스 운영을 못하게 될 것이다. 1초에 1명씩 처리 한다면 100번째 이용자는 100초 후에 처리가 될 것이다.
- 이러한 불편함을 소켓이 해소해 준다. 처리할 수 있는 곳이 한 곳이 아닌 여러개를 지정해서 동시에 여러 작업들을 처리해 주는 것

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9bb08209-c9cf-4a53-aede-d94fdac390b8/Untitled.png)

A와 B는 포트로 인해 통신이 된 상태이다.

만약 B가 C와 D라는 사람과 통신하고 싶을 때, C, D에 포트를 달아서 B와 연결하게 된다.

이런 상황에서 B는 동시에 A, C, D를 통신하므로 굉장히 힘들 것이다.  

 ⇒ **Stateful** 방식(= **연결이 지속된 상태**, 주로 채팅에서 쓰인다)

### Stateful 방식이란 무엇인가?

> 요청한 후 선을 계속 유지하는 방식
> 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3800e8de-1d34-4776-87ff-53fdcf4cd572/Untitled.png)

- 이러한 과정에서 A와 B사이에 **Session**이 생성되었다!
- 섹션이 생성되었다는 것은 **데이터를 응답할 준비가 되었다는 것!(인증)** ⇒ 근거로 인해 인증이 되었기 때문에 A와 B는 데이터를 마구 주고 받을 수 있다.

---

그러나, HTTP 방식은 Stateless 방식을 사용한다.

### Statelsee 방식이란 무엇인가?

> 요청 할 때마다 Stream(선)을 연결해서 데이터를 주고 받은 뒤 연결을 끊는 방식
> 

클라이언트인 A가 있고, 서버인 B가 있다고 가정해보자.

A가 B에게 get 방식으로 요청을 한 뒤, B는 A에게 그에 맞는 응답을 할 것이다. 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4e8c2347-2486-47a4-8d1b-593ab6314e55/Untitled.png)

***그 후에는 연결을 끊어버린다!***

그러므로 http 는 한번 인증을 하고 난 뒤, 연결을 끊기 때문에 동일한 클라이언트가 새로 요청을 했음에도 불구하고 서버입장에서는 보장이 안된다. 

🤔 이러한 경우에는 어떤식으로 인증이 진행되는가? 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d4f0d94d-7edf-4bce-9e7d-76410cf109ac/Untitled.png)

## HTTP의 구조

1. 헤더 : HTTP 헤더는 HTTP 본문(=Body) 의 요청/응답에 관한 정보를 포함한다.
    1. 일반 헤더(General Header)
    2. 요청/응답 헤더(Request/Response Header)
    3. 엔터티 헤더(Entity Header)
2. 본문 : 실제 데이터, 요청한 리소스에 따라 HTML, 이미지, CSS 스타일 시트, JavaScript 파일이 포함 될 수 있다.

## HTTP 통신

### 서킷 스위칭(Circuit-Switching)

> 서킷이라는 연결을 두 장비간 사이에 만들어서 통신에 사용
> 
- ex, 전화 시스템 → 속도와 성능이 일정

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/836b6485-7fc2-40ef-b223-5e7d3b3241f6/Untitled.png)

가, 나, 다, 라 라는 데이터가 있는데 이 데이터들을 한번에 실어서 전송한다.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9acb6063-7496-463f-a3c8-75b2669c0035/Untitled.png)

단점은 선이 추가적으로 생성되는 것이 서킷 스위치 방식인데, 속도가 빠른 반면에 물리적으로 선이 계속 연결되어야 하기 때문에 비용이 상승한다.

### 패킷 스위칭(Packet-Switching)

> 데이터를 패킷(Packet)이라는 단위로 분할하여 전송
> 
- ex, IP

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/70d79253-c50a-42c9-b224-d0508f9b9535/Untitled.png)

가, 나, 다, 라 같은 다수의 데이터를 보낼 때 각각 쪼개는데 한 조각을 패킷이라고 한다.

또한 C가 B에게 데이터를 전송 할 때, 선이 새로 생성 되는 것이 아니라 A의 선과 공유하는 형태로 전송된다.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/66da013f-6770-4073-bd2f-6a5d2cba0f83/Untitled.png)

🤔이러한 경우 A의 데이터와 C의 데이터가 섞이게 되는데 B는 어떤식으로 데이터들을 구분할까?

실제로 통신은 단순하지 않으므로 굉장히 복잡한 형태로 왔다갔다 할 것이다.

경로가 다양하고, 교통의 혼잡이 가장 적은 경로를 선택해 데이터가 전송하게 된다.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/bce19e09-593d-440a-ac85-5c7effb140f3/Untitled.png)

만약 A의 가와 라 데이터가 전송 될 때, 실제로 경로가 다를 수 있다. 전송 순서에 따르면 A가 먼저 전송됐는데 라가 먼저 도착한 경우 서버가 조립시에 문제가 발생한다.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e9cc6442-e732-4c27-8ba4-5fc340addf7d/Untitled.png)

그러므로 **모든 패킷에는 헤더가 붙어서(데이터 순서, 출처 등) 함께 전송**된다.

<aside>
💡 **통신 할 때는 반드시 헤더와 바디가 필요하다!**

</aside>

---

<aside>
💡 내가 보낼 데이터가 이미지 뿐만 아니라 다른 타입의 데이터가 있다면?

</aside>

이 때, [MINE](https://www.notion.so/MINE-500726a722424272a827b2dfb80465df) 타입을 사용해 데이터를 전송할 수 있다.

1. Text
2. image
3. avi
4. 이진데이터
5. JSON

바디에 실어서 보낼 데이터가 무슨 데이터인지 헤더에 적을 때 마음대로 작성 할 수 없다. 그래서 MINE 에서 설정할 수 있다.
