---
title: 인터넷
permalink: internet.html
sidebar: generic
tags: [Front-End]
product: Generic
---
# 인터넷

## 01. 인터넷

### 01) 인터넷은 어떻게 작동 될까요?

1. 인터넷은 웹의 핵심적인 기술이다.

2. 인터넷의 가장 기본적인 것은, 컴퓨터들이 서로 통신 가능한 거대한 네트워크라는 것이다.

3. 인터넷의 어원

   1. 1973년 TCP/IP를 정립한 빈튼 서프와 로버트 칸이 "네트워크의 네트워크"를 구현하여 **모든 컴퓨터를 하나의 통신망 안에 연결(International Network)**하고자 하는 의도에서 이를 줄여 인터넷(Internet)이라고 처음 명명하였던 것에 어원을 두고 있다.

4. 인터넷의 변화

   1. 단순한 네트워크

      1. 1. 1:1 연결
            1. 두 대의 컴퓨터가 통신이 필요할 때, 우리는 다른 컴퓨터와 물리적으로 (보통 이더넷 케이블, 일반적으로 우리가 말하는 '랜선') 또는 무선으로 (WiFi 나 Bluetooth) 연결되어야 한다. 모든 현대 컴퓨터들은 이러한 연결 중 하나를 이용하여 연결을 지속할 수 있다.
         2. 多:多 연결
            1. 우리는 1:1로 연결하는 방식과 같은 방식으로 원하는만큼 컴퓨터를 연결할 수 있다. 하지만 이렇게 연결할 경우 컴퓨터의 수가 늘어날수록 매우 복잡해진다. 1:1로 연결하는 방식으로 10대의 컴퓨터를 연결한다고 생각해보자.
         3. 라우터 연결
            1. 위 문제를 해결하기 위해 네트워크의 각 컴퓨터는 **라우터(Router)라고하는 특수한 소형 컴퓨터**에 연결된다. 이 라우터는 단 하나의 작업만 있다. 철도역의 신호원처럼 **주어진 컴퓨터에서 보낸 메시지가 올바른 대상 컴퓨터에 도착하는지 확인**하는 것이다. 컴퓨터 B에게 메시지를 보내려면 컴퓨터 A가 메시지를 라우터로 보내야하며, 라우터는 메시지를 컴퓨터 B로 전달하고 메시지가 컴퓨터 C로 전달되지 않도록 해야 한다.

   2. 네트워크 속의 네트워크

      1. 컴퓨터를 라우터에 연결하고, 라우터에서 라우터로 연결함으로써 연결을 무한히 확장할 수 있다.

         

### 02) HTTP는 무엇일까요?

HTTP (HyperText Transfer Protocol)

텍스트 기반의 통신 규약으로 인터넷에서 데이터를 주고받을 수 있는 프로토콜이다. 이렇게 규약을 정해두었기 때문에 모든 프로그램이 이 규약에 맞춰 개발해서 서로 정보를 교환할 수 있게 되었다.

1. HTTP 동작

   클라이언트 즉, 사용자가 브라우저를 통해서 어떠한 서비스를 url을 통하거나 다른 것을 통해서 요청(request)을 하면 서버에서는 해당 요청사항에 맞는 결과를 찾아서 사용자에게 응답(response)하는 형태로 동작한다.

   - 요청 : client -> server
   - 응답 : server -> client

   HTML 문서만이 HTTP 통신을 위한 유일한 정보 문서는 아니다.
   Plain text로 부터 JSON 데이터 및 XML과 같은 형태의 정보도 주고 받을 수 있으며, 보통은 클라이언트가 어떤 정보를 HTML 형태로 받고 싶은지, JSON 형태로 받고 싶은지 명시해주는 경우가 많다.

2. HTTP 동작

   - HTTP 메시지는 HTTP 서버와 HTTP 클라이언트에 의해 해석이 된다.
   - TCP/ IP를 이용하는 응용 프로토콜이다.
     (컴퓨터와 컴퓨터간에 데이터를 전송 할 수 있도록 하는 장치로 인터넷이라는 거대한 통신망을 통해 원하는 정보(데이터)를 주고 받는 기능을 이용하는 응용 프로토콜)
   - HTTP는 연결 상태를 유지하지 않는 비연결성 프로토콜이다.
     (이러한 단점을 해결하기 위해 Cookie와 Session이 등장하였다.)
   - HTTP는 연결을 유지하지 않는 프로토콜이기 때문에 요청/응답 방식으로 동작한다.

   ![img](https://media.vlpt.us/post-images/surim014/e0aa5520-2d59-11ea-86da-fb3b00230640/image.png)

3. 예시로 알아보는 HTTP

   - **서버** : 어떠한 자료에 대한 접근을 관리하는 네트워크 상의 시스템 **(요청에 대한 응답을 보내준다.)**
   - **클라이언트** : 그 자료에 접근할 수 있는 프로그램
     Ex) 웹 브라우저, 핸드폰 어플리케이션 등...

   클라이언트 프로그램에서 사용자가 회원가입을 시도하게 되면, 서버로 회원정보를 보내게 되고 서버는 회원 정보를 저장해주기도 한다. 이 과정에서 **클라이언트와 서버 간의 교류가 HTTP라는 규약을 이용하여 발생하게 된다.**

4. Request(요청)

   **클라이언트가 서버에게 연락하는 것**을 요청이라고 하며 요청을 보낼때는 요청에 대한 정보를 담아 서버로 보낸다.

5. 예시로 알아보는 Request

   서버가 주문서를 받아 클라이언트가 어떤 것을 원하는지 파악할 수 있게 한다. 이처럼 **요청은 식당에서 주문서를 작성하는 것과 같다**고 생각하면 된다.

6. Request Method (요청의 종류)

   - **GET** : 자료를 **요청**할 때 사용
   - **POST** : 자료의 **생성**을 요청할 때 사용
   - **PUT** : 자료의 **수정**을 요청할 때 사용
   - **DELETE** : 자료의 **삭제**를 요청할 때 사용

7.  Request HTTP 메시지 예시

   ```null
   GET https://velog.io/@surim014 HTTP/1.1								// 시작줄
   User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) ...			  // 헤더
   Upgrade-Insecure-Requests: 1
   ```

   1. 시작줄 (첫 줄)

      첫 줄은 시작줄로 **메서드 구조 버전**으로 구성되었다.

   - GET : HTTP Method
   - https://velog.io/@surim014 : 사이트 주소
   - HTTP/1.1 : HTTP 버전

   

   2. 헤더 (두 번째 줄부터)

      두번째 줄부터는 헤더이며 **요청에 대한 정보**를 담고 있다. User-Agent, Upgrade-Insecure-Requests 등등이 헤더에 해당되며 헤더의 종류는 매우 많다.

   3. 본문(헤더에서 한 줄 띄고)

      본문은 **요청을 할 때 함께 보낼 데이터를 담는 부분**이다. 현재 예시에는 단순히 주소로만 요청을 보내고 있고 따로 데이터를 담아 보내지 않기 때문에 본문이 비어있다.

8. Response (응답)

   **서버가 요청에 대한 답변을 클라이언트에게 보내는 것**을 응답이라고 한다.



### 05) 도메인 네임은 무엇일까요?

**도메인 네임**(**Domain** name, 문화어: 령역이름)**은** 넓은 의미로는 네트워크상에서 컴퓨터를 식별하는 호스트명을 가리키며, 좁은 의미에서는 **도메인** 레지스트리에게서 등록된 이름을 의미한다. 이를 통틀어서 '웹 주소'라고 (잘못) 부르는 경우도 있다.



### 06) 호스팅은 무엇일까요?

웹 호스팅이란 개인이나 기관이 홈페이지를 운영하려고 할 때 서버 컴퓨터가 없는 사람들을 위해서 홈페이지 공간을 임대로 빌려주는 서비스를 말합니다. 웹 호스팅 서비스를 제공하는 업체는 웹사이트와 관련된 데이터를 서버에 저장하고 임차인의 홈페이지가 인터넷과 연결될 수 있도록 기술력을 제공합니다. 웹 호스팅의 장점으로는 저렴한 가격으로 자신의 홈페이지를 운영할 수 있다는 것과 서버 관리에 대해서 전혀 신경을 쓸 필요가 없다는 것입니다. 후자인 부분은 단점으로도 작용을 할 수가 있는데 서버에 문제가 생겼을 때 홈페이지의 주인이 에러를 건드릴 수 있는게 아니라 업체에서 제어를 해야하기 때문에 단점으로 작용할 수 있습니다.